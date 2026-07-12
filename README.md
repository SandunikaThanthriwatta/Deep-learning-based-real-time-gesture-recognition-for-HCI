# 🖐️ Device-Free Hand Gesture Recognition for Human-Computer Interaction

<p align="center">
  <b>Real-time, webcam-only static & dynamic gesture recognition for touchless computer control</b>
</p>

<p align="center">
  <img alt="Python" src="https://img.shields.io/badge/Python-3.8-3776AB?style=for-the-badge&logo=python&logoColor=white">
  <img alt="TensorFlow" src="https://img.shields.io/badge/TensorFlow-CNN-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white">
  <img alt="OpenCV" src="https://img.shields.io/badge/OpenCV-Vision-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white">
  <img alt="PyQt" src="https://img.shields.io/badge/PyQt-Desktop%20UI-41CD52?style=for-the-badge&logo=qt&logoColor=white">
  <img alt="Flask" src="https://img.shields.io/badge/Flask-Mobile%20API-000000?style=for-the-badge&logo=flask&logoColor=white">
</p>

<p align="center">
  <img alt="Accuracy" src="https://img.shields.io/badge/Test%20Accuracy-99.81%25-success?style=flat-square">
  <img alt="Dataset" src="https://img.shields.io/badge/Dataset-88%2C000%20images-blue?style=flat-square">
  <img alt="Device" src="https://img.shields.io/badge/Sensor-Ordinary%20Webcam-lightgrey?style=flat-square">
  <img alt="Status" src="https://img.shields.io/badge/Status-Published-brightgreen?style=flat-square">
</p>

---

## 📄 Abstract

Gesture-driven interfaces are improving Human–Computer Interaction (HCI) by offering users a more natural, intuitive way to communicate with systems. This research presents a real-time hand gesture recognition framework that serves as an alternative to traditional input hardware, with static and dynamic gestures captured through an ordinary webcam. A custom-built dataset of **88,000 images** and a deep **Convolutional Neural Network (CNN)** were developed to support robust gesture recognition under diverse lighting and background conditions. Unlike existing systems that depend on depth sensors or computationally heavy models, the proposed method infers dynamic gestures by combining static CNN predictions with real-time directional hand movement analysis. The system enables seamless control of media players, presentations, system-level functions, and other frequently used applications, supported by a **PyQt-based interface** and **mobile remote-control support**. Achieving **99.81% testing accuracy** with low latency, this work demonstrates an accessible, efficient, device-free and practical approach to gesture-based interaction. The proposed framework advances HCI by enhancing usability, reducing device dependency, and broadening accessibility for a wide range of users.

---

## 📚 Publications

| | Title | Venue | Date |
|---|---|---|---|
| 📰 | **[Device-Free Hand Gesture Recognition for Human Computer Interaction Using Deep Learning](https://ieeexplore.ieee.org/document/11497830)** | IEEE Xplore — ICIPROB Conference | May 5, 2026 |
| 📰 | **[Gesture Recognition for Human-Computer Interaction Using Deep Learning](https://science.sjp.ac.lk/insoc/2024/08/16/symposium-e-book-release/)** | 10th Undergraduate Research Symposium (UNI-IN ALLIANCE 2024) | Aug 16, 2024 |

---

## ✨ Highlights

- 🎥 **Device-free** — no depth sensors, gloves, or wearables; works with any ordinary webcam
- 🧠 **Custom deep CNN** trained on a self-built **88,000-image** dataset across varied lighting/backgrounds
- ✋ **Static + dynamic gestures** — dynamic gestures inferred by combining CNN predictions with real-time directional hand-movement analysis (no heavy video models required)
- 🎯 **99.81% test accuracy** with low inference latency
- 🖥️ **PyQt desktop app** for gesture-driven control of media players, presentations, and system functions
- 📱 **Mobile remote control** via a Flask-based companion app
- 🔊 **Voice assistance module** and sound feedback for confirmation of recognized actions
- ⚙️ **Configurable gesture → action mapping** per mode (Static, Dynamic, Auto)

---

## 🤟 Supported Gestures

| # | Gesture | # | Gesture |
|---|---|---|---|
| 0 | Palm | 5 | L |
| 1 | Thumbs Up | 6 | Swag |
| 2 | Rock | 7 | C |
| 3 | Thumbs Left | 8 | Three Fingers |
| 4 | V | 9 | Scissor |

## 🎮 Controllable Applications

Each gesture (or gesture sequence, in Auto mode) can be mapped to one of the following contexts:

`VLC` · `System` · `Reading` · `Presentation` · `YouTube` · `Zoom` · and more, switchable through **Static**, **Dynamic**, and **Auto** operating modes.

---

## 🗂️ Project Structure

```text
├── 1_Model_Binding/                 # CNN inference & gesture prediction pipeline
├── 2_Application_Actions/           # Action handlers triggered by recognized gestures
├── 3_Intended_Gesture_Mapping/      # Gesture → intended-action mapping logic
├── 4_Voice_Assistance/              # Voice feedback / assistance module
├── 5_Mode_Selector/                 # Static / Dynamic / Auto mode switching
├── 6_Settings/                      # User-configurable settings
├── 7_Sound_manipulating/            # Audio feedback utilities
├── 8_Dynamic_Gesture_Recognition/   # Directional movement analysis for dynamic gestures
├── 9_Mobile_App/                    # Flask server + mobile remote-control app
├── 10_Storage_and_utils/            # Persistence & shared utilities
├── System_Backend/                  # Application entry point (main.py)
├── User_Interface/                  # PyQt desktop UI (windows, tray, icons)
├── Assets/                          # Sounds & static assets
├── Results_planning/                # Performance testers & evaluation scripts
└── Manual.txt                       # Gesture ↔ application mapping reference
```

---

## 🚀 Getting Started

```bash
# Clone the repository
git clone https://github.com/SandunikaThanthriwatta/gesture-based-hci-v2.git
cd gesture-based-hci-v2

# Install core dependencies
pip install tensorflow opencv-python pyqt5 flask numpy

# Launch the desktop application
python System_Backend/main.py
```

> 💡 See [`Manual.txt`](Manual.txt) for the full gesture-number ↔ application mapping across Static, Dynamic, and Auto modes.

---

## 🧩 Tech Stack

<p>
  <img src="https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white">
  <img src="https://img.shields.io/badge/-TensorFlow%2FKeras-FF6F00?style=flat-square&logo=tensorflow&logoColor=white">
  <img src="https://img.shields.io/badge/-OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white">
  <img src="https://img.shields.io/badge/-PyQt5-41CD52?style=flat-square&logo=qt&logoColor=white">
  <img src="https://img.shields.io/badge/-Flask-000000?style=flat-square&logo=flask&logoColor=white">
  <img src="https://img.shields.io/badge/-ONNX-005CED?style=flat-square&logo=onnx&logoColor=white">
  <img src="https://img.shields.io/badge/-NumPy-013243?style=flat-square&logo=numpy&logoColor=white">
</p>

---

## 📖 Citation

If you use this work, please cite:

```bibtex
@inproceedings{gesture_hci_iciprob,
  title     = {Device-Free Hand Gesture Recognition for Human Computer Interaction Using Deep Learning},
  booktitle = {Proceedings of the International Conference on Probabilistic and Data-Driven Modelling (ICIPROB)},
  year      = {2026},
  url       = {https://ieeexplore.ieee.org/document/11497830}
}
```

---

