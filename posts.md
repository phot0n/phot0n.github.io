---
title: /posts
permalink: /posts
layout: default
---

Just a place to writeout my thoughts, new learnings ,etc  :)

{% comment %} refer: https://jekyllrb.com/docs/posts {% endcomment %}

<br>

<ul>
  {% if site.posts.size != 0 %}
    {% for post in site.posts %}
      <li>
          {%- assign date_format = "%Y-%m-%d" -%}
          [ {{ post.date | date: date_format }} ] - <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      </li>
    {% endfor %}
  {% else %}
    Oops!! Nothing is here - maybe I'm lazying around or wandering into abyss.
  {% endif %}
</ul>
