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
```

### 2. Create Virtual Environment & Install Dependencies

```bash
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
pip install -r requirements.txt
```



### 3. Start Backend(FastAPI)
```bash
uvicorn app:app --reload
```

### 4. Start Frontend(Streamlit)
```bash
streamlit run frontend.py
```


### 💡Features Used in Model
1. bmi (calculated)
2. age_grouped
3. lifestyle_risk
4. city_tier
5. income_lpa
6. occupation


### 📁Project Structure
```bash
insurance-premium-predictor/
├── app.py             # FastAPI backend for prediction API
├── frontend.py        # Streamlit UI to interact with the API
├── model.pkl          # Trained machine learning model (pickled)
├── requirements.txt   # List of required Python packages
├── README.md          # Project documentation (this file)
├── .gitignore         # Files/folders to ignore in Git
```

### 🧠 Future Enhancements
* Add login/authentication system
* Deploy to cloud (Render, AWS, etc.)
* Add Jupyter notebook for model training
* Improve UI/UX using HTML/CSS components


### 🙌 Contributing
Pull requests are welcome! Open issues for feature ideas or bug reports.
