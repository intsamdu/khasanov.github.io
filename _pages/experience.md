---
layout: archive
title: "Experience"
permalink: /experience/
---

<style>
.timeline {
  border-left: 3px solid #6c757d;
  padding-left: 20px;
}

.exp-item {
  margin-bottom: 25px;
  position: relative;
}

.exp-item::before {
  content: "";
  position: absolute;
  left: -10px;
  top: 5px;
  width: 12px;
  height: 12px;
  background: #6c757d;
  border-radius: 50%;
}

.exp-title {
  font-weight: 600;
  font-size: 16px;
}

.exp-place {
  color: #2c7be5;
}

.exp-period {
  color: #888;
  font-size: 14px;
}

.exp-desc {
  margin-top: 5px;
}
</style>

## 💼 Professional Experience

<div class="timeline">
{% for exp in site.data.experience %}
  <div class="exp-item">
    <div class="exp-title">{{ exp.title }}</div>
    <div class="exp-place">{{ exp.place }}</div>
    <div class="exp-period">{{ exp.period }}</div>
    <div class="exp-desc">{{ exp.description }}</div>
  </div>
{% endfor %}
</div>
