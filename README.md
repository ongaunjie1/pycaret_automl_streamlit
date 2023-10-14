# Utilizes pandas-profilling and pycaret for a faster model selection process 
* https://github.com/pycaret/pycaret
* Deployed at Streamlit community cloud: https://automlapp-pycaret.streamlit.app/
  
# Important Note: 
1) The app was created for classification problems and regression problems
2) Purpose of the app is to quickly gauge the performance of different types of models on your dataset, allows for a quicker model selection process **(Does not include fine-tuning)**
3) Fine-tuning may be done on a notebook after model selection 
4) The app might take a long time to run on the streamlit community cloud due to limited resources available

# Other alternatives:
* Run the code locally on your computer for faster performance
*  Deploy the streamlit app on a paid cloud service for faster performance

# Further improvement:
* Add other pycaret's functionality into the app such as adding support for unsupervised ML problems or model fine-tuning capabilities.
* Check out pycaret's doc: https://pycaret.gitbook.io/docs/get-started/modules

# Steps on how to use the AutoML app?

Step 1: Upload your dataset

![image](https://github.com/ongaunjie1/automl_streamlit/assets/118142884/643dd549-acf5-4862-9fb6-f31d9a8a54f7)

Step 2: Select Profiling 

![image](https://github.com/ongaunjie1/automl_streamlit/assets/118142884/02bdc253-3ac2-4d5b-9ba4-daca22f48f2f)

Step 3: Select ML problem (Classification or Regression) and select target variable

![image](https://github.com/ongaunjie1/automl_streamlit/assets/118142884/81790877-548f-42ee-a607-7a1f8a6f891b)

Step 4: Run the modelling and review the output

![image](https://github.com/ongaunjie1/automl_streamlit/assets/118142884/598839fc-b4b0-413c-abf7-5ce577314ab8)





