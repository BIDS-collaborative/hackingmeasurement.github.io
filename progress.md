---
title: Progress
layout: page
exclude: true
---
### Enrolled students

<table class="table">
  <tr>
    <th>GitHub ID</th>
    <th style="text-align:center">Committer to site?</th>
  </tr>
  {% for enrolled in site.data.enrolled %}
  <tr>
    <td>{{ enrolled.github_id }}</td>
    <td id="{{ enrolled.github_id }}-committed" style="text-align:center"></td>
  </tr>
  {% endfor %}
</table>

<script>
var event_url = 'https://api.github.com/repos/BIDS-collaborative/' +
                'hackingmeasurement.github.io/events';

var ajax = new XMLHttpRequest();

// For now, keep event_data global
var event_data;
ajax.onreadystatechange = function() {
    // The if clause appears to be critical, otherwise
    // we end up with malformed JSON. Weird!
    if(ajax.readyState == 4 && ajax.status == 200) {
        event_data = JSON.parse(ajax.responseText);
        for(var i in event_data) {
            // We created elements with class based on username above
            var id = event_data[i].actor.login + '-committed';
            var target = document.getElementById(id);
            if(target) {
                target.innerHTML = 'X';
            }
        }
    }
}

// Actually do our AJAX request
ajax.open('GET', event_url, true);
ajax.send(null);

</script>
