# GAN-MNIST

UNet-Inspired GAN for Denoising and Classifying a Custom MNIST Dataset

This repository demonstrates how to use a UNet-inspired GAN (Generative Adversarial Network) to denoise images and then classify them on a custom MNIST dataset. The idea is to remove noise from MNIST-like digits using a generator with a UNet structure, then feed the denoised images into a classifier for improved accuracy.

⸻

Overview
	1.	Denoising with a UNet-inspired Generator
	•	The generator is designed with an encoder-decoder architecture similar to UNet. Skip connections help preserve spatial information, which is crucial in denoising tasks.
	2.	GAN Setup
	•	The Discriminator is a CNN-based network that distinguishes real (clean) MNIST images from generated (denoised) images.
	•	The Generator outputs denoised images that (hopefully) resemble clean MNIST digits.
	3.	Classification
	•	After denoising, a simple classifier (e.g., a CNN) is trained on the clean MNIST set and tested on denoised outputs to measure accuracy improvements over noisy inputs.

⸻

Data
	1.	Custom MNIST Dataset
	•	The dataset includes MNIST images with added noise (train.pkl).
	2.	Transforms
	•	Optional transforms (e.g., normalization, random cropping) can be applied.

<img width="873" alt="Screenshot 2025-04-08 at 3 42 11 PM" src="https://github.com/user-attachments/assets/d693ad8f-ad42-4622-ba9d-7e874e8e6e54" />
