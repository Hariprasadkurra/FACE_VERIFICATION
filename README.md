
# Face Identification using Siamese Network


## overview

This project implements a face identification system using a **Siamese Network**. The system verifies a user's identity by comparing a single input image against a set of 30 verification images. If the similarity score meets the specified detection and verification thresholds, the user is verified.
### what is Siamese Network
A Siamese Network is a type of neural network that learns to compare two inputs by computing their feature embeddings and measuring their similarity using a distance metric.
### Daliy life use case:
**Smartphone Face Unlock** (Biometric Authentication)
Used in Android face unlock systems.

Compares the user's face with stored facial features for secure authentication 

## Installation
pip install tensorflow numpy opencv-python os

## Usage
1. Run the verification script:

python main.py

2. Using the webcam:

Press v to capture an image and verify.

Press q to quit the application.

3. Verification Process:

Captured image is saved as input_image.jpg.

The model compares it with 30 verification images.

4. If the similarity score meets the threshold, verification succeeds.

Displays True if verified, else False.

### Dataset Link
https://www.kaggle.com/datasets/atulanandjha/lfwpeople

This above link is for **Negative** images
#### Why
Negative images help the **Siamese Network** differentiate between genuine and impostor faces. They improve the model’s **discriminative ability** by ensuring it learns both similarities and differences. This reduces **false positives**, preventing unauthorized users from being verified. Negative samples also **mimic real-world scenarios**, making verification systems more reliable. Finally, they help set an **optimal threshold** for accurate authentication. 🚀

