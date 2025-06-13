**Customer Churn Prediction App**

This project is a customer churn prediction application developed using Python, Streamlit, and machine learning. 
It allows users to input basic customer information—such as age, gender, tenure, and monthly charges—and receive a real-time prediction on whether the customer is likely to churn (leave the service). 
The application is designed to help businesses proactively identify customers at risk of leaving so that they can take preventive measures to retain them.

The project is built on a machine learning model trained in a Jupyter notebook (churn.ipynb) using a dataset named customer_churn_data.csv. 
After preprocessing the data and training the model, the scaler and model were saved as scaler.pkl and model.pkl, respectively. 
These files are then imported into the Streamlit web application (app.py) to make predictions based on user input. 
The gender input is encoded where "Female" is represented as 1 and "Male" as 0. The features used in prediction are age, gender, tenure, and monthly charges. 
These inputs are scaled using the same preprocessing technique used during training before being passed into the model to generate a prediction.

To run this project, users should first clone the repository and install necessary Python libraries including Streamlit, NumPy, pandas, joblib, and scikit-learn. 
Once dependencies are installed, the application can be launched locally by running streamlit run app.py. 
After launching, users can interact with a simple interface to enter values and click the predict button to see if the model forecasts churn ("Yes") or not ("No").

The project structure includes the training notebook (churn.ipynb), the dataset file (customer_churn_data.csv), the Streamlit app (app.py), and the saved model files (model.pkl and scaler.pkl). 
This project demonstrates a complete machine learning pipeline from data preprocessing and model training to deployment via a user-friendly web interface.
The repository and application are open-source and can be freely modified or extended as needed.
