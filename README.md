# Image Caption Generator
## Introduction
Image caption generation is a task in the field of artificial intelligence and computer vision where a machine generates a textual description of an image. This project aims to build an image caption generator using a combination of a pre-trained VGG19 model for feature extraction and a Long Short-Term Memory (LSTM) network for sentence generation.

The VGG19 model, renowned for its deep convolutional layers, is well-suited for extracting meaningful features from images. These features are then passed to the LSTM, which generates coherent sentences based on the visual information from the image.

---

## Approach
The image caption generator is designed using a two-part model:

VGG19 Model: Used to extract features from an input image.
LSTM Model: Generates a caption based on the image features provided by VGG19.

---

## Inference
During inference (when generating captions for a new image), the LSTM is fed the start token and the image features. It predicts the next word, and the process is repeated with the predicted word as input until the end token is generated. This process is called greedy search, where the word with the highest probability is selected at each time step.

---
## Model
![img1](https://github.com/SwamySaxena/image_caption_generator/blob/main/image1.jpg)

---
## Sample Output
![img2](https://github.com/SwamySaxena/image_caption_generator/blob/main/dog.jpg)
![img3](https://github.com/SwamySaxena/image_caption_generator/blob/main/image2.jpeg)
---
