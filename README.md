# Bengaluru House Price Prediction  


![Python](https://img.shields.io/badge/Python-3.11.9-blue)
![FastAPI](https://img.shields.io/badge/FastAPI-Backend-green)
![Render](https://img.shields.io/badge/Deployed%20on-Render-purple)
![License](https://img.shields.io/badge/License-MIT-yellow)


## Overview  
The **Bengaluru House Price Prediction** project is a web-based **machine learning application** that predicts real estate prices in Bengaluru.  
It is powered by a **FastAPI backend** and a **responsive frontend** built with **HTML, CSS, JavaScript, and jQuery**.  
### Users can input property details such as **location, area type, total square feet, number of bedrooms (BHK), bathrooms, and balconies** to get an instant estimated property price.



## Screenshots
![ ](assets/ss1.png)
![ ](assets/ss2.png)

## Live Demo  
You can try out the live version of the app here: 
[Live Demo on Render](https://bangalore-house-price-prediction-ilae.onrender.com)



## Tech Stack  

### Frontend  
- HTML  
- CSS  
- JavaScript  
- jQuery  

### Backend  
- FastAPI  
- Uvicorn
- Pydantic

### Machine Learning  
- Scikit-learn  
- Pandas  
- NumPy  

### Deployment  
- Render  



## Model Description  
- **Dataset:** Bengaluru House Prices ([Available here](https://www.kaggle.com/datasets/amitabhajoy/bengaluru-house-price-data))  
- **Algorithms Compared:** Linear Regression, Lasso Regression, Ridge Regression, Decision Tree Regressor, and Random Forest Regressor  
- **Best Model:** Random Forest Regressor (selected after hyperparameter tuning using GridSearchCV)  
- **Features Used:**  
  - Location  
  - Area Type (Super Built-up, Plot, Carpet, Built-up)  
  - Total Square Feet Area  
  - Number of Bedrooms (BHK)  
  - Number of Bathrooms  
  - Number of Balconies  

The dataset was cleaned, encoded, standardized, and normalized through a **data preprocessing pipeline**.  
Categorical columns like **location** and **area type** were one-hot encoded.  
The trained model was serialized using **pickle** and integrated into the FastAPI backend through a well-defined **machine learning pipeline** for seamless preprocessing and prediction.



## Features  
- Real-time Bengaluru house price prediction  
- Fast and lightweight backend with FastAPI  
- Interactive frontend with jQuery-based AJAX requests  
- Modular structure with `utils/` for helper functions  
- Fully deployed on Render  
- Simple and intuitive UI  



##  Getting Started  

### Clone the Repository  
```bash
git clone https://github.com/parvgupta09/Bangalore-House-Price-Prediction.git
cd Bangalore-House-Price-Prediction
```

### Create Virtual Environment  
```bash
python -m venv venv
source venv/bin/activate   # For Linux/Mac
venv\Scripts\activate      # For Windows
```

### Install Dependencies
```bash
pip install -r requirements.txt
```

### Run the FastAPI Server
```bash
uvicorn server:app --reload
```

### Access the Web App  
Open your browser and go to:  
[http://127.0.0.1:8000](http://127.0.0.1:8000)



## Project Structure  
```
Bangalore-House-Price-Prediction/
│
├── templates/
│ └── app.html   # Frontend HTML file
│
├── static/
│ ├── app.css   # Stylesheet for the web page
│ └── app.js   # JavaScript & jQuery logic
│
├── model/
│ ├── pipeline.pkl   # Serialized ML pipeline
│ ├── columns.json   # Feature columns metadata
│ ├── model train.ipynb   # Notebook for model training
│ │
│ └── dataset/
│ └── Bengaluru_House_Dataset.csv # Original dataset
│
├── utils.py   # Utility functions for model handling
├── server.py   # FastAPI backend server
├── requirements.txt   # Python dependencies
├── LICENSE   # License file
├── .gitignore   # Git ignore rules
└── README.md   # Project documentation
```



## License  
This project is licensed under the **MIT License** — see the [LICENSE](https://github.com/parvgupta09/Bangalore-House-Price-Prediction/blob/main/LICENSE) file for details.



## Contact / Connect
If you liked this project or want to collaborate, feel free to connect with me:
- [LinkedIn](https://www.linkedin.com/in/parv-gupta-323738309/)
- Email: parvguptajpr@gmail.com
