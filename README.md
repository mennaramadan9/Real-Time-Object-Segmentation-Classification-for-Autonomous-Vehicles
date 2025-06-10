# AutoVision 🚗📹  
**Real-Time Object Segmentation and Classification for Autonomous Driving**

AutoVision is a computer vision pipeline built in Python using PyTorch and OpenCV, designed to perform real-time semantic segmentation and object classification on video input — a foundational step for autonomous vehicle perception systems.

---

## 🧠 Features

- 🔍 Real-time object **segmentation** using DeepLabV3-ResNet101  
- 🏷️ Object **classification** using EfficientNet-B0 pretrained on ImageNet  
- 📦 Google Colab-compatible with GPU acceleration  
- 🎥 Supports any video input and exports annotated video with bounding boxes + labels  
- ⚙️ Modular and customizable for AVs, robotics, or surveillance  

---

## 🎥 How It Works

1. Upload a video (e.g., dashcam footage).
2. Each frame is segmented using DeepLabV3.
3. Objects are cropped and classified with EfficientNet.
4. Bounding boxes and labels are drawn on the frame.
5. Final annotated video is saved as `output.mp4`.

---

## 📁 Project Structure

```
📂 AutoVision/
├── README.md              ← Project description and instructions
├── main.ipynb             ← Google Colab Notebook
```

---

## ⚙️ Requirements

> If running locally (not in Colab):

```bash
pip install torch torchvision opencv-python timm
```

For best performance, use **Google Colab with GPU** enabled.

---

## 🧪 Models Used

| Task           | Model                  | Framework   |
|----------------|------------------------|-------------|
| Segmentation   | DeepLabV3 + ResNet101  | torchvision |
| Classification | EfficientNet-B0        | torchvision |

---

## ✅ How to Use in Google Colab

1. Upload your video when prompted in the notebook.
2. Run all cells in `main.ipynb`.
3. After processing, download `output.mp4`.
