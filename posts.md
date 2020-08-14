---
title: /posts
permalink: /posts/
---

Just a place to writeout my thoughts, new learnings ,etc  :)

<br>

<ul>
  {% for post in site.posts %}
    <li>
        {%- assign date_format = "%Y-%m-%d" -%}
        [ {{ post.date | date: date_format }} ] - <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
