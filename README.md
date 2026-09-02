<div align="center">

# 张家宁 | Zhang Jianing

<img src="./微信图片_20260609135726_251_39.jpg" width="180" style="border-radius: 50%;" alt="Zhang Jianing">

**中国科学技术大学** 信息与通信工程 硕士在读  
University of Science and Technology of China · Master Student

[![Email](https://img.shields.io/badge/Email-zhangjianing@mail.ustc.edu.cn-D14836?style=flat&logo=gmail&logoColor=white)](mailto:zhangjianing@mail.ustc.edu.cn)
![Profile Views](https://komarev.com/ghpvc/?username=zjn20021020&label=Profile%20views&color=0e75b6&style=flat)

[**🇨🇳 中文**](#) | [**🇬🇧 English**](./README_EN.md)

</div>

---

## 👤 关于我

我专注于 **Agent Harness 与 AI Agent 工程**，关注 Agent Loop、Tool Use、Skills、Memory、Context Engineering，以及真实任务中的可靠性与可观测性。

目前在科大讯飞担任 AI 研发工程师实习生（Agent Harness 方向），参与桌面 Agent 产品、Agent 内核与端云协同能力的研发和版本交付。

同时在读研期间从事磁共振序列开发工作，在医学影像领域积累了一定的研究经验。

**兴趣方向**：Agent Harness · AI Agent · Tool Use · Context Engineering · Multi-Agent · LLM 系统工程

---

## 🎓 教育背景

**硕士** | 中国科学技术大学  
信息与通信工程 | 2025 - 2028届

**本科** | 武汉大学  
电子信息工程 | 2021 - 2025  
- GPA 排名：**5/133**
- 综合测评排名：**2/133**
- 🏆 **国家奖学金获得者** (2023)

---

## 💼 实习经历

**科大讯飞** | AI 研发工程师实习生（Agent Harness 方向）  
_2026.06 - 至今_

- 持续参与 **AstronStudio、Acode、AstronClaw** 的开发与版本交付，覆盖桌面 Agent Harness、Rust Agent 内核与端云协同链路
- 参与 AstronStudio 多 Provider Harness 的会话生命周期、流式事件与能力建模；其渠道能力通过 Astron Connect 接入飞书、微信并映射到本地 Agent 会话
- 负责 Acode Agent 生命周期日志埋点，覆盖 Turn、Tool、MCP、Skills、Subagent、Plugin、上下文压缩与 Token 用量
- 开发 Agent 可观测大盘与 Elastic 自动查询能力，将真实任务中的失败链路反馈到模型与 Harness 联调、Bug 修复及回归测试

---

**OPPO 公司** | 语音算法开发工程师  
_2024.10 - 2025.1_

- 负责语音通话中多场景降噪算法的开发与优化
- 算法已实装于 **OPPO OnePlus 14** 及后续机型
- 涉及技术：语音信号处理、降噪算法、实时音频处理

---

## 🚀 项目经历

### 🤖 AI Agent 与应用开发

#### [solo-leveling](https://github.com/zjn20021020/solo-leveling)
**我独自升级 - 从对话摩擦中自我进化的 OpenClaw 插件**

基于 **Human-in-the-Loop** 的自适应学习系统，通过捕获用户纠正与负面情绪实现持续知识蒸馏：

- 🔍 **Friction Detection** - 双维度扫描：纠错次数 + 情感强度（calm/annoyed/agitated/hostile）
- 🧠 **Knowledge Distillation** - 三模式决策（skip/new/revise），将对话摩擦转化为可复用 Skill
- 📚 **Index-Based Registry** - index.json 单一事实源 + O(1) 检索，无需扫描目录
- ⚡ **Atomic Write Protocol** - Staging → Validation → Rename，写失败零污染
- 🔄 **Retrospective Mechanism** - 会话首轮注入 recap，展示新学 Skill 摘要

**核心架构**：Two-Phase Pipeline (Friction Scan → Lesson Distillation) · Budget-Greedy Transcript · Bracket-Depth JSON Carving

**技术栈**：`TypeScript` `OpenClaw Plugin SDK` `Zod` `Prompt Engineering` `Meta-Learning`

---

#### [PaperAgent](https://github.com/zjn20021020/PaperAgent)
**端到端学术论文自动生成 - 基于 LangGraph 的多智能体协作框架**

从零完成完整科研流程：论文检索 → 灵感提取 → 方案设计 → 实验设计 → 逐章撰写 → 多轮审稿优化

- 📄 **Multi-Agent Workflow** - LangGraph 状态机：14 个核心节点 + 条件分支 + 双循环机制
- 🔎 **Section Pipeline** - 架构设计 → 派发章节 → 写作 → 校验 → 重写（最多 3 次）→ 保存
- 💡 **Review Iteration Loop** - 改稿 → 润色 → 去 AI 味 → 审稿 → 返回改稿（最多 3 轮）
- ✍️ **Conditional Branching** - 章节校验分支 + 审稿迭代分支
- 📊 **Conference Templates** - NeurIPS / ICML / ICLR / ACL / CVPR / AAAI

**核心技术**：State Machine Architecture · Quality Control System (章节级 + 论文级) · arXiv Integration

**技术栈**：`Python` `LangGraph` `LangChain` `OpenAI API` `Anthropic API` `LaTeX`

---

#### [Pi_based-knowledge-agent](https://github.com/zjn20021020/Pi_based-knowledge-agent)
**Paper Knowledge Agent - 基于 Pi Agent 框架的对话式论文库管家**

构建在 Pi Agent 之上的终端 AI 助手，实现多主题论文库的自动化管理与段落级语义检索

- 🏗️ **Pi Framework Integration** - 复用 InteractiveMode(TUI) + SessionManager + ModelRegistry + Tool Dispatcher
- 🗂️ **Multi-Collection Management** - 智能路由（下载归属判断 / 检索库选择）
- 📥 **arXiv Crawler** - 批量下载 PDF + 限流策略（每篇 3s 间隔）
- 📑 **Section-Level Chunking** - 识别 20+ 学术章节关键词 + ~300 token 切分 + 章节定位
- 💾 **Zero External Services** - SQLite(sql.js) + JSON 向量库 + 本地 PDF
- 🔄 **Embedding Fallback** - OpenAI text-embedding-3-small (1536维) → TF-IDF 自动降级

**架构特点**：15 个 Custom Tools Injection · Hybrid Embedding (OpenAI + TF-IDF 双后端)

**技术栈**：`TypeScript` `Node.js` `Pi Agent Framework` `sql.js` `pdf-parse` `OpenAI Embedding` `TF-IDF`

---

#### [ScholarLife-Agent](https://github.com/zjn20021020/ScholarLife-Agent)
**面向学生与科研工作者的多场景 AI 助手**

基于 Workflow Orchestration 的多 Agent 协同系统：论文检索 · 写作润色 · 审稿模拟 · 工作流自动化

**技术栈**：`Dify` `LLM` `Multi-Agent System` `Workflow Orchestration` `Tool Use`

---

### 🤖 嵌入式智能系统

#### [bbcar](https://github.com/zjn20021020/bbcar)
**基于 STM32G474 的麦克纳姆轮全向机器人小车**

IMU 姿态解算 + 编码器轮速反馈 · PID 闭环控制 · 红外循迹 · 多传感器融合

**技术栈**：`STM32` `C` `Keil` `PID Control` `Sensor Fusion`

---

#### FPGA 体感贪吃蛇 [[📹 演示]](https://www.bilibili.com/video/BV1nP411K7T8)
**人体姿态控制的贪吃蛇小游戏**

计算机视觉识别人体姿态 · FPGA 实时交互 · 姿态识别与游戏逻辑结合

**技术栈**：`FPGA` `OpenCV` `Computer Vision`

---

### 🤝 协作项目

#### [henryzhuhr/deep-lane-detection](https://github.com/henryzhuhr/deep-lane-detection)
**基于深度学习的车道线检测**

深度学习车道线检测 · TensorRT 部署 Jetson Nano · 小车循迹

**技术栈**：`PyTorch` `TensorRT` `Jetson Nano` `Computer Vision`

---

## 📝 研究成果

### 会议论文

**Achieving Vendor-Agnostic Perfusion Imaging with PCASL using the Pulseq Framework**  
**Zhang, Jianing**, Wang, Jun, Li, Hongwei, Ye, Shaoyou, Okell, Thomas, Li, Xiaohu, Ji, Yang  
_ISMRM-ISMRT Annual Meeting & Exhibition_, Cape Town, South Africa, May 2026  
Program Number: 661-01-011 | [查看摘要](http://echo.ismrm.org/abstracts/view/773ce267-4fd2-4b8b-b367-eec6be612400)

> 💡 独立完成 **GE / Siemens / Philips / 联影** 多厂商通用磁共振成像方案  
> 📄 已拓展为期刊论文投递 **_Magnetic Resonance in Medicine_**，**under review**

### 专利

基于脑电信号的情感分析系统 | 申请号：CN202311089224.X

---

## 🏆 荣誉与竞赛

### 荣誉

- 🥇 **国家奖学金** (2023)
- 🏅 **毕马威专项奖学金** (2022)
- 📚 **甲等奖学金** (2022, 2023, 2024)

### 竞赛

- 🥈 **全国大学生光电设计竞赛 二等奖** (2023) | 迷宫寻宝小车 [[📹]](https://www.bilibili.com/video/BV1cN411z7co)
- 🥇 **全国大学生电子设计大赛 省级一等奖** (2023) | F 题：基于声传播的智能定位系统
- 🏆 **湖北省电子设计竞赛 特等奖** (2022) | C 题：小车跟随行驶系统 [[📹]](https://www.bilibili.com/video/BV1JB4y1t7NL)

---

## 🛠️ 技术栈

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=flat&logo=rust&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=flat&logo=go&logoColor=white)
![C](https://img.shields.io/badge/C-00599C?style=flat&logo=c&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat&logo=cplusplus&logoColor=white)
![MATLAB](https://img.shields.io/badge/MATLAB-0076A8?style=flat&logo=mathworks&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat&logo=pytorch&logoColor=white)
![STM32](https://img.shields.io/badge/STM32-03234B?style=flat&logo=stmicroelectronics&logoColor=white)
![FPGA](https://img.shields.io/badge/FPGA-FF6F00?style=flat&logo=xilinx&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)

**关键词**：`Agent Harness` · `Agent Loop` · `Tool Use` · `Skills` · `MCP` · `Memory` · `Subagent` · `Multi-Agent` · `Context Engineering` · `LangGraph` · `RAG` · `WebSocket` · `Observability`

---

## 📫 联系方式

- 📧 邮箱：zhangjianing@mail.ustc.edu.cn
- 💬 欢迎交流：Agent Harness、AI Agent、LLM 系统工程

---

## 📊 GitHub 统计

<div align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=zjn20021020&show_icons=true&hide_border=true&count_private=true&theme=default" alt="GitHub stats">
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=zjn20021020&layout=compact&hide_border=true&langs_count=8" alt="Top languages">
</div>

---

<div align="center">
  <sub>🤝 欢迎交流合作</sub>
</div>
