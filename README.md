# AI-Driven-Tourism-Demand-Forecasting-and-Destination-Overcrowding-Prediction-System

An end-to-end Streamlit application for tourism demand forecasting and destination overcrowding prediction using Machine Learning.
---
📁 Project Structure
```
tourism_app/
├── app.py              # Main Streamlit entry point
├── auth.py             # Login / signup / session management
├── model.py            # ML models (Linear Reg, Logistic Reg, Random Forest)
├── utils.py            # Helper functions, constants, KB
├── users.csv           # User database (auto-created)
├── requirements.txt    # Python dependencies
├── README.md
└── dataset/
    └── travel_data.csv # Tourism dataset
```
---
🚀 Quick Start
1. Install dependencies
```bash
pip install -r requirements.txt
```
2. Run the app
```bash
streamlit run app.py
```
3. Open in browser
```
http://localhost:8501
```
---
🔐 Demo Accounts
Role	Username	Password
Travel Agent	admin	admin123
User	user1	user123
---
🎯 Features
Travel Agent Dashboard
Tab	Description
📊 Overview	Dataset summary, statistics, distributions
📂 Dataset	Upload, filter, download datasets
📈 Dashboard	Interactive charts (line, bar, heatmap, pie, scatter)
🔮 Prediction	ML-powered demand & overcrowding predictions
💰 Budget Planner	Day-wise trip planning with cost breakdown
🗺 Map Explorer	State-wise tourist location map
🤖 Chatbot	AI travel assistant
🚨 Alerts	High-risk overcrowded locations & strategies
👤 Profile	Edit profile settings
User Dashboard
Tab	Description
🤖 Chatbot	AI travel assistant
💰 Budget Planner	Trip budget planning
🔍 Place Search	Search destinations with crowd info
👤 Profile	Manage profile
---
🤖 ML Models Used
Model	Task	Algorithm
Linear Regression	Visitor demand prediction	sklearn LinearRegression
Logistic Regression	Overcrowding classification	sklearn LogisticRegression
Random Forest	Both demand + crowd (ensemble)	sklearn RandomForest
---
📊 Dataset Columns
The `travel_data.csv` contains 25 columns including:
`Date`, `Month`, `Year`, `Season`, `Day_of_Week`, `Is_Weekend`
`Weather_Type`, `Location_City`, `Location_State`, `Zone`
`Place_Name`, `Place_Type`, `Google_Rating`, `Significance`
`Visitors_Count`, `Ticket_Price`, `Revenue`
`Tourist_Type`, `Rating`, `Review_Count_Lakhs`
---
💡 Tips
The ML models train automatically on first load and are cached for speed.
Upload a new CSV in the Dataset tab to replace the default data.
All user data is stored locally in `users.csv`.
