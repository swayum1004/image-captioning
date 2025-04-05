🖼️ **Image Captioning with Attention and InceptionResNetV2**

This repository implements an Image Captioning model using deep learning techniques. The model combines the power of transfer learning with a sequence-to-sequence architecture featuring GRU and attention mechanisms to generate descriptive captions for images.

📌 **Overview**

**Encoder**: Uses the pre-trained InceptionResNetV2 model to extract rich visual features from images.

**Decoder**: A custom RNN decoder with GRU, attention mechanism, and embedding layers to generate captions based on image features.

**Dataset:** Trained on the COCO Captions dataset, which contains a wide range of images paired with human-written captions.

**Goal:** Given a new image, the model generates a meaningful and relevant caption.

🧠 **Key Features**

✅ Transfer Learning with InceptionResNetV2 for efficient image feature extraction.

✅ Attention Mechanism to dynamically focus on important regions of the image while generating each word.

✅ Custom Training Loop with teacher forcing and loss masking.

✅ Prediction Pipeline to generate captions for new, unseen images.

✅ Built using TensorFlow and Keras.

🛠️ **Workflow**

**Import Libraries:** TensorFlow, TensorFlow Datasets, TensorFlow Hub, Matplotlib, etc.

**Set Parameters:** Define vocabulary size, embedding dimensions, attention units, etc.

**Load & Preprocess Data:** Load COCO dataset, resize/normalize images, tokenize captions with <start> and <end> tokens.

**Encoder:** Extract features using InceptionResNetV2 and pass through a dense layer.

**Decoder:** Generate captions using GRU, attention, and dense layers.

**Training:** Optimize the model using SparseCategoricalCrossentropy and AdamW.

**Prediction**: Generate captions for input images with a separate inference model.


📁 **Dataset**

COCO Captions: https://cocodataset.org/#captions-2015

Loaded via TensorFlow Datasets or from Google Cloud Storage.

⚙️ **Technologies Used**

Python

TensorFlow 2.x

Keras

TensorFlow Datasets

NumPy, Matplotlib
