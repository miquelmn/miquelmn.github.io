---
title: "Paper Reading Club"
permalink: /paper-club/
layout: single
author_profile: true
classes: wide
---

Our research group meet regularly to read and discuss a recent paper. Read the paper before the session; whoever presents walks us through the main ideas, and then we discuss them together.

{% assign sessions = site.data.paper_club | sort: "date" %}
{% assign today = site.time | date: "%Y-%m-%d" %}
{% assign upcoming = "" | split: "" %}
{% assign past = "" | split: "" %}
{% for s in sessions %}
  {% assign d = s.date | date: "%Y-%m-%d" %}
  {% if d >= today %}
    {% assign upcoming = upcoming | push: s %}
  {% else %}
    {% assign past = past | push: s %}
  {% endif %}
{% endfor %}

<div class="paper-club">

{% if upcoming.size > 0 %}
  <h2 class="paper-club-heading">Next paper</h2>
  {% include paper-club-card.html session=upcoming.first featured=true %}

  {% if upcoming.size > 1 %}
  <h2 class="paper-club-heading">Upcoming</h2>
  {% for s in upcoming offset:1 %}
    {% include paper-club-card.html session=s %}
  {% endfor %}
  {% endif %}
{% else %}
  <p class="paper-club-empty">No upcoming session scheduled yet. Stay tuned!</p>
{% endif %}

{% if past.size > 0 %}
  <h2 class="paper-club-heading">Past sessions</h2>
  {% assign past = past | reverse %}
  {% for s in past %}
    {% include paper-club-card.html session=s %}
  {% endfor %}
{% endif %}

</div>
