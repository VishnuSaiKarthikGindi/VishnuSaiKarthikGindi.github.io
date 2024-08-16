---
title: "Anomaly Detection in Medical Imagery"
excerpt: "Developed an anomaly detection system using autoencoders to identify anomalies in medical images using autoencoders and <br/><img src='/images/ADMI.png'>"
collection: portfolio
---

**Project Overview:**
This project focuses on developing a deep learning model to identify anomalies in images, particularly in the medical domains. The model utilizes autoencoders, a type of neural network, to learn the underlying patterns in normal data and detect anomalies as deviations from this learned representation.

The project utilized the MURA dataset for medical imaging, which includes musculoskeletal radiographs and Brain MRI imagery. The data was preprocessed by resizing images to a uniform size of 256x256 pixels and normalizing pixel values. Grayscale images were used for medical data.

**Model Development:**
The autoencoder model was built with an encoder-decoder architecture. The encoder compresses the input images into a lower-dimensional latent space, capturing essential features. The decoder reconstructs the image from this latent representation. The model was trained to minimize the reconstruction error on normal data. Anomalies were detected by setting a threshold on the reconstruction error—images with errors above the threshold were flagged as anomalies.

The developed model demonstrated a high detection accuracy, with the ability to correctly identify over 95% of anomalies in the test datasets. The model's effectiveness was quantified by evaluating its performance on a held-out validation set, showing a significant improvement over traditional methods with a reduction in false positives and false negatives.

For more detailed information and to view the code, visit the [GitHub repository](https://github.com/yourusername/Anomaly-Detection-Autoencoders).