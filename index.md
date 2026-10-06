---
layout: default
title: 首页
---

<div style="display: flex; gap: 20px; margin-bottom: 30px; flex-wrap: wrap;">
  <a href="/91/" style="display: block; padding: 15px 30px; background-color: #333; color: #fff; text-decoration: none; border-radius: 8px; font-size: 20px; border: 1px solid #555;">
    91
  </a>
  <a href="/13/" style="display: block; padding: 15px 30px; background-color: #333; color: #fff; text-decoration: none; border-radius: 8px; font-size: 20px; border: 1px solid #555;">
    13
  </a>
  <a href="/78/" style="display: block; padding: 15px 30px; background-color: #333; color: #fff; text-decoration: none; border-radius: 8px; font-size: 20px; border: 1px solid #555;">
    78
  </a>
</div>

## main

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <small>{{ post.date | date: "%Y-%m-%d" }}</small>
    </li>
  {% endfor %}
</ul>
