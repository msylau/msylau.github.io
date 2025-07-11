---
title: "News"
layout: textlay
excerpt: "Allan Lab at Leiden University."
sitemap: false
permalink: /allnews.html
---

# News
<ul class="news-list">
  {% for article in site.data.news %}
    <li class="news-item">
      <strong>{{ article.date }}</strong><br>
      {{ article.headline | markdownify }}
    </li>
  {% endfor %}
</ul>
