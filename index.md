---
layout: default
title: "Happy coding"
---

<div class="p-6 max-w-sm mx-auto bg-white dark:bg-slate-700 rounded-xl shadow-lg flex items-center space-x-4">
  <div class="shrink-0">
    <img class="rounded-full h-12 w-12" src="{{ "/assets/img/me-bucket-hat.png" | relative_url }}" alt="Anime me">
  </div>
  <div>
    <div class="text-xl font-medium text-black dark:text-blue-300">Alex Tsui</div>
    <p class="text-slate-500 dark:text-white">Hi, thanks for stopping by this humble developer's webpage. Feel free to take a look around.</p>
  </div>
</div>
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
