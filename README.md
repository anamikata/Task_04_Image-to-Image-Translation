# TASK_04 – Image-to-Image Translation using Pix2Pix cGAN

## 📌 Overview

This project implements an **Image-to-Image Translation model** using **Pix2Pix**, a Conditional Generative Adversarial Network (cGAN). The model learns a mapping between an input image and a target image, enabling automatic image transformation tasks such as converting architectural labels into realistic building facades.

Developed as part of **Task-04** of the **Machine Learning Internship Program at Prodigy InfoTech**.

---

## 🎯 Objective

To implement and train a **Pix2Pix Conditional GAN** capable of translating input images into corresponding target images using paired image datasets.

---

## 🧠 About Pix2Pix

Pix2Pix is a supervised image-to-image translation framework that combines:

* **Generator (U-Net Architecture)** for image generation
* **Discriminator (PatchGAN)** for distinguishing real and generated images
* **Adversarial Loss** for realism
* **L1 Loss** for preserving structural similarity

Together, these components enable the model to generate realistic output images from given inputs.

---

## 📂 Dataset

### Facades Dataset

The Facades dataset contains paired images where:

* Left Half → Architectural Label Map
* Right Half → Real Building Facade

The model learns to translate label maps into realistic building images.

---

## ⚙️ Technologies Used

* Python
* PyTorch
* Google Colab
* NumPy
* Matplotlib
* GANs (Generative Adversarial Networks)
* Pix2Pix (Conditional GAN)

---

## 🏗️ Model Architecture

### Generator

* U-Net Encoder–Decoder Architecture
* Generates realistic facade images from input label maps

### Discriminator

* PatchGAN Discriminator
* Evaluates local image patches for realism
* Improves texture and image quality

---

## 🚀 Workflow

1. Download and load the Facades dataset.
2. Split paired images into input and target images.
3. Apply preprocessing and normalization.
4. Train Generator and Discriminator simultaneously.
5. Compute Adversarial Loss and L1 Loss.
6. Generate translated images.
7. Evaluate output quality.

---

## 📊 Results

The Pix2Pix model successfully learns the mapping between architectural labels and real building facades.

### Sample Output

Input Label Map → Generated Facade → Ground Truth Facade

The generated outputs preserve structural information while producing visually realistic textures and details.

---

## 📁 Project Structure

```text
PRODIGY_ML_04/
│
├── Pix2Pix_Task4.ipynb
├── README.md
├── requirements.txt
├── outputs/
│   ├── result1.png
│   ├── result2.png
│   └── result3.png
│
├── models/
│   └── pix2pix_generator.pth
│
└── dataset/
```

---

## ▶️ How to Run

### Clone Repository

```bash
git clone https://github.com/yourusername/PRODIGY_ML_04.git
cd PRODIGY_ML_04
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Run Notebook

Open `Pix2Pix_Task4.ipynb` in Google Colab or Jupyter Notebook and execute all cells.

---

## 📈 Learning Outcomes

* Understanding Conditional GANs (cGANs)
* Working with Pix2Pix Architecture
* Implementing U-Net Generators
* Using PatchGAN Discriminators
* Adversarial Training Techniques
* Image-to-Image Translation
* Deep Learning with PyTorch

---

## 🎓 Internship Details

**Internship:** Machine Learning Internship

**Task:** Task-04 – Image-to-Image Translation using Pix2Pix cGAN

---

## 👩‍💻 Author

Anamika T A

AI Intern

Prodigy InfoTech

---

## ⭐ Acknowledgement

I would like to thank Prodigy InfoTech for providing practical machine learning projects that enhanced my understanding of deep learning, GANs, and image-to-image translation techniques.
