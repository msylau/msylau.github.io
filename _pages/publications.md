---
title: "Lau Lab - Publications"
layout: gridlay
excerpt: "Lau Lab -- Publications."
sitemap: false
permalink: /publications/
---

# Recent Publications

<div id="pub-list">
  {% for pub in site.data.publist %}
    <div class="pub-item" data-year="{{ pub.year }}" data-tags="{{ pub.tags | join: ',' }}">
      <strong>{{ pub.title }}</strong><br>
      <em>{{ pub.authors }}</em><br>
      {{ pub.journal }}, {{ pub.year }}<br>
      {% if pub.link and pub.link != "" %}
        <a href="{{ pub.link }}" target="_blank">[Link]</a>
      {% endif %}
      <br><br>
    </div>
  {% endfor %}
</div>
