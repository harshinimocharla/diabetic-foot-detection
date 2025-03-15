# diabetic-foot-detection
# Diabetic Foot Detection using ResNet50

## 📌 Project Overview
A deep learning-based system to detect diabetic foot conditions from thermal images using the ResNet50 architecture. The goal is to achieve **99% accuracy** through fine-tuned transfer learning and robust preprocessing.

---

## 🗂️ Project Structure
```
Diabetic_Foot_Detection/
│── data/
│   ├── diabetic_dataset/
│   ├── non_diabetic_dataset/
│   ├── processed/
│   ├── split_data/
│
│── notebooks/
│   ├── 01_exploratory_analysis.ipynb
│   ├── 02_preprocessing.ipynb
│   ├── 03_model_training.ipynb
│   ├── 04_evaluation.ipynb
│
│── src/
│   ├── data_loader.py
│   ├── model.py
│   ├── train.py
│   ├── evaluate.py
│   ├── inference.py
│   ├── utils.py
│
│── models/
│   ├── best_model.h5
│   ├── latest_model.h5
│
│── reports/
│   ├── figures/
│   ├── results.txt
│
│── deployment/
│   ├── app.py
│
│── requirements.txt
│── README.md
│── .gitignore
```

---

## ✅ Key Steps
1. **Data Preprocessing:** Augmentation and normalization of thermal images.
2. **Data Splitting:** 70% train, 20% validation, 10% test.
3. **Model Building:** ResNet50 with fine-tuning and custom classification head.
4. **Model Training:** Class weights handling and early stopping.
5. **Model Evaluation:** Accuracy, loss, and confusion matrix analysis.
6. **Model Inference:** Predict diabetic status from new images.
7. **Streamlit Deployment:** User-friendly web interface.

---

## 🖥️ Run the Project

### 1️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

### 2️⃣ Data Preprocessing
```bash
python src/data_preprocessing.py
```

### 3️⃣ Data Splitting
```bash
python src/data_splitting.py
```

### 4️⃣ Model Training
```bash
python src/model_training.py
```

### 5️⃣ Model Evaluation
```bash
python src/model_evaluation.py
```

### 6️⃣ Run the Streamlit App
```bash
streamlit run deployment/app.py
```

### 7️⃣ Model Inference
Upload a thermal foot image to get a **Diabetic** or **Non-Diabetic** prediction.

---

## 🎯 Results
Achieved **99% accuracy** with:
- ResNet50 fine-tuning
- Class balancing
- Robust data augmentation

---

## 📌 Future Work
- Real-time monitoring with live thermal camera feeds
- Extending to other diabetic complications like ulcers

---

## 💡 Contributors
- [Your Name]

---

