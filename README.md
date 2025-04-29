# Predicting Clear Images from Blurred Inputs using pix2pix and CycleGAN

This repository contains notebooks and code demonstrating how to restore clear images from blurred inputs using **pix2pix** and **CycleGAN** architectures, applied to the FMNIST and MNIST datasets.

Inspired by the [TensorFlow CycleGAN tutorial](https://www.tensorflow.org/tutorials/generative/cyclegan), this project explores the application of image-to-image translation models for image deblurring in a supervised (pix2pix) and unpaired (CycleGAN) setting.

## Datasets

We experiment on:
- **MNIST** – Handwritten digits.
- **FMNIST (Fashion-MNIST)** – Fashion product images from Zalando.
- **Blurred versions** of FMNIST created by applying Gaussian blur.

## Notebooks

- `MNIST Dataset of pix2pix cycleGAN.ipynb`: pix2pix and/or CycleGAN applied to MNIST.
- `FMNIST Dataset of pix2pix cycleGAN.ipynb`: Image-to-image translation models on FMNIST.
- `Blur of FMNIST Dataset of pix2pix cycleGAN.ipynb`: Training on blurred-to-clear FMNIST image pairs.

## Goals

- Learn mappings from **blurred** to **clear** images using paired data (pix2pix).
- Investigate whether CycleGAN can perform deblurring in **unpaired** settings.
- Compare performance of both models across datasets.

## Results

- Pix2pix successfully reconstructs clean images from blurred FMNIST inputs in a supervised setting.
- CycleGAN can learn meaningful transformations with unpaired training data, though with lower fidelity.

## Requirements

- Python 3.x
- TensorFlow 2.x
- Matplotlib, NumPy
- (Optional) GPU for faster training

Install dependencies:
```bash
pip install tensorflow matplotlib numpy
```

## Acknowledgments

- Based on [TensorFlow's CycleGAN tutorial](https://www.tensorflow.org/tutorials/generative/cyclegan).
- Datasets from [TensorFlow Datasets](https://www.tensorflow.org/datasets).
