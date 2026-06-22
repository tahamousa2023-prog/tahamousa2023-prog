<h1 align="center">👋 Hi, I'm Taha Mohammed</h1>

<p align="center">
  <strong>Mechatronics Engineer · MSc Computational Engineering Science · TU Berlin</strong><br/>
  Robotics researcher building perception-action systems that work <em>outside</em> controlled lab conditions.<br/>
  Previously at <strong>Siemens AG</strong> (4.5 yrs) · <strong>Fraunhofer IPK</strong> (Master Thesis) · <strong>TU Berlin</strong>
</p>

<p align="center">
  <a href="https://linkedin.com/in/taha-mahmoud">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
  <a href="https://tahamousa2023-prog.github.io">
    <img src="https://img.shields.io/badge/Portfolio-1a1a2e?style=for-the-badge&logo=githubpages&logoColor=white" />
  </a>
  <img src="https://img.shields.io/badge/Open_to_PhD_&_Research_Roles-FF375F?style=for-the-badge&logoColor=white" />
</p>

---

## 🎯 Research Focus

I build systems where robots must **perceive, decide, and act** in environments they were not explicitly designed for. My work sits at the intersection of:

- **Reinforcement Learning for Robot Control** — PPO-based agents for camera trajectory optimisation and viewpoint selection, trained in NVIDIA Isaac Sim using the Arena-Rosnav simulation framework
- **3D Perception & Reconstruction** — RGB-D sensor fusion, ICP/FPFH registration, VGGT-based surface fitting
- **Vision-Based Robot Calibration** — ResNet-18 CNNs for intelligent pose selection in TCP calibration (Fraunhofer IPK)
- **Sim-to-Real Transfer** — Deployable pipelines from Isaac Sim → UR5e physical robot

---

## 📄 Publication

### Camera-Orientation Effects in Robotic Viewpoint Acquisition for Feed-Forward 3D Reconstruction in Manufacturing Inspection Workcells
> **Submitted to The International Journal of Advanced Manufacturing Technology (Springer) · June 2026**

**Authors:** Adam Michael Altenbuchner, Richard Matthias Hartisch, **Taha Mohammed**, Ziad Abouhalawa, Artem Balatsiuk, Aziz Louati, Haroun Lallouche, Jörg Krüger · TU Berlin & Fraunhofer IPK

A modular simulation-based robotic inspection pipeline combining UR5e eye-in-hand acquisition, feed-forward 3D reconstruction (VGGT, Fast3R, SAM3D), point-cloud preprocessing, metric-scale correction, and ICP/FPFH registration-based evaluation. The study isolates camera orientation as a controllable acquisition variable, showing that object-pointing orientation increases mean registration fitness from 0.68 → 0.79 and reduces mean inlier RMSE from 0.035 m → 0.022 m across five scan patterns. A PPO-based coverage-learning module is analysed as a feasibility study for adaptive viewpoint acquisition.

`VGGT` `Fast3R` `ICP/FPFH` `PPO` `Isaac Sim` `UR5e` `ROS2` `Open3D`

---

## 🚀 Research Projects

### 🤖 [Path Matters](https://github.com/tahamousa2023-prog/path-matters-robotics) — RL Camera Trajectory for 3D Reconstruction
> **TU Berlin · WiSe 25/26**

PPO-based camera trajectory optimisation for robotic 3D reconstruction. A UR5e agent learns **where to look** to maximise surface coverage — trained in NVIDIA Isaac Sim using the Arena-Rosnav simulation framework.

| Metric | Result | Baseline |
|--------|--------|----------|
| VGGT Fitness Score | **0.93** | — |
| PPO Task Success | **45.2%** | 0.4% (sparse reward) |
| vs Random Exploration | — | 0% success |

`ROS2` `Isaac Sim` `PPO (RSL-RL)` `VGGT` `BUFFER-X` `ICP` `UR5e`

---

### 🔬 [TCP Calibration — Fraunhofer IPK](https://github.com/tahamousa2023-prog/tcp-calibration-fraunhofer) — CNN Pose Selection
> **Fraunhofer IPK · Master Thesis**

ResNet-18 CNN trained to select the **optimal 5-pose subset** from a 40-pose calibration protocol — replacing brute-force with learned geometric intuition.

| Metric | Result |
|--------|--------|
| Calibration Speed | **87.5% faster** |
| Accuracy | **76% more accurate** than full random baseline |

`PyTorch` `ResNet-18` `UR5e` `ROS2`

---

### 👁️ [RL Viewpoint Selection](https://github.com/tahamousa2023-prog/rl-viewpoint-selection) — PPO Camera Agent
> **TU Berlin**

PPO agent trained in Isaac Lab to learn optimal camera viewpoints for object inspection and 3D coverage.

- **45.2% task success** with proximity-shaped reward vs **0%** for random exploration baseline

`Isaac Lab` `PPO` `RSL-RL` `Python` `CUDA`

---

### 🤝 [Robotic Viewpoint Acquisition for 3D Reconstruction](https://github.com/Adam-yes/robotic-viewpoint-acquisition-for-3d-reconstruction) — Academic Collaboration
> **TU Berlin · Institute for Machine Tools and Factory Management · 2026**

Active research collaboration contributing to the paper above — data preparation and validation for a modular robotic 3D reconstruction pipeline evaluating feed-forward reconstruction backbones and acquisition strategies in NVIDIA Isaac Sim.

`3D Reconstruction` `Viewpoint Planning` `VGGT` `ICP/FPFH` `ROS2` `Python`

---

## 💻 Tech Stack

### 🦾 Robotics & Simulation
<p>
  <img src="https://img.shields.io/badge/ROS2-22314E?style=for-the-badge&logo=ros&logoColor=white" />
  <img src="https://img.shields.io/badge/Isaac_Sim-76B900?style=for-the-badge&logo=nvidia&logoColor=white" />
  <img src="https://img.shields.io/badge/Isaac_Lab-76B900?style=for-the-badge&logo=nvidia&logoColor=white" />
  <img src="https://img.shields.io/badge/Arena--Rosnav-FF6B35?style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/MoveIt2-2E86AB?style=for-the-badge&logo=ros&logoColor=white" />
  <img src="https://img.shields.io/badge/UR5e-EA4335?style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/NVIDIA_Jetson-76B900?style=for-the-badge&logo=nvidia&logoColor=white" />
</p>

### 🧠 AI / Machine Learning
<p>
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" />
  <img src="https://img.shields.io/badge/Deep_Learning-412991?style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/Reinforcement_Learning-FF6B35?style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/PPO_(RSL--RL)-412991?style=for-the-badge&logo=openai&logoColor=white" />
  <img src="https://img.shields.io/badge/ResNet--18-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white" />
  <img src="https://img.shields.io/badge/YOLO-00FFFF?style=for-the-badge&logo=yolo&logoColor=black" />
  <img src="https://img.shields.io/badge/TensorRT-76B900?style=for-the-badge&logo=nvidia&logoColor=white" />
  <img src="https://img.shields.io/badge/Stable_Baselines3-FF9900?style=for-the-badge&logoColor=white" />
</p>

### 🗺️ 3D Perception & Reconstruction
<p>
  <img src="https://img.shields.io/badge/Computer_Vision-1a1a2e?style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/ICP-1a1a2e?style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/FPFH-2E4057?style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/BUFFER--X-6B4226?style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/Open3D-E95420?style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/VGGT-0D7377?style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/RGB--D_Fusion-333333?style=for-the-badge&logoColor=white" />
</p>

### ⚙️ Systems & Languages
<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white" />
  <img src="https://img.shields.io/badge/CUDA-76B900?style=for-the-badge&logo=nvidia&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/PLC_(Siemens)-009999?style=for-the-badge&logoColor=white" />
  <img src="https://img.shields.io/badge/DCS_(SPPA--T3000)-E84545?style=for-the-badge&logoColor=white" />
</p>

---

## 🔬 Research Interests

```
Reinforcement Learning               Computer Vision
Deep Learning for Robotics           3D Scene Reconstruction
Social Robot Navigation              Sim-to-Real Transfer
Vision-Based Robot Control           Human-Robot Interaction
Foundation Models for Robotics       Embodied AI
```

---

## 🏭 Industry Background

4.5 years at **Siemens AG** through the **Europeans@Siemens** programme:

| Area | Details |
|------|---------|
| **Robot Programming** | UR5e integration · ROS2/MoveIt2 · offline path planning · adaptive control |
| **Machine Vision** | Vision-guided robotic systems · RGB-D sensor integration · CNN-based inspection |
| **PLC & Industrial Automation** | Siemens TIA Portal · ladder logic · production line commissioning |
| **Large-Scale Control Systems** | SPPA-T3000 DCS · control of a **4,800 MW power plant** |
| **Safety & Compliance** | Industrial safety standards · risk assessment in live production environments |
| **Commissioning & Ramp-up** | End-to-end deployment from design → testing → production handover |

> Industrial deployment experience is rare in academic robotics. I think in terms of **what actually works outside the lab** — not just benchmark numbers.

---

## 📊 Coding Practice

<p>
  <a href="https://github.com/tahamousa2023-prog/algo-arena">
    <img src="https://img.shields.io/badge/LeetCode_Repo-algo--arena-FFA116?style=for-the-badge&logo=leetcode&logoColor=black" />
  </a>
  <a href="https://leetcode.com/u/taha_1/">
    <img src="https://img.shields.io/badge/LeetCode-taha__1-FFA116?style=for-the-badge&logo=leetcode&logoColor=black" />
  </a>
</p>

Structured algorithm practice in Python & C++ — Arrays, Trees, Graphs, DP, Backtracking, Graph Search.

---

## 🌐 Connect

<p>
  <a href="https://linkedin.com/in/taha-mahmoud">
    <img src="https://img.shields.io/badge/LinkedIn-Taha_Mahmoud-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
  <a href="https://tahamousa2023-prog.github.io">
    <img src="https://img.shields.io/badge/Portfolio-Website-1a1a2e?style=for-the-badge&logo=githubpages&logoColor=white" />
  </a>
</p>

📍 Berlin, Germany · 📬 Open to **PhD positions**, **Applied Science internships**, and **Research Engineer** roles in robotics, deep learning, and computer vision

---

> *"The question is not whether intelligent machines can think. The question is whether they can act usefully in a world they did not expect."*
