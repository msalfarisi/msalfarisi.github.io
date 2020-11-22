---
permalink: /
title: "Home"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

## News 最新情報

{% for post in site.posts limit:5 %}
  <li><span>{{ post.date | date_to_string }}</span> » <a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a></li>
{% endfor %}

[Older updates](/news/)
