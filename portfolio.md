---
title: Portfolio
layout: default
permalink: /portfolio/
has_children: false
---

# Portfolio
{: .no_toc }

<p>
{% for category in site.categories %}
  <h4 name="{{ category | first }}" style="list-style: none !important;">{{ category | first }}</h4>
  {% for post in category.last %}
    <li style="list-style: none !important;"><a href="{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
{% endfor %}
</p>
