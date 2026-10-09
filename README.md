<div align="center">

# 🔎 Real-Time Image Recognition with ResNet152

**Classify whatever your webcam sees using a pre-trained ResNet152 (ImageNet) in a few lines of Keras.**

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?logo=tensorflow&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?logo=opencv&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?logo=jupyter&logoColor=white)

</div>

---

## ✨ How it works

`ResnetPretrained.ipynb`:

1. 📦 Loads **ResNet152** with ImageNet weights from `tensorflow.keras.applications` and prints the model summary.
2. 📷 Opens the webcam with OpenCV and, for every frame, resizes it to 224 × 224, converts BGR → RGB and applies `preprocess_input`.
3. 🏷️ Runs `model.predict` and decodes the top ImageNet class with `decode_predictions`, showing it on the live video.

No training is needed - the model recognises the 1 000 ImageNet categories out of the box.

## 🚀 Getting Started

```bash
git clone https://github.com/Arashomranpour/image-recognition-resnet.git
cd image-recognition-resnet
pip install tensorflow opencv-python numpy jupyter
jupyter notebook ResnetPretrained.ipynb
```

The ResNet152 weights (~230 MB) download automatically on first run. Press **Q** in the video window to quit.

## 📁 Project Structure

```
.
└── ResnetPretrained.ipynb
```

## 🛠️ Tech Stack

`TensorFlow / Keras (ResNet152)` · `OpenCV` · `NumPy`
