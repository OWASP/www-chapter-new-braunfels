---

layout: col-sidebar
title: OWASP New Braunfels Past Events
tags: chapter, New Braunfels, Texas, NBTX

---

{% include top_nav.md page="pastactivities" %}
{%if site.data.pastactivities == false or site.data.pastactivities.size < 1 %}
There are no past activities.
{%else%}
{% assign activities = site.data.pastactivities | sort: "start-date" | reverse %}
{% for activity in activities %}
<hr>
{:class='activity'}
* ### {{ activity.name }}

  **What: {{ activity.type | capitalize }}**<br>
  **Date: {{ activity.start-date }}{% if activity.start-date != activity.end-date %} - {{ activity.end-date }}{% endif %}**<br>
  **Time: {{ activity.start_time }} - {{ activity.end_time }}**<br>
  **Description:**
  {{ activity.description }}<br>

{%endfor%}
{%endif%}