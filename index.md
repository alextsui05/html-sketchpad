---
layout: default
title: "Happy coding"
---

<div class="py-6">
  <h1 class="text-4xl py-3">Posts</h1>
  <ul>
    {% for post in site.posts %}
      <li>
        <span class="font-bold pr-2">{{ post.date | date: "%Y-%m-%d" }}</span><a href="{% link {{ post.path }} %}">{{ post.title }}</a>
      </li>
    {% endfor %}
  </ul>
</div>
