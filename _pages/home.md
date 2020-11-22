---
permalink: /
title: "Home"
excerpt: "Home"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

## Welcome ようこそ

Welcome to the homepage of Muhammad Salman Al Farisi, a graduate student & JSPS research fellow at Department of Robotics, Graduate School of Engineering, Tohoku University, in Japan.

アル・ファリシィ　ムハンマド・サルマンのホームページへようこそ！東北大学大学院工学研究科ロボティクス専攻博士後期課程学生・日本学術振興会特別研究員です。

## News 最新情報

{% for post in site.posts limit:5 %}
  <li><span>{{ post.date | date_to_string }}</span> » <a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a></li>
{% endfor %}

[Older updates](/news/)
