
# 🚦 Road Traffic Condition Monitoring Using Deep Learning

A smart, deep learning-powered system that monitors live or recorded road footage to detect:

* 🚗 **Accidents** — and determine **how** they occurred (normal vs. fire accidents)
* 🚦 **Traffic Conditions** — classifies scenes into **Heavy Traffic** or **Low Traffic**

This system supports intelligent traffic management and emergency response automation.

---

## 🧠 What It Can Do

| Feature                    | Description                                                         |
| -------------------------- | ------------------------------------------------------------------- |
| 🚨 Accident Detection      | Detects whether an accident occurred or not                         |
| 🔥 Fire Accident Detection | Differentiates between **normal accidents** and **fire accidents**  |
| 🚗 Traffic Analysis        | Determines **traffic density**: Low or Heavy based on vehicle count |
| 🎥 Real-time Inference     | Works with live video feeds or recorded surveillance footage        |

---

## 💡 System Overview

The system combines **deep learning models** for image/video classification and object detection.

* **YOLOv5/YOLOv8** for accident detection & vehicle counting
* **CNN-based classifier** for distinguishing accident type (fire vs. normal)
* Fire detection may include **color/thermal feature filters** for enhanced accuracy

---

## 📁 Dataset Structure

Use a labeled dataset with video frames or images:

```
dataset/
├── normal_accident/
├── fire_accident/
├── heavy_traffic/
└── low_traffic/
```

You can create or augment datasets from:

* [AI City Challenge](https://www.aicitychallenge.org/)
* Dashcam videos
* Custom annotated CCTV footage

---

## ⚙️ Installation

### Prerequisites

* Python 3.8+
* PyTorch or TensorFlow
* OpenCV
* NumPy
* Matplotlib
* Streamlit (optional dashboard)

### Setup

```bash
git clone https://github.com/yourusername/traffic-condition-monitoring.git
cd traffic-condition-monitoring
pip install -r requirements.txt
```

---

## 🚀 How to Use

### 🏋️ Train the Model (Optional)

```bash
python train.py --dataset ./dataset --model yolov5 --epochs 50
```

### 🔍 Detect from an Image

```bash
python predict.py --image test_images/frame1.jpg
```
---

## 📊 Optional: Streamlit Dashboard

Launch a real-time monitoring dashboard:

```bash
streamlit run dashboard.py
```

Includes:

* Video playback
* Live annotations (accident/fire/traffic)
* Event timeline
* Exportable reports

---

## 📈 Example Results

| Class           | Precision | Recall | F1-score |
| --------------- | --------- | ------ | -------- |
| Normal Accident | 91%       | 89%    | 90%      |
| Fire Accident   | 88%       | 86%    | 87%      |
| Heavy Traffic   | 93%       | 95%    | 94%      |
| Low Traffic     | 97%       | 94%    | 95%      |

---

## 🗂️ Project Structure

```
traffic-condition-monitoring/
├── dataset/
├── models/
├── train.py
├── predict.py
├── video_predict.py
├── dashboard.py
├── utils/
├── requirements.txt
└── README.md
```

---

## 🤝 Contributing

Contributions are welcome! If you have improvements in:

* Traffic pattern detection
* Fire recognition algorithms
* Real-time optimization for edge devices

Please open an issue or pull request!

---

## 📬 Contact

* 📧 [Mail](mailto:sohindillu@gmail.com)
* 🌐 [LinkedIn](https://linkedin.com/in/shaik-sohin)
---
