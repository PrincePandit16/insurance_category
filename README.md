# 🛡️ Insurance Premium Category Predictor

A complete **machine learning web application** using **FastAPI (backend)** and **Streamlit (frontend)** that predicts the **insurance premium category** of a person based on age, weight, height, income, occupation, city, and smoking habits.

---

## 🚀 Demo

- Run FastAPI backend  
- Launch Streamlit frontend  
- Enter details and get your premium category predicted!

---

## 📦 Tech Stack

| Layer         | Technology     |
|--------------|----------------|
| Backend API  | FastAPI        |
| Frontend UI  | Streamlit      |
| Model        | Scikit-learn (Pickle) |
| Data Handling| Pandas         |
| Validation   | Pydantic       |

---

## ✅ Features

### 🔍 Frontend (Streamlit)

- Simple form for user input  
- Validated fields (age, height, weight, etc.)  
- Dropdowns and checkboxes for easy input  
- Real-time API call and prediction  
- Handles errors like server disconnection  

### ⚙️ Backend (FastAPI)

- Typed data input using Pydantic  
- Computes:  
  - **BMI** = weight / height²  
  - **Lifestyle risk** (based on BMI & smoking)  
  - **Age group** (young, adult, middle_aged, senior)  
  - **City tier** (1 for metro, 2 for semi-metro, 3 for others)  
- Uses a trained ML model to predict premium category  
- JSON response with status codes  

---

## 📥 How to Run Locally

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/insurance-premium-predictor.git
cd insurance-premium-predictor


