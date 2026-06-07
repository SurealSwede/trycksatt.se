---
layout: default
title: Artiklar
permalink: /artiklar/
---

<div class="page-hero">
  <div class="container">
    <div class="page-eyebrow">Kunskapsbas</div>
    <h1 class="page-title">Artiklar</h1>
    <p class="page-lead">Tekniska djupdykningar i sprinklerteknik, hydraulik och normer. Skrivet för praktiker.</p>
  </div>
</div>

<div class="container">
  <div class="artiklar-list">
    {% for post in site.posts %}
    <a href="{{ post.url | relative_url }}" class="artikel-row">
      <span class="artikel-row-datum">{{ post.date | date: "%-d %b %Y" }}</span>
      <span class="artikel-row-title">{{ post.title }}</span>
      {% if post.kategori %}<span class="artikel-row-kategori">{{ post.kategori }}</span>{% endif %}
    </a>
    {% endfor %}
  </div>
</div>
