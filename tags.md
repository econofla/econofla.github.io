---
layout: page
title: Tags
permalink: /tags/
---

<ul>
  {% assign tags_list = site.tags %}
  {% if tags_list %}
    {% for tag in tags_list %}
      <li>
        <a id="{{ tag[0] | slugify }}" href="{{ site.baseurl }}/tags/#{{ tag[0] | slugify }}">{{ tag[0] }}</a> ({{ tag[1].size }})
      </li>
    {% endfor %}
  {% endif %}
</ul>
