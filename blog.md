---
layout: page
title: Blogs
background: grey
---
<h1>Latest Posts</h1>

<ul>
  {% for post in site.posts %}
    <li>
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      {{ post.excerpt  | strip_html | strip_newlines | truncate: 156 }}  

    </li>
  {% endfor %}
</ul>