# Multiple Disease Prediction System (Streamlit App)

This is a **Multiple Disease Prediction System** built with **Streamlit**, showcasing a **Diabetes Prediction using Machine Learning** model and expandable to include other diseases like heart disease and Parkinson's.

##  Live Demo

Check out the live deployed version here:  
[iamdharma-disease-app.streamlit.app](https://iamdharma-disease-app.streamlit.app/)  
*(Directs to the "Diabetes Prediction using ML" section)*

---

##  Features

- **User-friendly Interface**: Built with Streamlit for interactive, easy-to-use UI.
- **Diabetes Prediction with ML**:
  - Uploads sample data or inputs manually.
  - Runs a trained model (`diabetes_model.sav`) to predict whether a patient has diabetes.
- **Expandable Architecture**: Designed to support more disease prediction modules (e.g., heart disease, Parkinson's).
- **Model Persistence**: Uses `pickle` to load pre-trained machine learning models.
- **Optional Backend Support**: Can integrate MySQL to persist user predictions and history.

---

##  Project Structure

multiple-disease-prediction-app/
│
├── app.py # Main Streamlit application
├── requirements.txt # Project dependencies
├── runtime.txt # Python version lock for hosting
├── saved_models/
│ └── diabetes_model.sav # Pre-trained model file
│
├── README.md # Overview & instructions (this file)
└── ... # (Optional) Additional disease modules

yaml
Copy code

---

##  Getting Started

### Prerequisites

- Python 3.12 (recommended – especially for Streamlit Cloud deployments)
- pip (Python package manager)

### Installation

1. **Clone the repository**  
   ```bash
   git clone https://github.com/IAMDHARMA/-Multiple-Disease-Prediction-System.git
   cd -Multiple-Disease-Prediction-System
(Optional) Create and activate a Python virtual environment

bash
Copy code
python -m venv venv
source venv/bin/activate   # On macOS/Linux
venv\Scripts\activate      # On Windows
Install dependencies

bash
Copy code
pip install -r requirements.txt
Run the app locally

bash
Copy code
streamlit run app.py
Deployment on Streamlit Cloud
Ensure runtime.txt exists with:

Copy code
python-3.12.4
Commit changes and push your repo to GitHub.

In Streamlit Cloud:

Create a new app from your GitHub repo.

Ensure dependencies in requirements.txt are satisfied.

Deploy — the app will auto-launch.

(Optional) If using MySQL, place credentials in Streamlit Secrets (don’t hard-code):

toml
Copy code
[mysql]
host = "your_host"
user = "your_user"
password = "your_pass"
database = "disease_prediction"
Dependencies
See requirements.txt for package versions. Here’s a snippet of pinned versions:

text
Copy code
streamlit==1.36.0
streamlit-option-menu==0.3.12
scikit-learn==1.4.2
pandas==2.2.2
numpy==1.26.4
matplotlib==3.8.4
seaborn==0.13.2
mysql-connector-python==9.0.0   # Optional, if using MySQL backend
Future Enhancements
Add more disease prediction modules (e.g., heart disease, Parkinson’s).

Connect with heuristic or deep learning models.

Add user authentication + prediction history tracking (MySQL or SQLite).

Enhance UI with custom CSS or interactive charts.

Improve model explainability (feature importance, SHAP values).

Contact & License
Developed by IAMDHARMA.
Feel free to open issues or submit pull requests!

Licensed under the MIT License. See LICENSE for details.

yaml
Copy code

---

###  How to Use It

1. Copy the content above into a file named `README.md` at the root of your project.
2. Adjust paths, links, or version numbers as necessary.
3. Commit it to your repo:
   ```bash
   git add README.md
   git commit -m "Add project README"
   git push
