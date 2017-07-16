---
layout: page
title: About
description: 天地之间，风华无限
keywords: JeetChan, 风华
comments: true
menu: 关于
permalink: /about/
---

关注编程、科学、思维、在线教育

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
