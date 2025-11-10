# 🧠 Handwritten Digit Recognition using CNN (Live Camera)

## 📖 Overview
This project implements a **Convolutional Neural Network (CNN)** model to recognize **handwritten digits (0–9)** using the MNIST dataset.  
It also includes a **live camera feature** that captures an image using your webcam in **Google Colab**, detects multiple digits, and predicts the full number in real time.

---

## ⚙️ Environment
This project is designed to run entirely in **Google Colab**.  
All required packages (TensorFlow, OpenCV, Matplotlib, NumPy) are installed automatically within the notebook using `!pip install` commands — **no external setup or local installation** is needed.

---

## 🚀 How to Run the Project

1. **Open Google Colab**  
   Visit [https://colab.research.google.com](https://colab.research.google.com)

2. **Upload the notebook file**  
   - Click on **File → Upload notebook**
   - Select the file:  
     ```
     live_digit_recognition.ipynb
     ```

3. **Run all cells sequentially**  
   - The first cell automatically installs required packages:
     ```bash
     !pip install tensorflow opencv-python matplotlib
     ```
   - Then, the model will be trained on the MNIST dataset.
   - Finally, the notebook will activate the webcam for digit recognition.

4. **Capture a handwritten number**
   - When prompted, click **“Capture”** to take a live photo of your handwritten digits (e.g., written on paper and shown to the webcam).

5. **View Predictions**
   - The model will automatically detect digits in the image,
   - Predict each digit individually,
   - Display the recognized number with bounding boxes.

---

## 🧠 Model Summary
- **Dataset:** MNIST (70,000 handwritten digits)
- **Model:** Sequential CNN  
  - Conv2D (32 filters, 3×3) + ReLU  
  - MaxPooling2D  
  - Conv2D (64 filters, 3×3) + ReLU  
  - MaxPooling2D  
  - Flatten + Dense(128, ReLU)  
  - Output: Dense(10, Softmax)
- **Optimizer:** Adam  
- **Loss Function:** Sparse Categorical Crossentropy  
- **Accuracy:** ~99% on test data

---

## 🧩 Files Included
```
Handwritten-Digit-Recognition/
│
├── live_digit_recognition.ipynb   # Main Colab notebook with full code
└── README.md                      # Project overview and usage instructions
```

---

## 👨‍💻 Author
**Anchit Patil**  
TYCSE AIES Mini Project – 2025  
Project Title: *Handwritten Digit Recognition using CNN (Live Camera)*
