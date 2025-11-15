---
layout: page
permalink: /team/
title: Team
description: Members of the QuISP team.
nav: true
nav_order: 2
---

<div class="team">
{% for member in site.team %}
  <div class="team-member">
    <img src="{{ member.avatar | relative_url }}" alt="{{ member.name }}" class="team-avatar">
    <h3>{{ member.name }}</h3>
    <p class="role">{{ member.role }}</p>
    <p class="email">{{ member.email }}</p>
    <div class="bio">
      {{ member.content }}
    </div>
  </div>
{% endfor %}
</div>
