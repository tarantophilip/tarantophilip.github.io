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
  <div class="team-member" style="display: flex; align-items: flex-start; margin: 2rem 0; gap: 2rem;">
    <div class="team-avatar-container">
      <img src="{{ member.avatar | relative_url }}" alt="{{ member.name }}" class="team-avatar" style="width: 150px; height: 150px; border-radius: 50%; object-fit: cover;">
    </div>
    <div class="team-info" style="text-align: left; flex: 1;">
      <h3 style="margin-top: 0;">{{ member.name }}</h3>
      <p class="role"><em>{{ member.role }}</em></p>
      <p class="email">{{ member.email }}</p>
      <div class="bio">
        {{ member.content | markdownify }}
      </div>
    </div>
  </div>
  <hr style="margin: 2rem 0;">
{% endfor %}
</div>
