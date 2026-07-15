# MEDICAL-IMAGE-CLASSIFIER

# MRI Image Denoising using Conditional GAN

A deep learning-based MRI image denoising system built using a Pix2Pix-style Conditional GAN. The model employs a U-Net generator and a PatchGAN discriminator to restore noisy brain MRI scans while preserving structural details.

## Features

- Pix2Pix-style Conditional GAN architecture
- U-Net generator with skip connections
- PatchGAN discriminator
- Synthetic Gaussian noise generation for supervised training
- Evaluation using PSNR and SSIM
- Trained on Brain MRI Images for Brain Tumor Detection dataset

## Results

| Metric | Score |
|--------|------:|
| PSNR | **27.39 dB** |
| SSIM | **0.8089** |

## Tech Stack

- Python
- PyTorch
- Torchvision
- NumPy
- Matplotlib
- Scikit-image

## Project Structure

```
├── notebooks/
├── models/
├── requirements.txt
├── medical_classifier.py
└── README.md
```

## Installation

```bash
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>
pip install -r requirements.txt
```

## Dataset

Brain MRI Images for Brain Tumor Detection (Kaggle)

## Future Improvements

- Support real MRI noise (Rician noise)
- Train on larger datasets (BraTS, IXI)
- 3D volumetric MRI denoising
- Deploy on Hugging Face Spaces

## License

MIT License
