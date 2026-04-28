---
layout: archive
title: "Professors"
permalink: /people/
---

<ul>
{% for prof in site.data.professors %}
  <li>
    <strong>{{ prof.name }}</strong> - {{ prof.field }}  
    📧 {{ prof.email }}
  </li>
{% endfor %}
</ul>
