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

我热爱 **Agent 开发**，包括 **AI Agent** 和**嵌入式智能系统**的设计与实现。

同时在读研期间从事磁共振序列开发工作，在医学影像领域积累了一定的研究经验。

**兴趣方向**：AI Agent 开发 · 嵌入式智能系统 · LLM 应用 · 磁共振序列设计

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

**OPPO 公司** | 语音算法开发工程师  
_2024.10 - 2025.1_

- 负责语音通话中多场景降噪算法的开发与优化
- 算法已实装于 **OPPO OnePlus 14** 及后续机型
- 涉及技术：语音信号处理、降噪算法、实时音频处理

---

## 🚀 项目经历

### 🤖 AI Agent 与应用开发

#### [solo-leveling](https://github.com/zjn20021020/solo-leveling)
**我独自升级 - 自我进化的 OpenClaw 插件**

基于 **Reflection** 机制的自适应学习系统，通过 **Human Feedback Loop** 实现持续优化：

- 🔍 **Friction Detection** - 实时监测用户纠正与情感信号（Sentiment Analysis）
- 🧠 **Knowledge Distillation** - 将交互摩擦蒸馏为可复用 Skill（Meta-Learning）
- 📚 **Skill Registry** - 索引派架构，O(1) 技能检索与版本管理
- ⚡ **Atomic Write** - Staging + Rename 原子操作，零风险技能更新
- 🔄 **Retrospective Loop** - 会话级回顾机制，增量式知识积累

**核心技术**：
- **Two-Phase Pipeline**: Friction Scan → Lesson Distillation
- **Budget-Greedy Context**: 预算约束下的贪心上下文采样
- **Bracket-Depth JSON Parsing**: 鲁棒的结构化输出解析

**技术栈**：`TypeScript` `OpenClaw Plugin SDK` `Zod Schema Validation` `Meta-Learning` `RLHF`

---

#### [PaperAgent](https://github.com/zjn20021020/PaperAgent)
**基于 RAG 的学术论文智能助手**

采用 **Retrieval-Augmented Generation** 架构的学术研究辅助系统：

- 📄 **Document Understanding** - 多模态论文解析（PDF/LaTeX）
- 🔎 **Semantic Search** - Vector Database 驱动的语义检索
- 💡 **Citation Network** - 引用关系图谱构建与分析
- ✍️ **Academic Writing** - 基于 Prompt Engineering 的写作辅助
- 📊 **Literature Review** - 自动化文献综述生成

**核心架构**：
- **Embedding Model**: 学术领域微调的向量化模型
- **Chunking Strategy**: 段落级语义分割与上下文保留
- **Reranking**: 多阶段检索优化（Coarse-to-Fine）

**技术栈**：`Python` `LangChain` `ChromaDB/FAISS` `RAG` `Transformer` `Few-Shot Learning`

---

#### [Pi_based-knowledge-agent](https://github.com/zjn20021020/Pi_based-knowledge-agent)
**树莓派边缘部署的知识型 Agent**

面向 **Edge Computing** 的轻量级智能 Agent，实现 **On-Device Inference**：

- 🖥️ **Model Quantization** - INT8/FP16 量化部署
- 🚀 **Inference Optimization** - TensorRT/ONNX Runtime 加速
- 🧠 **Knowledge Graph** - 本地知识图谱与推理引擎
- 💬 **Offline NLU** - 离线自然语言理解模块
- 🔌 **IoT Integration** - 物联网设备协议适配

**系统特性**：
- **Low-Latency**: <100ms 响应时延
- **Privacy-First**: 本地推理，数据不出设备
- **Resource-Aware**: 内存占用 <500MB

**技术栈**：`Raspberry Pi` `TensorFlow Lite` `ONNX` `Knowledge Graph` `Edge AI` `Model Compression`

---

#### [ScholarLife-Agent](https://github.com/zjn20021020/ScholarLife-Agent)
**面向学生与科研工作者的多场景 AI 助手**

基于 **Workflow Orchestration** 构建的多 Agent 协同系统：

- 📚 **Tool Use** - 论文检索与文献管理（Function Calling）
- ✍️ **Style Transfer** - 学术写作润色与 AI 检测规避
- 📝 **Peer Review Simulation** - 模拟审稿人视角的论文评审
- 🔧 **Task Automation** - 科研工作流自动化编排

**技术栈**：`Dify` `LLM` `Multi-Agent System` `Workflow Orchestration` `Tool Use`

---

### 🤖 嵌入式智能系统

#### [bbcar](https://github.com/zjn20021020/bbcar)
**基于 STM32G474 的麦克纳姆轮全向机器人小车**

- IMU 姿态解算 + 编码器轮速反馈
- PID 闭环控制系统
- 红外循迹功能
- 多传感器融合控制

**技术栈**：`STM32` `C` `Keil` `PID Control` `Sensor Fusion`

---

#### FPGA 体感贪吃蛇 [[📹 演示视频]](https://www.bilibili.com/video/BV1nP411K7T8)
**人体姿态控制的贪吃蛇小游戏**

- 通过计算机视觉识别人体姿态
- 部署在 FPGA 上实现实时交互
- 姿态识别与游戏逻辑结合

**技术栈**：`FPGA` `OpenCV` `Computer Vision`

---

### 🤝 协作项目

#### [henryzhuhr/deep-lane-detection](https://github.com/henryzhuhr/deep-lane-detection)
**基于深度学习的车道线检测**

- 将视频中的车道线检测出来
- 使用深度学习方法实现车道线检测
- 训练好的模型使用 TensorRT 部署在 Jetson Nano 上，达到较高推理效率
- 同时根据识别结果完成小车循迹，在不触碰车道线的情况下走完较复杂路段

**技术栈**：`PyTorch` `TensorRT` `Jetson Nano` `Computer Vision`

---

## 📝 研究成果

### 会议论文

**Achieving Vendor-Agnostic Perfusion Imaging with PCASL using the Pulseq Framework**  
**Zhang, Jianing**, Wang, Jun, Li, Hongwei, Ye, Shaoyou, Okell, Thomas, Li, Xiaohu, Ji, Yang  
_ISMRM-ISMRT Annual Meeting & Exhibition_, Cape Town, South Africa, May 2026  
Program Number: 661-01-011 | [查看摘要](http://echo.ismrm.org/abstracts/view/773ce267-4fd2-4b8b-b367-eec6be612400)

> 💡 独立完成了一套包含 **GE / Siemens / Philips / 联影**的多厂商通用磁共振成像实现方案  
> 📄 该工作已拓展为期刊论文并投递至顶刊 **_Magnetic Resonance in Medicine_**，目前 **under review**

### 专利

基于脑电信号的情感分析系统 | 申请号：CN202311089224.X

---

## 🏆 荣誉与竞赛

### 荣誉

- 🥇 **国家奖学金** (2023)
- 🏅 **毕马威专项奖学金** (2022)
- 📚 **甲等奖学金** (2022, 2023, 2024)

### 竞赛

- 🥈 **全国大学生光电设计竞赛 二等奖** (2023)  
  项目：迷宫寻宝小车（基于视觉识别与自主导航）[[📹 演示视频]](https://www.bilibili.com/video/BV1cN411z7co)
  
- 🥇 **全国大学生电子设计大赛 省级一等奖** (2023)  
  F 题：基于声传播的智能定位系统（负责定位算法实现与神经网络部署）
  
- 🏆 **湖北省电子设计竞赛 特等奖** (2022)  
  C 题：小车跟随行驶系统（双车协同、自适应跟随与超车）[[📹 演示视频]](https://www.bilibili.com/video/BV1JB4y1t7NL)

---

## 🛠️ 技术栈

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![C](https://img.shields.io/badge/C-00599C?style=flat&logo=c&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat&logo=cplusplus&logoColor=white)
![MATLAB](https://img.shields.io/badge/MATLAB-0076A8?style=flat&logo=mathworks&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat&logo=pytorch&logoColor=white)
![STM32](https://img.shields.io/badge/STM32-03234B?style=flat&logo=stmicroelectronics&logoColor=white)
![FPGA](https://img.shields.io/badge/FPGA-FF6F00?style=flat&logo=xilinx&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)

**关键词**：`AI Agent` · `RAG` · `Meta-Learning` · `Edge AI` · `Embedded Systems` · `LLM Applications` · `Knowledge Graph` · `RLHF` · `Multi-Agent System`

---

## 📫 联系方式

- 📧 邮箱：zhangjianing@mail.ustc.edu.cn
- 💬 欢迎交流：AI Agent 开发、嵌入式系统、LLM 应用

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
