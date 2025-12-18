---
layout: default
title: Home
---

# Today I Learned

데이터 사이언스 & 개발 공부 기록을 모아두는 TIL 페이지입니다.

## 최근 TIL

<ul>
  {% for post in site.til reversed limit:10 %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <span> – {{ post.date | date: "%Y-%m-%d" }}</span>
    </li>
  {% endfor %}
</ul>
