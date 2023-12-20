---
layout: default
work: true
main: true
title: Project, 개발에 참여한 프로젝트
---

<div class="catalogue">
{% assign sorted = site.pages | sort: 'order' | reverse %}
{% for page in sorted %}
{% if page.projects == true %}

     {% include post-list.html %}

{% endif %}
{% endfor %}

</div>
