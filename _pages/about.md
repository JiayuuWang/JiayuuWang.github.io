---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>

<strong>
I'm a third-year Computer Science student at the College of Computer Science and Technology, Xi'an Jiaotong University, expected to earn my B.S. in Engineering in fall 2027. My research interests primarily focus on Large Language Model (LLM) Agents in Domain-specific Scenarios, and Autonomous Agents in Computer Use (CLI, GUI). Contact me at jiayuw794@gmail.com.
</strong>

# 🔥 News
- *2026.01.05*: &nbsp;🎉🎉 I attend the semi-final competition of AI Agent 2025([Link](https://www.aiagent2025.com/)) held by ([Chinese Association for Artificial Intelligence](https://www.aiagent2025.com/))(CAAI) in Shenzhen, China!
- *2025.12.01*: &nbsp;🎉🎉 I get the merit award(￥1500) working with my teammates [zepeng](https://github.com/xcarl1) and [weijiang](https://github.com/Johanson-colab) in Harmony System Control Agent Competition([Link](https://developer.huaweicloud.com/competition/information/1300000181/introduction)) held by Nanjing University and Huawei!
- *2025.11.30*: &nbsp;🎉🎉 The number of subscribers of the Account has reached 500!
- *2025.11.22*: &nbsp;🎉🎉 GeoPlan-bench Releases!
- *2025.11.04*: &nbsp;🎉🎉 Earth-Insights WeChat Official Account's Paper-Deep-Dive Feature Releases!
- *2025.10.28*: &nbsp;🎉🎉 I attend "Vibe Coding hackthon" held by WaytoAGI([Link](https://www.waytoagi.com/)) and give a talk on GUI-Agents and their potential in the future!
- *2025.10.21*: &nbsp;🎉🎉 Auto-Cursor Releases!
- *2025.10.21*: &nbsp;🎉🎉 Earth-Insights Account has started cross-posting on RedNote!
- *2025.10.03*: &nbsp;🎉🎉 Earth-Insights WeChat Official Account's first Semi-Weekly-Report Release!
- *2025.09.20*: &nbsp;🎉🎉 I attend Cursor Meetup Xi'an!
- *2025.09.15*: &nbsp;🎉🎉 EarthAgent succeeds in MVP test by AI Agent 2025 Committee!
- *2025.08.24*: &nbsp;🎉🎉 I participate in the "First National College Student Artificial Intelligence Security Competition" ([Link](https://scss.bupt.edu.cn/info/1055/6018.htm)) held at Beijing University of Posts and Telecommunications and win the first prize!


# 📝 Publications 

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">CVPR 2026 (submitted)</div><img src='images/2511.17198v1_01.png' alt="sym" width="80%"></div></div>
<div class='paper-box-text' markdown="1">

**Designing Domain-Specific Agents via Hierarchical Task Abstraction Mechanism**

[Paper](https://arxiv.org/abs/2511.17198) | [Code](https://github.com/earth-insights/GeoPlan-bench) | [Project](https://earth-insights.github.io/EarthAgent/)

Kaiyu Li, **Jiayu Wang**, Zhi Wang, Hui Qiao, Weizhan Zhang, Deyu Meng, Xiangyong Cao
- We introduce a novel agent design framework centered on a Hierarchical Task Abstraction Mechanism (HTAM). 
- We instantiate this framework as EarthAgent, a multi-agent system tailored for complex geospatial analysis. To evaluate such complex planning capabilities, we build GeoPlan-bench, a comprehensive benchmark of realistic, multi-step geospatial planning tasks. It is accompanied by a suite of carefully designed metrics to evaluate tool selection, path similarity, and logical completeness. 
- Experiments show that EarthAgent substantially outperforms a range of established single- and multi-agent systems.

</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">TPAMI (submitted)</div><img src='images/2509.25654v1_01.png' alt="sym" width="80%"></div></div>
<div class='paper-box-text' markdown="1">

**DescribeEarth: Describe Anything for Remote Sensing Images**

[Paper](https://arxiv.org/abs/2509.25654) | [Code](https://github.com/earth-insights/DescribeEarth) | [Dataset](https://huggingface.co/datasets/earth-insights/DE-Dataset) | [Benchmark](https://huggingface.co/datasets/earth-insights/DE-Benchmark)

Kaiyu Li, Zixuan Jiang, Xiangyong Cao, **Jiayu Wang**, Yuchen Xiao, Deyu Meng, Zhi Wang
- We propose Geo-DLC, a novel task of object-level fine-grained image captioning for remote sensing.
- We construct DE-Dataset, a large-scale dataset containing 25 categories and 261,806 annotated instances with detailed descriptions of object attributes, relationships, and contexts. 
- Furthermore, we introduce DE-Benchmark, an LLM-assisted question-answering based evaluation suite designed to systematically measure model capabilities on the Geo-DLC task.
- We also present DescribeEarth, a Multi-modal Large Language Model (MLLM) architecture explicitly designed for Geo-DLC. 
- Our DescribeEarth model consistently outperforms state-of-the-art general MLLMs on DE-Benchmark, demonstrating superior factual accuracy, descriptive richness, and grammatical soundness, particularly in capturing intrinsic object features and surrounding environmental attributes across simple, complex, and even out-of-distribution remote sensing scenarios. 

</div>
</div>


<span class='anchor' id='-projects'></span>

# 🚀 Projects (selected)
<div markdown="1"> 
## 🔥**Auto-Cursor** ([link](https://github.com/JiayuuWang/Auto-Cursor)) (Oct 2025) 
Auto-Cursor is **THE FIRST** (to the best of my knowledge) GUI-native orchestration layer that pilots the Cursor IDE like a human operator. By combining large language models, visual grounding, and deterministic automation, the project explores how agents can build software without being confined to command-line tooling.


### Why Through GUI?
1. **Human-parity reach**: Command-line automation is capped by the APIs that tools expose. A GUI agent, however, can click, type, drag, and navigate any surface that a human can. This dramatically widens the solution space—if a person can operate it, an agent can learn to operate it too, opening the door to automating entire product lifecycles.
2. **Grounded perception is ready**: Domain-specific MLLMs now recognize icons, layouts, and context with far higher reliability. The bottleneck has shifted from perception to orchestration. Auto-Cursor focuses on that orchestration layer—sequencing vision, language, and action—to unlock richer, end-to-end workflows.
3. **Standing on the shoulders of the ecosystem**: GUI-first control leverages advances in agents, LLMs, GPU-accelerated rendering, and even display hardware. We treat the modern desktop as a programmable environment, turning existing tools into improvable building blocks instead of rewriting them.

### Vision
1. **Build a resilient, self-improving system** that can iterate on its own behaviors, learn from failures, and adapt to different project constraints.
2. **Provide tangible GUI agent scenarios** that inspire new ideas for downstream industries—design, ops, education, assistive tech, and beyond.
3. **Stimulate thinking on AI safety and software design**, showing how oversight, logging, and guardrails can coexist with highly capable automation.
</div>
<iframe src="https://player.bilibili.com/player.html?bvid=BV1weUvBoExk&page=1&high_quality=1&danmaku=0" width="70%" height="500" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"></iframe>
<div markdown="1"> 
## 🔥**EarthAgent** ([link](https://www.aiagent2025.com/projects/buq2zyaq05w2)) (July 2025) 


EarthAgent is a groundbreaking general AI agent for the remote sensing field, dedicated to making complex and high-threshold geospatial analysis more accessible and automated. It allows users to drive a fully automated workflow that integrates multimodal data acquisition, intelligent interpretation, and deep reasoning through simple natural language conversations. Whether with text or image inputs, EarthAgent can autonomously plan and execute tasks, reducing traditional manual analysis processes that used to take days to just minutes. It has attracted <span style="color:blue">**300+**</span> likes on RedNote. [link](https://www.xiaohongshu.com/explore/68d2b443000000001400bd21?xsec_token=YBz1lxaWzYRLK2xD2jWcZICLY7PQLbdt5qfafsk5X2LbM%3D&xsec_source=pc_creatormng)
</div>
<iframe src="https://player.bilibili.com/player.html?bvid=BV1PaUvBFE7A&page=1&high_quality=1&danmaku=0" width="70%" height="500"  scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"></iframe>
<div markdown="1"> 
## 🔥**Earth-Insights WeChat Official Account Agent (地球洞察微信公众号)** (Oct 2025)
This is an **automated system** that fetches the latest papers in the fields of remote sensing and deep learning. Through sophisticated design and arrangement, it utilizes document analysis agents and various document analysis tools to achieve fully automated analysis and summarization. Currently, it consists of two modules: the Semi-Weekly Report and the Paper Deep Dive. As of December 16, the official account has published a total of <span style="color:blue">**60+**</span> blogs, covering <span style="color:blue">**240+**</span> papers, accumulating over <span style="color:blue">**4,000**</span> reads, and attracting more than <span style="color:blue">**500**</span> followers, providing the community with convenient access to the latest information.
<img src='images/wechat-public-account.png' alt="sym" width="80%">
- Semi-Weekly Report Demo: [link](https://mp.weixin.qq.com/s/iNYby5U9HvpnGki1JaaV7w)
- Paper Deep Dive Demo: [link](https://mp.weixin.qq.com/s/6B67lV7Se1zRXL7kl1sWqw) 
</div>