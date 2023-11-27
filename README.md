# Utilizes pandas-profilling and pycaret for a faster model selection process 
* https://github.com/pycaret/pycaret
* pycaret's documentation: https://pycaret.gitbook.io/docs/get-started/modules
* Strealit app deployed at Streamlit community cloud: https://automlapp-pycaret.streamlit.app/

# This repository will showcase the simplest implementation of PyCaret into a streamlit app (only using model comparison)
* Refer to the last section below for a more in-depth use case of PyCaret, adding in other features such as data-preprocessing, model creation, model tuning, model evaluation
* These features can be added to the streamlit app if desire.

# What does pandas-profiling do ?
* Pandas-Profiling is a Python library that provides a simple and efficient way to perform exploratory data analysis (EDA) on a Pandas DataFrame. The library generates a comprehensive HTML report with various statistical and visual insights into the structure and characteristics of the dataset.

# What does PyCaret do ?
* PyCaret is an open-source, low-code maching learning library in Python that automates machine learning workflows. It is an end-to-end machine learning and Model management
  tool that exponentially speeds up experiment cycle and makes you more productive.


# App features
* Utilize pandas-profiling to generate a HTML report with insights from a dataset.
* Utilizes PyCaret to quickly compare between different algorithms, generates a table ranking each algorithms based on metrics. 
  
# Important Note: 
1) The app was created for classification problems and regression problems
2) Make sure that your data is cleaned before using PyCaret
3) Purpose of the app is to quickly gauge the performance of different types of models on your dataset, allows for a quicker model selection process **(Does not include data pre-processing and fine-tuning)*
4) The app might take a long time to run on the streamlit community cloud due to limited resources available
5) Pycaret is CPU intensive, make sure your CPU is fast enough. Else, you could run Pycaret using GPU for a faster performance
6) Simply add **use_gpu=True** into classification_setup(df, target=chosen_target, verbose=False, **use_gpu=True**) to utilize GPU instead of CPU

# Other alternatives:
* Run the code locally on your computer for a faster performance
* Deploy the streamlit app on a paid cloud service for a faster performance

# Further improvement:
* Add pycaret's other functionality into the app such as adding data pre-processing and model fine-tuning capabilities.

# Docker Image
* Pull command: docker pull ongaunjie1/automl-app:latest
* Run command: docker run -d -p 8501:8501 ongaunjie1/automl-app:latest

# Steps on how to use the AutoML app?

* **Step 1: Upload your dataset**

![image](https://github.com/ongaunjie1/automl_streamlit/assets/118142884/643dd549-acf5-4862-9fb6-f31d9a8a54f7)

* **Step 2: Select Profiling** 

![image](https://github.com/ongaunjie1/automl_streamlit/assets/118142884/02bdc253-3ac2-4d5b-9ba4-daca22f48f2f)

* **Step 3: Select ML problem (Classification or Regression) and select target variable**

![image](https://github.com/ongaunjie1/automl_streamlit/assets/118142884/81790877-548f-42ee-a607-7a1f8a6f891b)

* **Step 4: Run the modelling and review the output**

![image](https://github.com/ongaunjie1/automl_streamlit/assets/118142884/598839fc-b4b0-413c-abf7-5ce577314ab8)

# A more in-depth use-case of PyCaret, running on a notebook.



