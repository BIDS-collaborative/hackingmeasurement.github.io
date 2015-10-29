---
title: Progress
layout: page
exclude: true
---
### Enrolled students

<table class="table">
  <tr>
    <th>GitHub ID</th>
    <th>Project</th>
    <th>Evaluate</th>
    <th style="text-align:center">Committer to site?</th>
  </tr>
  {% for enrolled in site.data.enrolled %}
  <tr>
    <td>{{ enrolled.github_id }}</td>
    <td>{{ enrolled.project }}</td>
    <td>{{ enrolled.evaluate }}</td>
    <td id="{{ enrolled.github_id }}-committed" style="text-align:center"></td>
  </tr>
  {% endfor %}
</table>

<script>
// Isolate our JavaScript
(function() {
  var event_url = 'https://api.github.com/repos/BIDS-collaborative/' +
                  'hackingmeasurement.github.io/events';

  var ajax = new XMLHttpRequest();

  // For now, keep event_data global
  var event_data;
  ajax.onreadystatechange = function() {
      var qualifying_event = ['PushEvent', 'PullRequestEvent'];

      // The if clause appears to be critical, otherwise
      // we end up with malformed JSON. Weird!
      if(ajax.readyState == 4 && ajax.status == 200) {
          var event_data = JSON.parse(ajax.responseText);
          for(var i in event_data) {
              // .indexOf() is -1 if the item is not found
              if(qualifying_event.indexOf(event_data[i].type) !== -1) {
                  // We created elements with class based on username above
                  var id = event_data[i].actor.login + '-committed';
                  var target = document.getElementById(id);
                  if(target) {
                      target.innerHTML = 'X';
                  }
              }
          }

          // Maybe wrap in try / catch?
          var link_header = ajax.getResponseHeader('Link');
          var matches = link_header.match(/<([^,]*?)>; rel="next"/);
          if(matches) {
              console.log('visiting', matches[1]);
              ajax.open('GET', matches[1], true);
              ajax.send(null);
          }
      }
  }

  // Actually do our AJAX request
  ajax.open('GET', event_url, true);
  ajax.send(null);
})();
</script>
