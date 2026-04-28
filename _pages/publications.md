---
layout: archive
title: "Publications"
permalink: /publications/
---

<style>
.pub-card {
  border-left: 4px solid #2c7be5;
  background: #f9fbfd;
  padding: 15px 20px;
  margin-bottom: 20px;
  border-radius: 8px;
  transition: 0.3s;
}

.pub-card:hover {
  background: #eef5ff;
  transform: translateY(-2px);
}

.pub-title {
  font-weight: 600;
  font-size: 16px;
  color: #1a1a1a;
}

.pub-authors {
  color: #555;
  margin-top: 5px;
}

.pub-journal {
  font-style: italic;
  color: #2c7be5;
  margin-top: 5px;
}

.pub-year {
  float: right;
  color: #888;
}
</style>

## 📄 Publications

{% assign pubs = site.data.publications | sort: "year" | reverse %}

{% for pub in pubs %}
<div class="pub-card">

  <div class="pub-year">{{ pub.year }}</div>

  <div class="pub-title">
    {% if pub.doi %}
      <a href="{{ pub.doi }}" style="text-decoration:none; color:#1a1a1a;">
        {{ pub.title }}
      </a>
    {% else %}
      {{ pub.title }}
    {% endif %}
  </div>

  <div class="pub-authors">
    {{ pub.authors }}
  </div>

  <div class="pub-journal">
    {{ pub.journal }}
  </div>

  <div style="margin-top:8px;">
  {% if pub.pdf %}
    <a href="{{ pub.pdf }}" style="margin-right:10px; text-decoration:none; color:#2c7be5;">📄 PDF</a>
  {% endif %}
  
  {% if pub.doi %}
    <a href="{{ pub.doi }}" style="text-decoration:none; color:#2c7be5;">🔗 DOI</a>
  {% endif %}
</div>

</div>
{% endfor %}
