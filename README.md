<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,100:1a2744&height=120&section=header&text=Vedant%20Kaulgekar&fontSize=42&fontColor=ffffff&fontAlignY=65&animation=fadeIn" width="100%"/>

### AI/ML Engineer · Data Scientist · Full-Stack Developer

[![LinkedIn](https://img.shields.io/badge/LinkedIn-vedant--kaulgekar-0a66c2?style=flat-square&logo=linkedin)](https://linkedin.com/in/vedant-kaulgekar)
[![GitHub](https://img.shields.io/badge/GitHub-VedantKaulgekar-181717?style=flat-square&logo=github)](https://github.com/VedantKaulgekar)
[![HuggingFace](https://img.shields.io/badge/🤗%20Hugging%20Face-VedantKaulgekar-ff9d00?style=flat-square)](https://huggingface.co/VedantKaulgekar)
[![Email](https://img.shields.io/badge/Email-vedantkaulgekar.work@gmail.com-ea4335?style=flat-square&logo=gmail&logoColor=white)](mailto:vedantkaulgekar.work@gmail.com)
![Profile views](https://komarev.com/ghpvc/?username=VedantKaulgekar&color=4a9eff&style=flat-square&label=Profile+Views)

*4th-year Engineering student, Pune · Building end-to-end AI systems that go beyond the notebook.*

*Where machine learning, data science, and software engineering converge.*

</div>

---

## 🚀 Flagship Project — Automotive Decision Intelligence Platform

> **Industrial ML models are black boxes. This platform makes them auditable, uncertain, and explainable.**

An end-to-end AI platform for **automotive factory sustainability analytics** — from raw sensor data to regulatory compliance, with uncertainty you can trust.

```
┌──────────────────────────────────────────────────────────────────┐
│  AutoML Pipeline  →  7 candidate models trained in parallel      │
│  (RandomForest · XGBoost · LightGBM · MLP + 3 more)              │
│  via ThreadPoolExecutor — best model selected automatically      │
│                                                                  │
│  Monte Carlo UQ  →  real sensor noise from datasheets            │
│  propagated through trained models → P5 / P95 output bounds      │
│                                                                  │
│  RAG Q&A  →  FAISS vector search + Groq LLM (llama-3.1-8b)       │
│  grounded strictly in uploaded policy documents                  │
│                                                                  │
│  Dashboard  →  Streamlit + Plotly · sensitivity tornado plots    │
│  PDF export · deployable as web app or native desktop (pywebview)│
└──────────────────────────────────────────────────────────────────┘
```

| Capability | Details |
|---|---|
| Model selection | 7-way parallel AutoML with automatic champion selection |
| Uncertainty quantification | Monte Carlo — datasheets-grounded sensor noise, P5/P95 bounds |
| Regulatory Q&A | RAG-powered, strictly document-grounded (no hallucination) |
| Deployment targets | Streamlit web app **or** native desktop via pywebview |

[![GitHub](https://img.shields.io/badge/GitHub-Automotive--Decision--Intelligence--Platform-181717?style=flat-square&logo=github)](https://github.com/VedantKaulgekar/Automotive-Decision-Intelligence-Platform)

`Python` `Streamlit` `scikit-learn` `XGBoost` `LightGBM` `FAISS` `sentence-transformers` `Groq` `Plotly` `ReportLab`

---

## 🔬 Projects

<table>
<tr>
<td width="50%" valign="top">

### [CreditMaze](https://github.com/VedantKaulgekar/CreditMaze)
OpenEnv-compatible RL benchmark for evaluating credit assignment in long-horizon LLM agent tasks. Submitted to the **Meta PyTorch OpenEnv Hackathon**.
- Simulates research synthesis, debugging, resource allocation, and triage
- Hidden pivotal steps + decoy steps to isolate causal credit
- Normalized graders measure whether agents credit the actions that actually mattered
- Algorithm-agnostic: compatible with GRPO, PPO, iStar, HCAPO

`Python` `PyTorch` `OpenEnv` `FastAPI` `Docker` `RL`

</td>
<td width="50%" valign="top">

### [AgriTech Platform](https://github.com/VedantKaulgekar/AgriTech-Platform)
AI-powered agricultural intelligence platform — data-driven insights for farmers who can't afford to be wrong.
- Crop and soil analysis with ML-driven recommendations
- Interactive dashboards for field-level decision support
- Built for real-world data availability constraints

`Python` `Jupyter Notebook` `HTML`

</td>
</tr>
</table>

---

## ⚙️ Tech Stack

```python
LANGUAGES     = ["Python", "PHP", "HTML5", "SQL"]

ML_AI         = ["scikit-learn", "XGBoost", "LightGBM", "PyTorch",
                 "FAISS", "sentence-transformers", "LangChain"]

DATA          = ["Pandas", "NumPy", "Plotly", "Matplotlib"]

LLM_INFRA     = ["RAG pipelines", "Groq API", "vector search",
                 "document-grounded Q&A"]

RL            = ["OpenEnv", "GRPO", "PPO", "credit assignment", "LLM agents"]

BACKEND       = ["FastAPI", "Streamlit", "pywebview", "ReportLab", "Docker"]

TOOLS         = ["Git", "GitHub", "Jupyter", "VS Code"]
```

---

## 🎯 Interests

- 🤖 **AutoML & MLOps** — production-grade pipelines, not just notebooks
- 🔍 **RAG & LLM applications** — grounded, auditable, deployable
- 🧠 **RL & agent evaluation** — credit assignment, long-horizon reasoning
- 📊 **Decision intelligence** — uncertainty quantification, sensitivity analysis
- 🌱 **AI for real-world impact** — sustainability, agriculture, industry

---

## 🤖 Robotics — ABU Robocon 2026

**Team Vulcans · Software Lead (Robot 2)**

Built the complete ROS2 runtime and GPU perception stack for R2 — the autonomous robot responsible for KFS collection (Zone 2) and Tic-Tac-Toe placement (Zone 3) in the *Kung Fu Quest* theme.

```
┌─────────────────────────────────────────────────────────────────────┐
│  8 ROS2 nodes running simultaneously on Jetson Orin Nano 8GB        │
│                                                                     │
│  communication_node  (C++)  — Binary ESP-1 serial @ 200 Hz TX       │
│  hardware_interface_node (Py) — ASCII ESP-2/3 bridge + E-stop chain │
│  climb_action_node   (Py)   — rclpy action server, non-blocking FSM │
│  sensor_fusion_node  (C++)  — Encoder + IMU → RobotPose @ 100 Hz    │
│  safety_monitor_node (C++)  — 50 Hz E-stop watchdog                 │
│  state_machine_node  (C++)  — Global FSM @ 20 Hz                    │
│  perception_node     (C++)  — CUDA kernels + TensorRT @ ~15 Hz      │
│  planner_node        (C++)  — A* Zone 2 + RL Zone 3 @ 20 Hz         │
└─────────────────────────────────────────────────────────────────────┘
```

**My contribution — ROS2 architecture & GPU perception:**
- Designed and implemented all 8 ROS2 nodes and the custom `r2_msgs` package (strongly-typed messages + `ClimbAction` action interface)
- Built `hardware_interface_node` — ASCII bridge to ESP-2/3, routing all actuator commands through the ROS2 graph and wiring them into the E-stop chain (previously unreachable by the safety monitor)
- Built `climb_action_node` — non-blocking `rclpy.action` server replacing blocking `time.sleep()` climb sequences; executor never stalls
- Implemented `perception_node` GPU pipeline: CUDA preprocessing kernels (sm_87), TensorRT FP16 YOLOv11s-seg for Zone 1 spearhead detection, YOLOv8 + ByteTrack + CUDA belief map for Zone 2, ArUco + HSV classifier for Zone 3 rack detection

[![GitHub](https://img.shields.io/badge/GitHub-ABU--Robocon--2026-181717?style=flat-square&logo=github)](https://github.com/VedantKaulgekar/ABU-Robocon-2026)

`ROS2 Humble` `C++17` `Python` `CUDA` `TensorRT` `YOLOv11s-seg` `YOLOv8` `OpenCV` `Jetson Orin Nano` `rclpy.action`

---

## 📈 Contribution Activity

![GitHub Streak](https://streak-stats.demolab.com?user=VedantKaulgekar&theme=dark&hide_border=true&background=0d1117&ring=4a9eff&fire=4a9eff&currStreakLabel=4a9eff)

---

## 📫 Connect

- 💼 [linkedin.com/in/vedant-kaulgekar](https://linkedin.com/in/vedant-kaulgekar)
- 📧 [vedantkaulgekar.work@gmail.com](mailto:vedantkaulgekar.work@gmail.com)
- 📍 Pune, Maharashtra, India
- 📬 **Open to internships, collaborations, and interesting problems**

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1a2744,100:0d1117&height=80&section=footer" width="100%"/>

*"Building intelligent systems that solve real-world problems."*

![Profile views](https://komarev.com/ghpvc/?username=VedantKaulgekar&color=4a9eff&style=flat-square&label=Profile+Views)

</div>
