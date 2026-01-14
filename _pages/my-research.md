

---
layout: default               # 必须加：继承模板样式，和首页保持一致
permalink: /my-research/      # 改：和导航栏url完全一致，唯一路径
title: "我的研究"             # 页面标题
excerpt: ""
author_profile: true
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>

## 核心研究方向
### 计算机视觉
1.  目标检测：RT-DETR 模型轻量化与精度优化
2.  边缘计算：低 GFLOPs 模型的实时推理部署

### 已开展项目
- 面向自动驾驶的 RT-DETR 改进算法研究（2024-2025）
- 工业质检场景的轻量化目标检测系统开发（2023-2024）
