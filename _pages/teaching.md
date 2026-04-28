---
layout: archive
title: "Teaching"
permalink: /teaching/
---

<style>
.course-card {
  border-left: 4px solid #2c7be5;
  background: #f9fbfd;
  padding: 15px 20px;
  margin-bottom: 20px;
  border-radius: 8px;
  transition: 0.3s;
}

.course-card:hover {
  background: #eef5ff;
  transform: translateY(-2px);
}

.course-title {
  font-weight: 600;
  font-size: 16px;
}

.course-level {
  float: right;
  color: #2c7be5;
  font-weight: 500;
}

.course-desc {
  margin-top: 5px;
  color: #555;
}
</style>

## 🎓 Teaching

{% for course in site.data.teaching %}
<div class="course-card">

  <div class="course-level">
    {{ course.level }}
  </div>

  <div class="course-title">
    {{ course.course }}
  </div>

  <div class="course-desc">
    {{ course.description }}
  </div>

</div>
{% endfor %}
