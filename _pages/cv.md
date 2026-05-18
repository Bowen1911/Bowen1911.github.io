---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

<html lang="zh-CN">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>李孙博闻 - 学术简历</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600&family=Noto+Serif+SC:wght@400;600&family=JetBrains+Mono:wght@400&display=swap');

  :root {
    --primary: #1a1a2e;
    --accent: #0f6e56;
    --accent-light: #e1f5ee;
    --text: #2c2c2a;
    --text-muted: #5f5e5a;
    --text-light: #888780;
    --border: #e0dfd8;
    --bg: #fafaf8;
    --card-bg: #ffffff;
    --tag-bg: #e6f1fb;
    --tag-text: #185fa5;
  }

  * { margin: 0; padding: 0; box-sizing: border-box; }

  body {
    font-family: 'Inter', 'Noto Serif SC', -apple-system, sans-serif;
    background: var(--bg);
    color: var(--text);
    line-height: 1.6;
    font-size: 13.5px;
  }

  .page {
    max-width: 880px;
    margin: 0 auto;
    padding: 36px 36px;
    background: var(--card-bg);
    min-height: 100vh;
  }

  @media print {
    @page {
      size: A4;
      margin: 15mm 18mm;
    }
    body {
      background: white;
      -webkit-print-color-adjust: exact;
      print-color-adjust: exact;
    }
    .page {
      padding: 0;
      box-shadow: none;
      max-width: 100%;
    }
    .pub-item, .exp-item, .summary-bar, .tag {
      break-inside: avoid;
    }
    .section-title {
      break-after: avoid;
    }
    .print-hint { display: none !important; }
  }

  /* Header */
  .header {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    margin-bottom: 20px;
    padding-bottom: 16px;
    border-bottom: 2px solid var(--primary);
  }

  .header-left h1 {
    font-size: 26px;
    font-weight: 600;
    color: var(--primary);
    letter-spacing: -0.5px;
    margin-bottom: 2px;
  }

  .header-left .cn-name {
    font-family: 'Noto Serif SC', serif;
    font-size: 15px;
    color: var(--text-muted);
  }

  .header-right {
    text-align: right;
    font-size: 12.5px;
    color: var(--text-muted);
    line-height: 1.7;
  }

  .header-right a {
    color: var(--accent);
    text-decoration: none;
    border-bottom: 1px solid transparent;
    transition: border-color 0.2s;
  }

  .header-right a:hover {
    border-bottom-color: var(--accent);
  }

  .contact-item {
    display: flex;
    align-items: center;
    justify-content: flex-end;
    gap: 5px;
  }

  .contact-icon {
    width: 13px;
    height: 13px;
    opacity: 0.5;
  }

  /* Summary bar */
  .summary-bar {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    margin-bottom: 20px;
    padding: 10px 16px;
    background: var(--accent-light);
    border-radius: 8px;
    font-size: 12.5px;
  }

  .summary-item {
    display: flex;
    align-items: center;
    gap: 5px;
  }

  .summary-label {
    font-weight: 500;
    color: var(--accent);
  }

  .summary-value {
    color: var(--text);
  }

  .divider {
    width: 1px;
    background: var(--accent);
    opacity: 0.3;
    align-self: stretch;
  }

  /* Section */
  .section {
    margin-bottom: 20px;
  }

  .section-title {
    font-size: 14px;
    font-weight: 600;
    color: var(--primary);
    text-transform: uppercase;
    letter-spacing: 1.5px;
    margin-bottom: 10px;
    padding-bottom: 4px;
    border-bottom: 1px solid var(--border);
  }

  /* Education */
  .edu-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 12px;
  }

  .edu-degree {
    font-weight: 600;
    font-size: 13px;
    color: var(--text);
  }

  .edu-school {
    color: var(--text-muted);
    font-size: 12px;
  }

  .edu-date {
    color: var(--text-light);
    font-size: 11.5px;
    font-family: 'JetBrains Mono', monospace;
  }

  /* Publications */
  .pub-category {
    margin-bottom: 14px;
  }

  .pub-category-title {
    font-size: 12.5px;
    font-weight: 500;
    color: var(--accent);
    margin-bottom: 8px;
    display: flex;
    align-items: center;
    gap: 8px;
  }

  .pub-category-title::after {
    content: '';
    flex: 1;
    height: 0.5px;
    background: var(--border);
  }

  .pub-item {
    margin-bottom: 8px;
    padding-left: 14px;
    border-left: 2px solid var(--accent-light);
    transition: border-color 0.2s;
  }

  .pub-item:hover {
    border-left-color: var(--accent);
  }

  .pub-title {
    font-weight: 500;
    font-size: 13.5px;
    color: var(--text);
    line-height: 1.45;
  }

  .pub-title a {
    color: var(--text);
    text-decoration: none;
    border-bottom: 1px solid var(--border);
    transition: border-color 0.2s;
  }

  .pub-title a:hover {
    border-bottom-color: var(--accent);
  }

  .pub-meta {
    font-size: 12px;
    color: var(--text-muted);
    margin-top: 1px;
  }

  .pub-venue {
    display: inline-block;
    font-size: 11px;
    font-weight: 500;
    padding: 1px 7px;
    border-radius: 3px;
    margin-right: 5px;
  }

  .venue-a { background: #fcebeb; color: #a32d2d; }
  .venue-b { background: #e6f1fb; color: #185fa5; }
  .venue-sci { background: #eaf3de; color: #3b6d11; }
  .venue-preprint { background: #f1efe8; color: #5f5e5a; }
  .venue-findings { background: #fbeaf0; color: #72243e; }

  /* Experience */
  .exp-item {
    margin-bottom: 10px;
    padding: 10px 14px;
    background: var(--card-bg);
    border: 0.5px solid var(--border);
    border-radius: 6px;
  }

  .exp-header {
    display: flex;
    justify-content: space-between;
    align-items: baseline;
    margin-bottom: 4px;
  }

  .exp-company {
    font-weight: 600;
    font-size: 13.5px;
    color: var(--text);
  }

  .exp-role {
    font-size: 12.5px;
    color: var(--accent);
    font-weight: 500;
    margin-left: 8px;
  }

  .exp-date {
    font-size: 12px;
    color: var(--text-light);
    font-family: 'JetBrains Mono', monospace;
  }

  .exp-details {
    font-size: 12.5px;
    color: var(--text-muted);
    line-height: 1.6;
  }

  /* Awards */
  .award-item {
    display: flex;
    justify-content: space-between;
    align-items: baseline;
    padding: 4px 0;
    border-bottom: 0.5px solid var(--border);
    font-size: 12.5px;
  }

  .award-item:last-child {
    border-bottom: none;
  }

  .award-name { color: var(--text); }

  .award-date {
    color: var(--text-light);
    font-size: 12px;
    font-family: 'JetBrains Mono', monospace;
  }

  /* Tags */
  .tags {
    display: flex;
    flex-wrap: wrap;
    gap: 6px;
  }

  .tag {
    font-size: 12px;
    padding: 3px 10px;
    border-radius: 20px;
    background: var(--tag-bg);
    color: var(--tag-text);
    font-weight: 500;
  }

  .tag-accent {
    background: var(--accent-light);
    color: var(--accent);
  }

  /* Print hint */
  .print-hint {
    position: fixed;
    bottom: 0;
    left: 0;
    right: 0;
    background: var(--primary);
    color: white;
    text-align: center;
    padding: 10px 20px;
    font-size: 13px;
    z-index: 999;
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 16px;
  }

  .print-hint button {
    background: var(--accent);
    color: white;
    border: none;
    padding: 6px 20px;
    border-radius: 4px;
    font-size: 13px;
    cursor: pointer;
  }

  .print-hint .close-hint {
    background: transparent;
    border: 0.5px solid rgba(255,255,255,0.4);
    padding: 6px 14px;
  }

  @media (max-width: 640px) {
    .page { padding: 20px 16px; }
    .header { flex-direction: column; gap: 10px; }
    .header-right { text-align: left; }
    .summary-bar { flex-direction: column; gap: 6px; }
    .divider { display: none; }
    .edu-grid { grid-template-columns: 1fr; }
    .exp-header { flex-direction: column; }
  }
</style>
</head>
<body>
<div class="page">

  <div class="header">
    <div class="header-left">
      <h1>李孙博闻</h1>
      <div class="cn-name">Sunbowen Lee</div>
    </div>
    <div class="header-right">
      <div class="contact-item">
        <svg class="contact-icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"/><polyline points="22,6 12,13 2,6"/></svg>
        <a href="mailto:bw1863@outlook.com">bw1863@outlook.com</a>
      </div>
      <div class="contact-item">
        <svg class="contact-icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M22 16.92v3a2 2 0 01-2.18 2 19.79 19.79 0 01-8.63-3.07 19.5 19.5 0 01-6-6 19.79 19.79 0 01-3.07-8.67A2 2 0 014.11 2h3a2 2 0 012 1.72 12.84 12.84 0 00.7 2.81 2 2 0 01-.45 2.11L8.09 9.91a16 16 0 006 6l1.27-1.27a2 2 0 012.11-.45 12.84 12.84 0 002.81.7A2 2 0 0122 16.92z"/></svg>
        (+86) 17386126551 &middot; 微信 L14561
      </div>
      <div class="contact-item">
        <svg class="contact-icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0118 0z"/><circle cx="12" cy="10" r="3"/></svg>
        北京·海淀
      </div>
      <div class="contact-item" style="margin-top:3px;">
        <a href="https://bowen1911.github.io/" target="_blank">个人主页</a>
        &middot;
        <a href="https://github.com/bowen1911" target="_blank">GitHub (300+ ★)</a>
        &middot;
        <a href="https://scholar.google.cz/citations?user=MplgzoIAAAAJ&hl=zh-CN" target="_blank">Scholar</a>
        &middot;
        <a href="https://orcid.org/0009-0004-9288-2799" target="_blank">ORCID</a>
      </div>
    </div>
  </div>

  <div class="summary-bar">
    <div class="summary-item">
      <span class="summary-label">成果</span>
      <span class="summary-value">10 篇论文 (5 一作 + 5 合作)</span>
    </div>
    <div class="divider"></div>
    <div class="summary-item">
      <span class="summary-label">顶会</span>
      <span class="summary-value">ACL 2025, ICML 2026, AAMAS 2025</span>
    </div>
    <div class="divider"></div>
    <div class="summary-item">
      <span class="summary-label">英语</span>
      <span class="summary-value">CET-6 516</span>
    </div>
  </div>

  <div class="section">
    <div class="section-title">研究方向</div>
    <div class="tags">
      <span class="tag tag-accent">基模后训练</span>
      <span class="tag tag-accent">大语言模型</span>
      <span class="tag tag-accent">模型蒸馏</span>
      <span class="tag tag-accent">AI 安全</span>
      <span class="tag">可解释性</span>
      <span class="tag">强化学习</span>
      <span class="tag">高效推理</span>
      <span class="tag">AI 音频</span>
    </div>
  </div>

  <div class="section">
    <div class="section-title">教育背景</div>
    <div class="edu-grid">
      <div>
        <div class="edu-degree">博士，计算机科学与技术</div>
        <div class="edu-school">北京理工大学，计算机学院</div>
        <div class="edu-date">2026.9 – 2030.6</div>
      </div>
      <div>
        <div class="edu-degree">硕士，系统科学</div>
        <div class="edu-school">武汉科技大学，理学院</div>
        <div class="edu-date">2023.9 – 2026.6</div>
      </div>
      <div>
        <div class="edu-degree">学士，金融学</div>
        <div class="edu-school">湖北经济学院，金融学院</div>
        <div class="edu-date">2018.9 – 2022.6</div>
      </div>
    </div>
  </div>

  <div class="section">
    <div class="section-title">发表论文</div>

    <div class="pub-category">
      <div class="pub-category-title">一作论文</div>

      <div class="pub-item">
        <div class="pub-title">
          <a href="https://aclanthology.org/2025.acl-long.248/" target="_blank">Quantification of Large Language Model Distillation</a>
        </div>
        <div class="pub-meta">
          <span class="pub-venue venue-a">ACL 2025 (CCF-A)</span>
          <b>Sunbowen Lee</b>, Junting Zhou, Chang Ao, Kaige Li, Xeron Du, Sirui He, Haihong Wu, Tianci Liu, Jiaheng Liu, Hamid Alinejad-Rokny, et al.
        </div>
      </div>

      <div class="pub-item">
        <div class="pub-title">
          <a href="https://arxiv.org/abs/2510.05969" target="_blank">Probing the Difficulty Perception Mechanism of Large Language Models</a>
        </div>
        <div class="pub-meta">
          <span class="pub-venue venue-preprint">预印本</span>
          <b>Sunbowen Lee</b>, Qingyu Yin, Chak Tou Leong, Jialiang Zhang, Yicheng Gong, Shiwen Ni, Min Yang, Xiaoyu Shen
        </div>
      </div>

      <div class="pub-item">
        <div class="pub-title">
          <a href="https://arxiv.org/abs/2501.16727" target="_blank">xJailbreak: Representation Space Guided Reinforcement Learning for Interpretable LLM Jailbreaking</a>
        </div>
        <div class="pub-meta">
          <span class="pub-venue venue-preprint">预印本</span>
          <b>Sunbowen Lee</b>, Shiwen Ni, Chi Wei, Shuaimin Li, Liyang Fan, Ahmadreza Argha, Hamid Alinejad-Rokny, Ruifeng Xu, Yicheng Gong, Min Yang
        </div>
      </div>

      <div class="pub-item">
        <div class="pub-title">
          <a href="https://www.sciencedirect.com/science/article/abs/pii/S0925231225006897" target="_blank">Counterfactual Experience Augmented Off-Policy Reinforcement Learning</a>
        </div>
        <div class="pub-meta">
          <span class="pub-venue venue-sci">Neurocomputing (SCI-2)</span>
          <b>Sunbowen Lee</b>, Yicheng Gong, Chao Deng
        </div>
      </div>

      <div class="pub-item">
        <div class="pub-title">
          <a href="https://dl.acm.org/doi/10.5555/3709347.3743758" target="_blank">MacLight: Multi-scene Aggregation Convolutional Learning for Traffic Signal Control</a>
        </div>
        <div class="pub-meta">
          <span class="pub-venue venue-b">AAMAS 2025 (CCF-B)</span>
          <b>Sunbowen Lee</b>, Hongqin Lyu, Yicheng Gong, Yingying Sun, Chao Deng
        </div>
      </div>
    </div>

    <div class="pub-category">
      <div class="pub-category-title">合作论文</div>

      <div class="pub-item">
        <div class="pub-title">
          <a href="https://arxiv.org/abs/2601.13752" target="_blank">Finding RELIEF: Shaping Reasoning Behavior without Reasoning Supervision via Belief Engineering</a>
        </div>
        <div class="pub-meta">
          <span class="pub-venue venue-findings">ACL Findings 2026 (CCF-A)</span>
          Chak Tou Leong, Dingwei Chen, Heming Xia, Qingyu Yin, <b>Sunbowen Lee</b>, Jian Wang, Wenjie Li
        </div>
      </div>

      <div class="pub-item">
        <div class="pub-title">
          <a href="https://arxiv.org/abs/2512.23165v2" target="_blank">Evaluating Parameter Efficient Methods for RLVR</a>
        </div>
        <div class="pub-meta">
          <span class="pub-venue venue-a">ICML 2026 (CCF-A)</span>
          Qingyu Yin, Yulun Wu, Zhennan Shen, <b>Sunbowen Lee</b>, Zhilin Wang, Yanshu Li, Chak Tou Leong, Jiale Kang, Jinjin Gu
        </div>
      </div>

      <div class="pub-item">
        <div class="pub-title">
          <a href="https://arxiv.org/abs/2407.10953" target="_blank">MMM: Multilingual Mutual Reinforcement Effect Mix Datasets & Test with Open-domain Information Extraction Large Language Models</a>
        </div>
        <div class="pub-meta">
          <span class="pub-venue venue-findings">ACL Findings 2026 (CCF-A)</span>
          Chengguang Gan, <b>Sunbowen Lee</b>, Qingyu Yin, Yunhao Liang, Xinyang He, Hanjun Wei, Younghun Lim, Shijian Wang, Hexiang Huang, Qinghao Zhang, Shiwen Ni, Tatsunori Mori
        </div>
      </div>

      <div class="pub-item">
        <div class="pub-title">
          <a href="https://arxiv.org/abs/2509.11976" target="_blank">PoolingVQ: A VQVAE Variant for Reducing Audio Redundancy and Boosting Multi-Modal Fusion in Music Emotion Analysis</a>
        </div>
        <div class="pub-meta">
          <span class="pub-venue venue-preprint">预印本</span>
          Dinghao Zou, Yicheng Gong, Xiaokang Li, Xin Cao, <b>Sunbowen Lee</b>
        </div>
      </div>

      <div class="pub-item">
        <div class="pub-title">
          <a href="https://arxiv.org/abs/2509.10781" target="_blank">EmoAnti: Audio Anti-Deepfake with Refined Emotion-Guided Representations</a>
        </div>
        <div class="pub-meta">
          <span class="pub-venue venue-preprint">预印本</span>
          Xiaokang Li, Yicheng Gong, Dinghao Zou, Xin Cao, <b>Sunbowen Lee</b>
        </div>
      </div>
    </div>
  </div>

  <div class="section">
    <div class="section-title">实习与项目经历</div>

    <div class="exp-item">
      <div class="exp-header">
        <div>
          <span class="exp-company">腾讯</span>
          <span class="exp-role">应用研究实习</span>
        </div>
        <span class="exp-date">2026.4 – 至今</span>
      </div>
      <div class="exp-details">微信基础大语言模型后训练研发。</div>
    </div>

    <div class="exp-item">
      <div class="exp-header">
        <div>
          <span class="exp-company">宁波东方理工高等研究院</span>
          <span class="exp-role">大模型科研实习</span>
        </div>
        <span class="exp-date">2025.9 – 2025.11</span>
      </div>
      <div class="exp-details">沈晓宇老师团队，研究 LLMs 可解释性，产出论文一篇。</div>
    </div>

    <div class="exp-item">
      <div class="exp-header">
        <div>
          <span class="exp-company">共道网络科技有限公司</span>
          <span class="exp-role">大模型算法实习</span>
        </div>
        <span class="exp-date">2025.4 – 2025.9</span>
      </div>
      <div class="exp-details">口语文本表征可解释性研究；构建音频数据自动筛选管道及 TTS 异常检测；优化 BGE 嵌入模型召回与微调管道，模型蒸馏工程实现。</div>
    </div>

    <div class="exp-item">
      <div class="exp-header">
        <div>
          <span class="exp-company">中科院深圳先进技术研究院 / 深圳理工大学</span>
          <span class="exp-role">科研实习</span>
        </div>
        <span class="exp-date">2024.9 – 2025.4</span>
      </div>
      <div class="exp-details">杨敏、倪仕文老师团队，研究大语言模型安全性与蒸馏检测，产出 ACL 2025 主会论文一篇、越狱攻击论文一篇。</div>
    </div>

    <div class="exp-item">
      <div class="exp-header">
        <div>
          <span class="exp-company">武汉海云健康科技股份有限公司</span>
          <span class="exp-role">数据挖掘项目</span>
        </div>
        <span class="exp-date">2024.2 – 2024.6</span>
      </div>
      <div class="exp-details">负责大数据分析与处理，主要完成数据清洗及特征工程构建。</div>
    </div>

    <div class="exp-item">
      <div class="exp-header">
        <div>
          <span class="exp-company">北京金信网银金融信息服务有限公司</span>
          <span class="exp-role">数据标注实习</span>
        </div>
        <span class="exp-date">2021.2 – 2021.6</span>
      </div>
      <div class="exp-details">基于词袋模型完成文本数据打标工作并实现脚本自动化。</div>
    </div>
  </div>

  <div class="section">
    <div class="section-title">竞赛获奖</div>
    <div class="award-item">
      <span class="award-name">一等学业奖学金 (连续三年: 2023, 2024, 2025)</span>
      <span class="award-date">2023 – 2025</span>
    </div>
    <div class="award-item">
      <span class="award-name">全国数学建模竞赛，湖北省一等奖 (负责完成研究代码与实验)</span>
      <span class="award-date">2020.11</span>
    </div>
    <div class="award-item">
      <span class="award-name">全国统计建模竞赛，湖北省三等奖 (负责完成代码与模型构建)</span>
      <span class="award-date">2024.6</span>
    </div>
  </div>

</div>

<div class="print-hint" id="printHint">
  <span>打印提示：请在打印设置中取消勾选「页眉和页脚」以去除页码</span>
  <button onclick="window.print()">打印</button>
  <button class="close-hint" onclick="document.getElementById('printHint').style.display='none'">关闭</button>
</div>

</body>
</html>
