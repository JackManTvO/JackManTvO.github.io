---
layout: archives
title: Archives
description: 按年份归档
keywords: 归档
comments: false
menu: 归档
permalink: /archives/
---

<!-- Blog list -->
<ul id="posts-list">
    {% for post in site.posts %}
    <li class="posts-list-item">
        <div class="posts-content">
            <span class="posts-list-meta">{{ post.date | date: "%Y-%m-%d" }}</span>
            <a class="posts-list-name bubble-float-left" href="{{ site.url }}{{ post.url }}">{{ post.title }}</a>
            <span class='circle'></span>
        </div>
    </li>
    {% endfor %}
</ul>
