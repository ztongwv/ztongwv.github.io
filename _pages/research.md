---
layout: default
title: Research
permalink: /research/
---


<button onclick="switchLang('zh')" style="padding:8px 20px;margin:0 5px;background:#2c3e50;color:white;border:none;border-radius:4px;cursor:pointer;">中文</button>
<button onclick="switchLang('en')" style="padding:8px 20px;margin:0 5px;background:white;color:#2c3e50;border:1px solid #2c3e50;border-radius:4px;cursor:pointer;">English</button>


<div id="zh-content">
# 研究方向 & 成果
## 核心研究方向
1. 填写你的研究方向1（如：深度学习在医疗影像中的应用）
2. 填写你的研究方向2（如：联邦学习算法优化）

## 研究项目
1. 项目名称：XXX
   周期：XXXX-XXXX
   成果：XXX
</div>


<div id="en-content" style="display:none;">
# Research Directions & Achievements
## Core Research Directions
1. Fill in your research direction 1 (e.g.: Application of deep learning in medical imaging)
2. Fill in your research direction 2 (e.g.: Federated learning algorithm optimization)

## Research Projects
1. Project Name: XXX
   Period: XXXX-XXXX
   Achievements: XXX
</div>


<script>
function switchLang(lang) {
  document.getElementById('zh-content').style.display = lang === 'zh' ? 'block' : 'none';
  document.getElementById('en-content').style.display = lang === 'en' ? 'block' : 'none';
  document.title = lang === 'zh' ? '研究方向 & 成果 | Zhetong Zhang' : 'Research Directions & Achievements | Zhetong Zhang';
}

window.onload = () => switchLang('zh');
</script>
