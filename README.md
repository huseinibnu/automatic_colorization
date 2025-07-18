# Automatic Colorization of Landscape Images Using Deep Learning

This project implements a deep learning approach to automatically colorize grayscale landscape images using a U-Net autoencoder with a VGG16 encoder backbone. The model is trained on paired grayscale-color images and optimized with a perceptual + contrastive + SSIM loss function.

---

## Features

- ✅ Grayscale to RGB colorization
- ✅ U-Net architecture with VGG16 encoder
- ✅ Custom perceptual + contrastive + chroma-weighted loss
- ✅ Evaluation with SSIM and PSNR
- ✅ Visualization of predicted vs ground-truth images

---

## Model Overview

The model follows the U-Net architecture:
- **Encoder:** Pretrained VGG16 (ImageNet), partially fine-tuned
- **Decoder:** Transposed convolutions with skip connections
- **Loss:** Combined perceptual, pixel-wise, SSIM, contrastive, and chroma-weighted loss

---

## Sample Results

<table> 
  <tr> <th>Grayscale Input</th> <th>Model Output</th> <th>Ground Truth</th> </tr> 
  <tr> 
    <td><img width="250" alt="grayscale1" src="https://github.com/user-attachments/assets/fe80115a-7912-48f3-9d86-535f4348270c" /></td> 
    <td><img width="250" alt="predicted1" src="https://github.com/user-attachments/assets/def876fa-b17f-4b28-8b53-2bc2c53e1c6f" /></td> 
    <td><img width="250" alt="groundtruth1" src="https://github.com/user-attachments/assets/5c839125-0a3c-4b6a-b3a4-24f31c707269" /></td> 
  </tr> 
  <tr> 
    <td><img width="250" alt="grayscale2" src="https://github.com/user-attachments/assets/b331e1f4-d97f-4f83-802a-e28f78876646" /></td> 
    <td><img width="250" alt="predicted2" src="https://github.com/user-attachments/assets/8bae232b-fab3-4d0d-8f4a-3d1e4cda0dc9" /></td> 
    <td><img width="250" alt="groundtruth2" src="https://github.com/user-attachments/assets/f152943d-92c0-41f3-b07a-ffd09a517da2" /></td> 
  </tr> 
  <tr> 
    <td><img width="250" alt="grayscale3" src="https://github.com/user-attachments/assets/7b9923e4-ee06-4278-9bc3-c14aedc42bb9" /></td> 
    <td><img width="250" alt="predicted3" src="https://github.com/user-attachments/assets/d3c34e13-04f1-4984-ac45-1546b507f31d" /></td> 
    <td><img width="250" alt="groundtruth3" src="https://github.com/user-attachments/assets/6542dc96-cb36-46e9-b48a-62c0f2fc1586" /></td> 
  </tr> 
</table>







---

