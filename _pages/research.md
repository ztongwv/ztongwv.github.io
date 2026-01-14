---
layout: default
title: Research
permalink: /research/
---

<!-- 中英文切换按钮 -->
<div style="margin: 30px 0; text-align: center;">
  <button onclick="switchLang('zh')" style="padding: 10px 24px; margin: 0 8px; border: none; border-radius: 6px; background: #2c3e50; color: white; cursor: pointer; font-size: 16px;">中文</button>
  <button onclick="switchLang('en')" style="padding: 10px 24px; margin: 0 8px; border: 1px solid #2c3e50; border-radius: 6px; background: white; color: #2c3e50; cursor: pointer; font-size: 16px;">English</button>
</div>

<!-- 中文内容区块 -->
<div id="zh-content" style="line-height: 1.8; font-size: 16px; color: #333;">
  <h1>研究方向 & 成果</h1>
  <h2>核心研究方向</h2>
  <ol style="margin-left: 20px; line-height: 2;">
    <li>填写你的研究方向1（如：深度学习在医疗影像中的应用）</li>
    <li>填写你的研究方向2（如：联邦学习算法优化）</li>
  </ol>

  <h2 style="margin-top: 30px;">研究项目</h2>
  <ol style="margin-left: 20px; line-height: 2;">
    <li>
      <strong>项目名称：</strong>XXX<br>
      <strong>周期：</strong>XXXX-XXXX<br>
      <strong>成果：</strong>XXX
    </li>
  </ol>
</div>

<!-- 英文内容区块（默认隐藏） -->
<div id="en-content" style="display: none; line-height: 1.8; font-size: 16px; color: #333;">
  <h1>Research Directions & Achievements</h1>
  <h2>Core Research Directions</h2>
  <ol style="margin-left: 20px; line-height: 2;">
    <li>Fill in your research direction 1 (e.g.: Application of deep learning in medical imaging)</li>
    <li>Fill in your research direction 2 (e.g.: Federated learning algorithm optimization)</li>
  </ol>

  <h2 style="margin-top: 30px;">Research Projects</h2>
  <ol style="margin-left: 20px; line-height: 2;">
    <li>
      <strong>Project Name：</strong>XXX<br>
      <strong>Period：</strong>XXXX-XXXX<br>
      <strong>Achievements：</strong>XXX
    </li>
  </ol>
</div>

<!-- 切换逻辑JS -->
<script>
// 切换语言核心函数
function switchLang(lang) {
  // 隐藏所有语言区块
  document.getElementById('zh-content').style.display = 'none';
  document.getElementById('en-content').style.display = 'none';
  // 显示选中的语言区块
  document.getElementById(lang + '-content').style.display = 'block';
  // 同步修改页面标题
  if (lang === 'zh') {
    document.title = '研究方向 & 成果 | Zhetong Zhang';
  } else {
    document.title = 'Research Directions & Achievements | Zhetong Zhang';
  }
}

// 页面加载默认显示中文
window.onload = function() {
  switchLang('zh');
};
</script>

<!-- 样式优化（可选，提升美观度） -->
<style>
  h1 {
    color: #2c3e50;
    border-bottom: 2px solid #eee;
    padding-bottom: 10px;
    margin-bottom: 20px;
  }
  h2 {
    color: #34495e;
    margin-top: 25px;
  }
  li {
    margin-bottom: 10px;
  }
  button:hover {
    opacity: 0.9;
    transition: opacity 0.2s ease;
  }
</style>
