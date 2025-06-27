# Image_colorizer
AI-powered image colorization — Transform black and white images into vibrant colored photos using deep learning!

This project implements a **U-Net based neural network** that automatically adds realistic colors to grayscale images.

---

## ✨ Features

- 🚀 **Advanced U-Net Architecture** with skip connections for high-quality results  
- 🖥️ **Multiple Interface Options**: Command-line, interactive script, and a Streamlit web app  
- 🗂️ **Batch Processing** support for multiple images  
- 📈 **Real-time Visualization** of training progress  
- 🧪 **Optimized Training** with augmentation, learning rate scheduling & validation monitoring  

---

## 🚀 Quick Start

### 🏋️‍♀️ Training the Model
```bash python train_colorization.py ```

---
## Web Interface
``` bash streamlit run colorize_web_app.py ```
## 📋 Requirements

- Python 3.7+
- PyTorch
- torchvision
- PIL/Pillow
- matplotlib
- numpy
- tqdm
- streamlit (for web interface)

## 🏗️ Architecture
The model uses a U-Net architecture with:
- Encoder-Decoder structure with skip connections
- Batch normalization for stable training
- Perceptual loss combining MSE and L1 loss
- Data augmentation for better generalization

## 📊 Results
The model achieves excellent colorization results on various image types:
- Natural scenes and landscapes
- Portraits and people
- Objects and still life
- Architecture and buildings

## 🔧 Technical Details
- Dataset: Trained on CIFAR-10 (expandable to custom datasets)
- Input: Grayscale images (any size)
- Output: RGB colorized images
- Training Time: ~2-3 hours on GPU
- Inference Time: <1 second per image
