# 🧑‍💻 Face Identification using Siamese Network
---
### 📌 Overview

This project implements a Face Identification System using a Siamese Network architecture.
Instead of traditional classification, the model focuses on verifying similarity between two faces.

👉 The system compares a captured input image against 30 verification images, and grants access if the similarity passes predefined detection and verification thresholds.

---
### 🤔 What is a Siamese Network?

A Siamese Network is a neural network that learns to measure similarity between two inputs.

Each input is passed through identical subnetworks that produce embeddings.

A distance metric (e.g., Euclidean / Cosine) is used to determine similarity.

✅ This makes it ideal for verification tasks like authentication, signature verification, or one-shot learning.

🔒 Real-World Example: Smartphone Face Unlock

Your face is compared with stored embeddings (not classified).

Provides faster & more secure verification compared to traditional classification.

---

### ✨ Features

✅ Real-time webcam verification

✅ Siamese Network model for image similarity

✅ Adjustable thresholds for sensitivity control

✅ Easy dataset management with negative sampling

✅ Lightweight and portable for real-world use cases

---

### 📂 Dataset

We use the Labeled Faces in the Wild (LFW) dataset.

📌 Negative Images (different identities) are crucial:

Train the model to recognize differences as well as similarities

Prevent false positives (e.g., random person unlocking a device)

Improve reliability & robustness

---

### ⚙️ Installation

Clone the repository and install dependencies:

git clone https://github.com/Hariprasadkurra/FACE_VERIFICATION/

cd FACE_VERIFICATION

pip install -r requirements.txt


---

### requirements.txt

numpy

pandas

matplotlib

opencv-python

scikit-learn

tensorflow>=2.9

keras

tqdm

---

### 🎥 Webcam Controls

Press v → Capture image & run verification

Press q → Quit

---

### 🔍 Verification Process

Captured image is saved as input_image.jpg

Compared against 30 verification images in /verification_images

Siamese Network outputs similarity score

If score ≥ threshold → ✅ Verified
Else → ❌ Not Verified

---

### 📁 Project Structure

📂 Project Root

├── 📄 main.ipynb                  # Main verification script

├── 📄 requirements.txt         # Dependencies list

├── 📄 README.md                # Project documentation

└── 📂 model/                   # Trained model storage
    |
    └── siamesemodelv1          # Siamese network weights

    
---

### 📜 License

This project is licensed under the MIT License – see the LICENSE file for details.

---

### 🤝 Contributing

Contributions are welcome! 🎉

Fork the repo

Create a new branch (feature/my-feature)

Commit changes & open a PR
