---
layout: page
title: GM Vault
description: Private campaign planning and secrets
permalink: /gm-vault-32f8a9/
nav_exclude: true
---

# GM-Only Content

This page is for the Game Master's eyes only. Players, turn back now!

---

## Campaign Planning

Content for campaign arcs, session prep, and long-term story development goes in `_gm/planning/`.

## Secret NPCs

Hidden NPC motivations, backgrounds, and stats go in `_gm/npcs/`.

## World Secrets

Unrevealed faction information, conspiracy details, and hidden lore go in `_gm/secrets/`.

---

{% assign groups = site.gm | group_by: "topic" | sort: 'name' %}
{% for group in groups %}

  {% if group.items.size > 0 %}
  <h2>{{ group.name }}</h2>
  <ul>
  {% assign items = group.items | sort: 'title' %}
  {% for doc in items %}
    <li><a href="{{ doc.url | relative_url }}">{{ doc.title }}</a>{% if doc.summary %} — {{ doc.summary }}{% endif %}</li>
  {% endfor %}
  </ul>
  {% endif %}
{% endfor %}

---

*Remember: This URL is obscured but not secured. Don't share it with players!*
