# Predicting Clear Images from Blurred Inputs using pix2pix and CycleGAN

This repository contains notebooks and code demonstrating how to restore clear images from blurred inputs using **pix2pix** and **CycleGAN** architectures, applied to the FMNIST and MNIST datasets.

Inspired by the [TensorFlow CycleGAN tutorial](https://www.tensorflow.org/tutorials/generative/cyclegan), this project explores the application of image-to-image translation models for image deblurring in a supervised (pix2pix) and unpaired (CycleGAN) setting.

## Datasets

We experiment on:
- **MNIST** – Handwritten digits.
- **FMNIST (Fashion-MNIST)** – Fashion product images from Zalando.
- **Blurred versions** of FMNIST created by applying Gaussian blur.

## Notebooks

- `MNIST Dataset of pix2pix cycleGAN.ipynb`: pix2pix and CycleGAN applied to MNIST.
- `FMNIST Dataset of pix2pix cycleGAN.ipynb`: pix2pix and CycleGAN applied to FMNIST.
- `Blur of FMNIST Dataset of pix2pix cycleGAN.ipynb`: Evaluated robustness on Gaussian blurred FMNIST.

## Goals

- Learn mappings from **blurred** to **clear** images.
- Compare performance models across datasets.

## Results

- Pix2pix-CycleGAN successfully reconstructs clean images from blur photo inputs to their original images for MNIST, FMNIST, blurred FMNIST in a supervised setting.

## Requirements

- Python 3.x
- TensorFlow 2.x
- Matplotlib, NumPy
- (Optional) GPU for faster training

## Acknowledgments

- Based on [TensorFlow's CycleGAN tutorial](https://www.tensorflow.org/tutorials/generative/cyclegan).
- Datasets from [TensorFlow Datasets](https://www.tensorflow.org/datasets) and photos we take.
