---
layout: page
title: About
description: 关于刘茂密
keywords: 刘茂密, Jack Liu
comments: true
menu: 关于
permalink: /about/
---

我是刘茂密，用着模板作博客的小学生。

追求「有趣、求知、自强」。

## 联系

{% for website in site.data.social %}

* {{ website.sitename }}：[@{{ website.name }}]({{ website.url }})
{% endfor %}

## Skill Keywords

{% for category in site.data.skills %}

### {{ category.name }}

<div class="btn-inline">

{% for keyword in category.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}
