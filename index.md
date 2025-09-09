---
layout: single
title: Home
author_profile: false
classes: wide
---

{% assign hint = "style='margin:6px 0 18px; color:#6b7280; font-size:.95rem;'" %}

## 림프종
<p {{ hint }}>최신 글 3개</p>
{% for post in site.categories["림프종"] limit:3 %}
- [{{ post.title }}]({{ post.url | relative_url }}) — {{ post.excerpt | default: post.content | strip_html | truncate: 120 }}
{% else %}
- (아직 글 없음)
{% endfor %}

---

## 운동
<p {{ hint }}>최신 글 3개</p>
{% for post in site.categories["운동"] limit:3 %}
- [{{ post.title }}]({{ post.url | relative_url }}) — {{ post.excerpt | default: post.content | strip_html | truncate: 120 }}
{% else %}
- (아직 글 없음)
{% endfor %}

---

## 산문
<p {{ hint }}>최신 글 3개</p>
{% for post in site.categories["산문"] limit:3 %}
- [{{ post.title }}]({{ post.url | relative_url }}) — {{ post.excerpt | default: post.content | strip_html | truncate: 120 }}
{% else %}
- (아직 글 없음)
{% endfor %}

---

## 직장
<p {{ hint }}>최신 글 3개</p>
{% for post in site.categories["직장"] limit:3 %}
- [{{ post.title }}]({{ post.url | relative_url }}) — {{ post.excerpt | default: post.content | strip_html | truncate: 120 }}
{% else %}
- (아직 글 없음)
{% endfor %}
