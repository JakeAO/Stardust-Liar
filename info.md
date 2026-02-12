---
layout: page
title: Rules & Info
description: Stars Without Number rules, mechanics, and cheat sheets
permalink: /info/
---

This page contains player-facing rules clarifications, cheat sheets, and game mechanics for the Stardust Liar campaign.

## Core Resources

- **[Core Rulebook (Deluxe Edition)]({{ site.baseurl }}/info/mechanics/core-rulebook/)** – The full deluxe rulebook used for this campaign
- **[Stars Without Number: Revised Free Edition](https://www.drivethrurpg.com/product/230009/Stars-Without-Number-Revised-Edition-Free-Version)** – The complete free rulebook
- **[SWN Resources on Dicegeeks](https://www.dicegeeks.com/stars-without-number-rpg-character-sheet/)** – Character sheets, faction sheets, and flowcharts
- **[SWN Faction Spreadsheet](https://d0ngiovanni.github.io/swn-faction-spreadsheet/)** – Automated faction turn management
- **[r/SWN Community](https://www.reddit.com/r/SWN/)** – Active community with resources and advice

## Quick Reference

Below are campaign-specific resources and rules clarifications, organized by topic.

{% assign groups = site.info | group_by: "topic" | sort_natural: "name" %}
{% for group in groups %}

  {% assign has_content = false %}
  {% for doc in group.items %}
  {% unless doc.tags contains "nested" %}
  {% assign has_content = true %}
  {% endunless %}
  {% endfor %}

  {% if has_content %}
  <h3>{{ group.name }}</h3>
  <ul>
  {% assign items = group.items | sort: "title" %}
  {% for doc in items %}
  {% unless doc.tags contains "nested" %}
    <li><a href="{{ doc.url | relative_url }}">{{ doc.title }}</a>{% if doc.summary %} — {{ doc.summary }}{% endif %}</li>
  {% endunless %}
  {% endfor %}
  </ul>
  {% endif %}
{% endfor %}

---

*New to Stars Without Number? Start by viewing the [Core Rulebook]({{ site.baseurl }}/info/mechanics/core-rulebook/) and reading the Quick Reference on page 59.*
