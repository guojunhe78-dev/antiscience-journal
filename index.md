---
layout: default
title: AntiScience Journal
---

欢迎来到 **AntiScience Journal
——文明发展的绊脚石**！  

最新文章：
{% for post in site.posts %}
- [{{ post.title }}]({{ post.url }}) - {{ post.date | date: "%Y-%m-%d" }}
{% endfor %}
{% for post in site.posts %}
<div class="post-preview">
  <img src="{{ post.cover }}" alt="{{ post.title }}" />
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <p>{{ post.date | date: "%Y-%m-%d" }}</p>
</div>
{% endfor %}
