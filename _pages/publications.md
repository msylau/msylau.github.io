---
title: "Lau Lab - Publications"
layout: gridlay
excerpt: "Lau Lab -- Publications."
sitemap: false
permalink: /publications/
---

# Selected Publications

{% for pub in site.data.publist %}
<div class="pub-item" data-year="{{ pub.year }}" data-tags="{{ pub.tags | join: ',' }}">
  <strong>{{ pub.title }}</strong><br>
  <em>{{ pub.authors }}</em><br>
  {{ pub.journal }}, {{ pub.year }}<br>
  {% if pub.link %}
    <a href="{{ pub.link }}" target="_blank">[Link]</a>
  {% endif %}
  <br><br>
</div>
{% endfor %}
