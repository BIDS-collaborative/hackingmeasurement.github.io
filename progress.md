---
title: Progress
layout: page
exclude: true
---
### Enrolled students

<table class="table">
  <tr>
    <th>GitHub ID</th>
    <th>Committer to site?</th>
  </tr>
  {% for enrolled in site.data.enrolled %}
  <tr>
    <td>{{ enrolled.github_id }}</td>
    <td class="{{ enrolled.github_id }}"></td>
  </tr>
  {% endfor %}
</table>

<script>
var event_url = 'https://api.github.com/repos/BIDS-collaborative/' +
                'hackingmeasurement.github.io/events';

var ajax = new XMLHttpRequest();

// For now, keep event_data global
var event_data;
function get_commiters() {
    // The if clause appears to be critical, otherwise
    // we end up with malformed JSON. Weird!
    if (ajax.readyState == 4 && ajax.status == 200) {
        event_data = JSON.parse(ajax.responseText);
    }
}

// Actually do our AJAX request
ajax.open('GET', event_url, true);
ajax.onreadystatechange = get_commiters;
ajax.send(null);

</script>
