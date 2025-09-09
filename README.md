# Multi-Disease Prediction System 🏥

A unified AI system to predict multiple diseases using tabular medical data and chest X-ray images.  
<img width="1915" height="929" alt="Screenshot 2025-09-09 203320" src="https://github.com/user-attachments/assets/371ed6e8-3c70-4995-98f6-6e30ed0269b8" />


- **Diabetes, Heart Disease, Chronic Kidney Disease (CKD)** – Predicted using **Artificial Neural Networks (ANN)**  
- **Pneumonia** – Predicted using **Convolutional Neural Networks (CNN)**  
<img width="1915" height="906" alt="Screenshot 2025-09-09 213032" src="https://github.com/user-attachments/assets/84258b39-cf3a-4cf2-ba52-0233baa72c14" />

Built with **Gradio** for an interactive and user-friendly interface.

---

## Features

- Predict multiple diseases from a single interface  
- Supports tabular medical data and image-based data  
- Quick and accurate predictions without requiring medical expertise  

---

## How It Works

1. **Data Collection**
   - Tabular datasets (CSV) for Diabetes, Heart, CKD  
   - Chest X-ray images for Pneumonia  

2. **Data Preprocessing**
   - **Tabular Data (ANN)**: Handle missing values, encode categorical features, scale values, split into train/test  
   - **Image Data (CNN)**: Resize images, normalize pixel values, optional data augmentation  

3. **Model Design**
   - **ANN**: Input → Hidden layers → Output (sigmoid)  
   - **CNN**: Convolution + Pooling → Flatten → Dense → Output (sigmoid)  

4. **Model Training**
   - Train ANN on tabular datasets  
   - Train CNN on Pneumonia images  
   - Evaluate performance using accuracy, precision, recall, and F1-score  

5. **Gradio Interface**
   - Dropdown menu to select disease  
   - Input fields for tabular data or file upload for X-ray  
   - Submit → Preprocessing → Model predicts → Result displayed  

---

## Installation

1. Clone this repository:

```bash
git clone https://github.com/your-username/multi-disease-prediction.git
cd multi-disease-prediction
Install dependencies:

pip install -r requirements.txt


Dependencies include: TensorFlow, scikit-learn, pandas, numpy, matplotlib, Gradio

Usage

Run the app:

python app.py


Open the Gradio interface in your browser

Select the disease and enter medical data or upload a chest X-ray image

Click Submit to get prediction results

Datasets

Diabetes: Features like Glucose, Blood Pressure, BMI, Age, etc.

Heart Disease: Features like Age, Sex, Cholesterol, Resting BP, Max Heart Rate, etc.

CKD: Lab tests and categorical features (Blood Pressure, Hemoglobin, Creatinine, etc.)

Pneumonia: Chest X-ray images labeled Pneumonia or Normal

Results

ANN achieves high accuracy for Diabetes, Heart Disease, CKD prediction

CNN accurately classifies Pneumonia from chest X-rays

Single system integrates both tabular and image-based predictions
