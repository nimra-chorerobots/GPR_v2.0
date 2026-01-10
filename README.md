##🛰️ Physical-AI Subsurface Perception using GPR##

This repository implements a Physical-AI perception stack for autonomous robots equipped with Ground-Penetrating Radar (GPR).

Unlike classical obstacle-avoidance systems, this framework enables robots to reason about buried hazards before physical interaction, allowing pre-emptive safety behavior instead of reactive collision handling.

The system includes a live subsurface visualization interface that converts raw GPR signals into real-time underground perception displays, making hidden hazards directly observable to operators and system developers.

#🧠 Perception Architecture#
GPR Antenna
     ↓
B-Scan Formation
     ↓
Subsurface Feature Encoding
     ↓
Anomaly-Based Hazard Detection
     ↓
Physical-AI Safety Supervisor
     ↓
Robot Motion Constraint / Tool Control

#📸 Live Visualization Outputs#
<img width="321" height="360" alt="Screenshot_1" src="https://github.com/user-attachments/assets/ceeaa5c2-89c8-4f37-8e47-c44dcf6fed2e" />

Raw GPR B-Scan — Subsurface Reflection Profile

<img width="315" height="358" alt="Screenshot_2" src="https://github.com/user-attachments/assets/429f9a99-216f-45dd-8141-25a7709b4baa" />

High-Frequency Radar Texture — Clutter & Micro-Reflections

<img width="511" height="547" alt="Screenshot_3" src="https://github.com/user-attachments/assets/bc6d5903-9c16-48cb-87d8-d3ca5cdb8157" />

Encoded Subsurface Feature Map

<img width="633" height="354" alt="Screenshot_4" src="https://github.com/user-attachments/assets/673712e7-f59e-417b-b5d8-2dd041a45b7f" />

Raw GPR vs Encoded Feature Representation

<img width="322" height="359" alt="Screenshot_5" src="https://github.com/user-attachments/assets/998223dc-2abf-453b-b0c6-b3d660cafb60" />

Physical-AI Safety Supervisor — SAFE TERRAIN State

<img width="319" height="355" alt="Screenshot_6" src="https://github.com/user-attachments/assets/d56d8b13-5c71-4dd5-92fc-71458e88082c" />

Physical-AI Safety Supervisor — HIGH RISK Subsurface Anomaly Detected

 
These windows are generated live while the robot processes underground radar signals.

#📂 Repository Structure#
physical-ai-gpr-perception/
 ├── gpr_dataset.py
 ├── gpr_live_view.py
 ├── gpr_feature_map.py
 ├── gpr_hazard_map.py
 ├── gpr_safety_supervisor.py
 └── main_demo.py

# 🔧 File Responsibilities#
 | Script                     | Function                                            |
| -------------------------- | --------------------------------------------------- |
| `gpr_dataset.py`           | Robust multi-folder GPR dataset loader              |
| `gpr_live_view.py`         | Real-time GPR sensor feed visualizer                |
| `gpr_feature_map.py`       | Subsurface feature encoding                         |
| `gpr_hazard_map.py`        | Buried hazard intensity heat-map                    |
| `gpr_safety_supervisor.py` | Physical-AI safety controller with live risk alerts |
| `main_demo.py`             | Subsurface object detection with bounding boxes     |


▶ Installation
pip install numpy opencv-python


#🚀 Run Demos#
| Demo              | Command                           |
| ----------------- | --------------------------------- |
| Live GPR Feed     | `python gpr_live_view.py`         |
| Feature Encoding  | `python gpr_feature_map.py`       |
| Hazard Heat-Map   | `python gpr_hazard_map.py`        |
| Safety Supervisor | `python gpr_safety_supervisor.py` |
| Object Detection  | `python main_demo.py`             |

🛡️ Safety Supervisor Logic

The system computes high-frequency anomaly energy from radar B-scans to detect buried objects and terrain irregularities.

  
