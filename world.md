---
layout: page
title: Galaxy
description: Factions, locations, characters, and the harsh realities of the outer sectors
permalink: /world/
---

This page contains player-facing information about the galaxy of Stardust Liar – the corrupt systems, syndicate territories, desperate communities, and the people trying to survive in the margins.

Information is added here as it's discovered during the campaign.

{% assign groups = site.world | group_by: "topic" | sort: 'name' %}
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

*The galaxy is vast. Most of it is controlled by syndicates, corrupt governors, or nobody at all. This is what we've seen so far.*
