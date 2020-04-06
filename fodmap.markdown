---
layout: page
title: Fodmap
permalink: /fodmap/
---


<h2>High in Fodmap, to avoid...</h2>
<table>
{% for category in site.data.fodmap-list.list["high FODMAP"] %}
  <tr>
    <th> {{ category[0] }} </th>
  </tr>
  {% for item in category[1] %}
  <tr>
      <td>{{ item }}</td>
  </tr>
  {% endfor %}
{% endfor %}
</table>

<h2>Low in Fodmap</h2>
<table>
{% for category in site.data.fodmap-list.list["low FODMAP"] %}
  <tr>
    <th> {{ category[0] }} </th>
  </tr>
  {% for item in category[1] %}
  <tr>
      <td>{{ item }}</td>
  </tr>
  {% endfor %}
{% endfor %}
</table>