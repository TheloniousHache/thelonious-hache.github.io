---
layout: page
title: Articles
permalink: /articles/
---

Tous mes articles consacrés aux politiques publiques de l'énergie.

<div class="article-list">

{% for post in site.posts %}

<article class="article-list-item">

  <p class="post-date">
    {{ post.date | date: "%d/%m/%Y" }}
  </p>

  <h2>
    <a href="{{ post.url | relative_url }}">
      {{ post.title }}
    </a>
  </h2>

  {% if post.excerpt %}
    <p>
      {{ post.excerpt | strip_html | truncatewords: 40 }}
    </p>
  {% endif %}

</article>

{% endfor %}

</div>
