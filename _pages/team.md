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
  <div class="team-member" style="text-align: center; margin: 2rem 0;">
    <img src="{{ member.avatar | relative_url }}" alt="{{ member.name }}" class="team-avatar" style="width: 200px; height: 200px; border-radius: 50%; object-fit: cover;">
    <h3>{{ member.name }}</h3>
    <p class="role"><em>{{ member.role }}</em></p>
    <p class="email">{{ member.email }}</p>
    <div class="bio">
      {{ member.content }}
    </div>
  </div>
{% endfor %}
</div>
