# Hyperspectral Band Selection Using Attention-Based CNNs

This repository implements **Hyperspectral Band Selection** using **Attention-Based Convolutional Neural Networks (CNNs)**.  
The project is based on the concept of **identifying the most informative spectral bands** from hyperspectral images (HSI) while maintaining high classification accuracy.

---

## **Overview**

- **Hyperspectral Imaging (HSI)** captures images with hundreds of narrow spectral bands, resulting in high-dimensional data.
- Many bands are redundant or noisy, which:
  - Increases computational costs.
  - Decreases classification performance if irrelevant data is included.
- This project leverages:
  - **1D CNNs** to learn spectral features.
  - **Attention modules** to automatically score the importance of each band.
  - **Anomaly detection (Elliptic Envelope)** to select the top informative bands.
  
The model is evaluated on the **Different hyperspectral dataset**, achieving state-of-the-art classification performance with reduced spectral dimensions.

---

## **Key Features**
- Attention-based band importance estimation.
- Band selection using anomaly detection (EllipticEnvelope).
- Multiple CNN architectures (`Model2`, `Model3`, `Model4`) with 2–4 attention modules.
- Training and evaluation pipeline with visualization of:
  - **Training vs Validation Loss**
  - **Training vs Validation Accuracy**

---

## **Project Structure**
.
├── arguments.py # Argument definitions
├── generate_datasets.py # Data loading and preprocessing
├── model_2.py # CNN with 2 attention modules
├── model_3.py # CNN with 3 attention modules
├── model_4.py # CNN with 4 attention modules
├── training_attention.py # Main training and evaluation script
├── output/ # Output directory for models, plots, and metrics
└── README.md

##  Future Work
Add support for more hyperspectral datasets.

Experiment with Transformer-based models for band selection.

Extend to segmentation tasks.

## References
Hyperspectral Band Selection Using Attention-Based Convolutional Neural Networks (research paper).

Pavia University Dataset (Remote Sensing Lab, University of Pavia).

