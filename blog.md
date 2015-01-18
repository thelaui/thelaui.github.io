---
layout: page
title: Blog
---

<ul class="post-list hbox">
  {% for post in site.posts %}
    <li class="overlay post-entry">
      <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

      <h2>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </h2>
    </li>
  {% endfor %}
</ul>
