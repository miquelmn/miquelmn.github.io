---
title: "Teaching"
permalink: /teaching/
layout: single
author_profile: true
---

{% raw %}<div class="teaching-wrap">

{% assign courses = site.teaching | group_by: "course" %}
{% for course in courses %}
  {% assign items = course.items | sort: "date" | reverse %}
  <div class="teaching-course-block">
    <h2 class="teaching-course-title">{{ course.name }}</h2>
    <p class="teaching-course-sub">{{ items.first.semester }}</p>

    <div class="teaching-grid">
      {% for item in items %}
      <a class="teaching-card" href="{{ item.pdf }}" target="_blank" rel="noopener">
        <div class="teaching-card-thumb">
          {% if item.thumbnail %}
            <img src="{{ item.thumbnail }}" alt="{{ item.title }} thumbnail" loading="lazy">
          {% else %}
            <i class="fas fa-file-pdf teaching-card-icon"></i>
          {% endif %}
          <span class="teaching-card-badge"><i class="fas fa-file-pdf"></i> PDF</span>
        </div>
        <div class="teaching-card-body">
          <h3>{{ item.title }}</h3>
          <time>{{ item.date | date: "%B %-d, %Y" }}</time>
          {% if item.excerpt %}<p>{{ item.excerpt }}</p>{% endif %}
        </div>
      </a>
      {% endfor %}
    </div>
  </div>
{% endfor %}

</div>{% endraw %}