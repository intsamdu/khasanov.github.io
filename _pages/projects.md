---
layout: archive
title: "Projects"
permalink: /projects/
---

<style>
.project-card {
  border-left: 4px solid #28a745;
  background: #f8fff9;
  padding: 15px 20px;
  margin-bottom: 20px;
  border-radius: 8px;
  transition: 0.3s;
}

.project-card:hover {
  background: #eaffea;
  transform: translateY(-2px);
}

.project-title {
  font-weight: 600;
  font-size: 16px;
}

.project-role {
  color: #555;
  margin-top: 5px;
}

.project-desc {
  margin-top: 5px;
}

.project-funding {
  float: right;
  color: #28a745;
  font-weight: 500;
}
</style>

## 🚀 Projects

{% for proj in site.data.projects %}
<div class="project-card">

  <div class="project-funding">
    {{ proj.funding }}
  </div>

  <div class="project-title">
    {{ proj.title }}
  </div>

  <div class="project-role">
    {{ proj.role }}
  </div>

  <div class="project-desc">
    {{ proj.description }}
  </div>

</div>
{% endfor %}
