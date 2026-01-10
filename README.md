# 🛰️ Physical-AI Subsurface Perception using GPR

This repository implements a **Physical-AI perception stack** for autonomous robots equipped with **Ground-Penetrating Radar (GPR)**.

Unlike classical obstacle-avoidance systems, this framework enables robots to **reason about buried hazards before physical interaction**, allowing **pre-emptive safety behaviour** instead of reactive collision handling.

The system includes a **live subsurface visualization interface** that converts raw GPR signals into real-time underground perception displays, making hidden hazards directly observable to operators and developers.

---

## 🧠 Perception Architecture

**GPR Antenna → B-Scan Formation → Subsurface Feature Encoding → Anomaly-Based Hazard Detection → Physical-AI Safety Supervisor → Robot Motion Constraint / Tool Control**

---

## 📸 Live Visualization Outputs

### Figure 1 –Raw GPR B-Scan: Subsurface Reflection Profile  
<img width="321" height="360" alt="Screenshot_1" src="https://github.com/user-attachments/assets/60e7a4f1-8d41-4973-80d5-31134525650e" />

### Figure 2 – High-Frequency Radar Texture: Clutter & Micro-Reflections  
<img width="315" height="358" alt="Screenshot_2" src="https://github.com/user-attachments/assets/f0e0d51f-e7b7-469d-b128-ad630cec2350" />

### Figure 3 – Encoded Subsurface Feature Map  
<img width="511" height="547" alt="Screenshot_3" src="https://github.com/user-attachments/assets/3f7de418-f9de-4d8d-9085-d419face5589" />

### Figure 4 – Raw GPR vs Encoded Feature Representation  
<img width="633" height="354" alt="Screenshot_4" src="https://github.com/user-attachments/assets/56e2eac9-5145-4590-bedb-fdfa2cf73744" />

### Figure 5 – Physical-AI Safety Supervisor: SAFE TERRAIN  
<img width="322" height="359" alt="Screenshot_5" src="https://github.com/user-attachments/assets/b53fb331-c278-410f-89a8-c20cf87a5f47" />

### Figure 6 – Physical-AI Safety Supervisor: HIGH-RISK Subsurface Anomaly  
<img width="319" height="355" alt="Screenshot_6" src="https://github.com/user-attachments/assets/9e10eab1-8adc-44bd-85ae-b13656a474dc" />



*All windows are generated live while the robot processes underground radar signals.*

---

## 📂 Repository Structure

<img width="297" height="239" alt="image" src="https://github.com/user-attachments/assets/c3301540-e897-4944-b3b1-0ebf2eb73784" />


---

## 🔧 File Responsibilities

| Script | Description |
|-------|-------------|
| `gpr_dataset.py` | Robust multi-folder GPR dataset loader |
| `gpr_live_view.py` | Real-time GPR sensor feed visualizer |
| `gpr_feature_map.py` | Subsurface feature encoding |
| `gpr_hazard_map.py` | Buried hazard intensity heat-map |
| `gpr_safety_supervisor.py` | Physical-AI safety controller with live risk alerts |
| `main_demo.py` | Subsurface object detection with bounding boxes |

---

## ▶ Installation

```bash
pip install numpy opencv-python

