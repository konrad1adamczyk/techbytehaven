---
layout: default
title: "Home"
---

<section class="posts-list">
  {% for post in site.posts %}
    <article class="post-preview">
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <p><small>Published on {{ post.date | date: "%B %d, %Y" }}</small></p>
      <p>{{ post.excerpt }}</p>
      <a href="{{ post.url }}">Read more →</a>
    </article>
  {% endfor %}
</section>