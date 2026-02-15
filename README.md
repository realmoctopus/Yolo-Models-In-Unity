# Yolo Models In Unity
### YOLO Object Detection, Classification, Segmentation & Pose Estimation in Unity – Easy & Powerful Setup

<p align="center">
  <img src="https://assetstorev1-prd-cdn.unity3d.com/key-image/cea043f8-d2fa-4d90-9562-f12d1d5ac759.webp" alt="YoloModelRunner Thumbnail" width="800"/>
</p>

<p align="center">
  <a href="https://assetstore.unity.com/packages/tools/ai-ml-integration/yolomodelrunner-353736">
    <img src="https://img.shields.io/badge/Unity-Asset%20Store-black?logo=unity" />
  </a>
  <a href="https://www.youtube.com/watch?v=E8GOZr2n9fY">
    <img src="https://img.shields.io/badge/Demo-Video-red?logo=youtube" />
  </a>
</p>

---

## 🚀 Overview

**YoloModelRunnerTemplate** is a Unity plugin designed to completely remove the complexity of running YOLO ONNX models inside Unity.

Running YOLO models manually usually requires:

* Understanding fixed input tensor dimensions
* Parsing complex output tensor structures
* Writing custom decoding logic for:

  * Bounding boxes
  * Segmentation masks
  * Pose landmarks
  * Confidence scores

This plugin abstracts all of that.

Simply **drag and drop your YOLO ONNX model** into the `ModelRunner`, and the system automatically handles:

* ✅ Input tensor preparation
* ✅ Model inference execution
* ✅ Output tensor decoding
* ✅ Post-processing (Confidence filtering + IOU filtering)

The final result is returned as a clean, unified **Prediction** structure — ready for immediate use in gameplay, UI overlays, visualization, or analytics.

---

## 🎯 Supported YOLO Model Types

* 🟦 Object Detection
* 🟩 Image Classification
* 🟪 Image Segmentation
* 🟨 Pose Estimation
* 🧠 Custom-trained YOLO models (Detection / Classification / Segmentation / Pose)

---

## ✨ Key Features

### 🔹 Zero-Complexity YOLO Integration

No need to understand YOLO tensor formats.

### 🔹 No External Dependencies

Uses only Unity’s official Inference package.
No third-party runtime dependencies.

### 🔹 Drag & Drop Workflow

Assign your YOLO ONNX model to the `ModelRunner`.

### 🔹 Unified Prediction Output

A single `Prediction` class containing:

* Class index
* Class label
* Confidence score
* Bounding box
* Segmentation mask
* Pose landmarks

### 🔹 Multiple Input Sources

* 🖼 Image Source – single image inference
* 🎬 Video Source – frame-by-frame video inference
* 📷 Webcam Source – real-time camera feed

### 🔹 Post-Processing Controls

* Adjustable **Confidence Threshold**
* Adjustable **IOU (Intersection over Union) Threshold**

### 🔹 Backend Type Selection

* CPU
* GPU Compute
* GPU Pixel

### 🔹 Multiple Demo Scenes

Dedicated demo scenes for:

* Detection
* Classification
* Segmentation
* Pose

---

## 📦 Installation & Setup

### 1️⃣ Import Unity Inference Package

1. Open **Unity Package Manager**
2. Switch to **Unity Registry**
3. Install **Inference / Inference Engine**

This package is required to run ONNX models inside Unity.

---

### 3️⃣ Open a Demo Scene

Open the demo scene that matches your YOLO model type:

* Detection
* Classification
* Segmentation
* Pose

Each scene is preconfigured for correct setup.

---

### 4️⃣ Assign Your YOLO ONNX Model

1. Select the **ModelRunner** GameObject
2. Drag & drop your `.onnx` model into the **ModelAsset** field

The system automatically configures:

* Input size
* Preprocessing
* Output decoding

---

### 5️⃣ Assign Class Labels (Optional)

If using a custom-trained model:

* Assign a `TextAsset` containing class names
* One class per line

If not assigned, embedded/default labels are used (if available).

---

### 6️⃣ Configure Thresholds

Inside the ModelRunner Inspector:

* **Confidence Threshold** → Filters low-confidence predictions
* **IOU Threshold** → Controls overlap suppression

---

## 📥 Input Sources

Switch input sources directly from ModelRunner settings:

| Source | Description                    |
| ------ | ------------------------------ |
| Image  | Static image inference         |
| Video  | Frame-by-frame video inference |
| Webcam | Real-time camera feed          |

---

## ⚡ Performance Tips

### 1. Use Nano / Small Models for Real-Time

Ideal for mobile platforms and AR/VR.

### 2. Use Large Models for Higher Accuracy

Better precision but requires more compute power.

### 3. Use GPU Backend When Available

GPU Compute or GPU Pixel significantly improves inference speed.

---

## 🧩 Recommended Use Cases

* Real-time object detection in games
* AR/VR interaction systems
* Pose-based gameplay mechanics
* AI-powered visualization tools
* Image & video analysis applications
* Rapid prototyping of computer vision features in Unity

---

## 🎬 Demo Video

📺 Watch here:
[https://www.youtube.com/watch?v=E8GOZr2n9fY](https://www.youtube.com/watch?v=E8GOZr2n9fY)

---

## 🛒 Unity Asset Store

Get the full package here:

👉 [https://assetstore.unity.com/packages/tools/ai-ml-integration/yolomodelrunner-353736](https://assetstore.unity.com/packages/tools/ai-ml-integration/yolomodelrunner-353736)

---

## 📬 Support

Need help or want to request features?

* 📧 Email: [realmoctopus@gmail.com](mailto:realmoctopus@gmail.com)
* 🛍 Unity Asset Store: Contact via the asset’s official page

---

## ⭐ If This Project Helps You

If you find YoloModelRunnerTemplate useful, consider leaving a review on the Unity Asset Store.
It helps support future updates and improvements.

---

**Build powerful computer vision systems in Unity — without the complexity.**
