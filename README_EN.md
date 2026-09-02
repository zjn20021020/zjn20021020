<div align="center">

# Zhang Jianing | 张家宁

<img src="./微信图片_20260609135726_251_39.jpg" width="180" style="border-radius: 50%;" alt="Zhang Jianing">

**University of Science and Technology of China** · Master Student  
中国科学技术大学 信息与通信工程 硕士在读

[![Email](https://img.shields.io/badge/Email-zhangjianing@mail.ustc.edu.cn-D14836?style=flat&logo=gmail&logoColor=white)](mailto:zhangjianing@mail.ustc.edu.cn)
![Profile Views](https://komarev.com/ghpvc/?username=zjn20021020&label=Profile%20views&color=0e75b6&style=flat)

[**🇨🇳 中文**](./README.md) | [**🇬🇧 English**](#)

</div>

---

## 👤 About Me

I focus on **Agent Harness and AI Agent engineering**, including agent loops, tool use, skills, memory, context engineering, reliability, and observability in real-world tasks.

I am currently an AI R&D Engineer Intern at iFLYTEK, working on desktop agent products, agent runtimes, and cloud-device collaboration.

During my graduate studies, I also work on MRI pulse sequence development and have accumulated research experience in medical imaging.

**Interests**: Agent Harness · AI Agent · Tool Use · Context Engineering · Multi-Agent · LLM Systems

---

## 🎓 Education

**Master of Engineering** | University of Science and Technology of China (USTC)  
Information and Communication Engineering | 2025 - 2028

**Bachelor of Engineering** | Wuhan University  
Electronic Information Engineering | 2021 - 2025  
- GPA Rank: **5/133**
- Comprehensive Rank: **2/133**
- 🏆 **National Scholarship Recipient** (2023)

---

## 💼 Work Experience

**iFLYTEK** | AI R&D Engineer Intern, Agent Harness  
_Jun 2026 - Present_

- Contribute to the development and release delivery of **AstronStudio, Acode, and AstronClaw**, spanning a desktop agent harness, a Rust agent runtime, and cloud-device collaboration
- Work on AstronStudio's multi-provider session lifecycle, streaming event model, and capabilities; its Astron Connect channel module bridges Feishu and Weixin with local agent sessions
- Build Acode lifecycle telemetry across turns, tools, MCP, skills, subagents, plugins, context compaction, and token usage
- Develop observability and automated Elastic trace lookup to feed real-task failures into model/harness debugging, bug fixes, and regression testing

---

**OPPO** | Voice Algorithm Development Engineer  
_Oct 2024 - Jan 2025_

- Developed multi-scenario noise reduction algorithms for voice calls
- Algorithms deployed in **OPPO OnePlus 14** and later models
- Technologies: Voice signal processing, noise reduction, real-time audio processing

---

## 🚀 Projects

### 🤖 AI Agent & Application Development

#### [solo-leveling](https://github.com/zjn20021020/solo-leveling)
**Self-learning Skill and Memory plugin for OpenClaw**

- Detects user corrections and conversation friction through lifecycle hooks
- Distills reusable Skills with skip/new/revise decisions and injects relevant experience into future contexts
- Uses atomic writes, an indexed registry, and session-level deduplication to limit memory pollution

**Tech Stack**: `TypeScript` `OpenClaw Plugin SDK` `Skills` `Memory` `Context Engineering`

---

#### [Pi_based-knowledge-agent](https://github.com/zjn20021020/Pi_based-knowledge-agent)
**Conversational academic RAG agent built on the Pi Agent harness**

- Injects 15 custom tools for paper collection management, arXiv retrieval, PDF parsing, indexing, and search
- Uses ReAct-style routing across multiple collections and returns section-aware evidence

**Tech Stack**: `TypeScript` `Pi Agent` `Tool Use` `RAG` `Embedding` `SQLite`

---

#### [PaperAgent](https://github.com/zjn20021020/PaperAgent)
**End-to-end academic workflow built with LangGraph**

- Models planning, retrieval, experiment design, section writing, and review as a 14-node state graph
- Uses conditional branches and two iterative loops for section-level and paper-level quality control

**Tech Stack**: `Python` `LangGraph` `Multi-Agent` `Planning` `State Machine`

---

#### [ScholarLife-Agent](https://github.com/zjn20021020/ScholarLife-Agent)
**Multi-scenario AI Assistant for Students & Researchers**

An intelligent assistant system built on Dify, featuring:
- 📚 Paper search & literature management
- ✍️ Academic writing enhancement & AI-flavor reduction
- 📝 Paper review assistance
- 🔧 Daily research tools

**Tech Stack**: `Dify` `LLM` `AI Agent` `Workflow Orchestration`

---

### 🤖 Embedded Intelligent Systems

#### [bbcar](https://github.com/zjn20021020/bbcar)
**Mecanum-wheel Omnidirectional Robot Car based on STM32G474**

- IMU attitude calculation + encoder wheel speed feedback
- PID closed-loop control system
- Infrared tracking functionality
- Multi-sensor fusion control

**Tech Stack**: `STM32` `C` `Keil` `PID Control` `Sensor Fusion`

---

#### FPGA Gesture-controlled Snake Game [[📹 Demo]](https://www.bilibili.com/video/BV1nP411K7T8)
**Snake Game Controlled by Body Gestures**

- Recognizes human body posture through computer vision
- Deployed on FPGA for real-time interaction
- Integration of posture recognition and game logic

**Tech Stack**: `FPGA` `OpenCV` `Computer Vision`

---

### 🤝 Collaborative Projects

#### [henryzhuhr/deep-lane-detection](https://github.com/henryzhuhr/deep-lane-detection)
**Deep Learning-based Lane Detection**

- Detects lane lines in video footage
- Implements lane detection using deep learning methods
- Trained model deployed on Jetson Nano using TensorRT for high inference efficiency
- Achieves vehicle tracking based on detection results, navigating complex road sections without touching lane lines

**Tech Stack**: `PyTorch` `TensorRT` `Jetson Nano` `Computer Vision`

---

## 📝 Publications

### Conference Papers

**Achieving Vendor-Agnostic Perfusion Imaging with PCASL using the Pulseq Framework**  
**Zhang, Jianing**, Wang, Jun, Li, Hongwei, Ye, Shaoyou, Okell, Thomas, Li, Xiaohu, Ji, Yang  
_ISMRM-ISMRT Annual Meeting & Exhibition_, Cape Town, South Africa, May 2026  
Program Number: 661-01-011 | [View Abstract](http://echo.ismrm.org/abstracts/view/773ce267-4fd2-4b8b-b367-eec6be612400)

> 💡 Independently developed a vendor-agnostic MRI implementation compatible with **GE / Siemens / Philips / United Imaging**  
> 📄 Extended work submitted to **_Magnetic Resonance in Medicine_** (under review)

### Patents

Emotion Analysis System Based on EEG Signals | Application No.: CN202311089224.X

---

## 🏆 Honors & Awards

### Honors

- 🥇 **National Scholarship** (2023)
- 🏅 **KPMG Scholarship** (2022)
- 📚 **First-class Scholarship** (2022, 2023, 2024)

### Competitions

- 🥈 **National Optoelectronic Design Contest - 2nd Prize** (2023)  
  Project: Maze Treasure Hunt Car (vision recognition & autonomous navigation) [[📹 Demo]](https://www.bilibili.com/video/BV1cN411z7co)
  
- 🥇 **National Undergraduate Electronics Design Contest - Provincial 1st Prize** (2023)  
  Problem F: Intelligent Positioning System Based on Sound Propagation (algorithm implementation & neural network deployment)
  
- 🏆 **Hubei Electronics Design Contest - Grand Prize** (2022)  
  Problem C: Vehicle Following System (dual-vehicle coordination, adaptive following & overtaking) [[📹 Demo]](https://www.bilibili.com/video/BV1JB4y1t7NL)

---

## 🛠️ Tech Stack

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

**Keywords**: `Agent Harness` · `Agent Loop` · `Tool Use` · `Skills` · `MCP` · `Memory` · `Subagent` · `Multi-Agent` · `Context Engineering` · `LangGraph` · `RAG` · `WebSocket` · `Observability`

---

## 📫 Contact

- 📧 Email: zhangjianing@mail.ustc.edu.cn
- 💬 Open to discuss: Agent Harness, AI Agent, and LLM systems engineering

---

## 📊 GitHub Stats

<div align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=zjn20021020&show_icons=true&hide_border=true&count_private=true&theme=default" alt="GitHub stats">
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=zjn20021020&layout=compact&hide_border=true&langs_count=8" alt="Top languages">
</div>

---

<div align="center">
  <sub>🤝 Open to collaboration and communication</sub>
</div>
