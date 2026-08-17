---
layout: page
title: Articles
permalink: /articles/
---

Tous mes articles consacrés aux politiques publiques de l'énergie.

<div class="article-list">

{% for post in site.posts %}

<div class="article-list-item">

  <div class="article-date">
    {{ post.date | date: "%d/%m/%Y" }}
  </div>

  <div class="article-title">
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
  </div>

</div>

{% endfor %}

</div>
