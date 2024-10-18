# Churn-Prediction-Model-for-Customer-Retention-Using-SMOTEENN-and-Random-Forest-Duration

In this repository, we have performed the end to end Exploratory Data Analysis, and idenfitied the characteristics of the customers that are more likely to churn, and I have used them to create a model and have deployed the model.

## Project Structure
1. Problem Statement: Understanding the challenges in the telecom industry and the significance of predicting customer churn.

2. Data Preparation Steps: Deriving new features, filtering high-value customers, tagging churners, and removing attributes of the churn phase.

3. Modelling Approach: Preprocessing data, handling missing values, and conducting exploratory analysis. Deriving new features for improved model performance. Reducing variables using PCA and handling class imbalance. Training a variety of models (Logistic Regression, Decision Trees, and Random Forests) and evaluating them based on appropriate metrics. Building a secondary model to identify important predictor attributes.

4. Conclusion and Recommendations: Summarizing the findings from the models and recommending strategies to manage customer churn based on observations.

## Contributions and Acknowledgments
Contributions to the project are welcome through pull requests. Feel free to share insights, suggestions, or improvements.

Acknowledgments to the telecom industry for providing valuable datasets and insights, enabling us to enhance customer retention strategies.
### 1 For EDA, please refer to : Churn Analysis - EDA.ipynb
### 2 For Model Building, please refer to: Churn Analysis - Model Building.ipynb
### 3 For Model Deployment, please refer to app.py


###  Creating the flask API

```
app = Flask("__name__")
```

The loadPage method calls our home.html.
```
@app.route("/")
def loadPage():
	return render_template('home.html', query="")
```

The predict method is our POST method, which is basically called when we pass all the inputs from our front end and click SUBMIT.
```
@app.route("/", methods=['POST'])
def predict():
```
  
The run() method of Flask class runs the application on the local development server.
```
app.run()
```


Yay, our model is ready, let’s test our bot.
The above given Python script is executed from Python shell.

Go to Anaconda Prompt, and run the below query.
```
python app.py
```


Below message in Python shell is seen, which indicates that our App is now hosted at http://127.0.0.1:5000/ or localhost:5000
```
* Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
```


HERE'S HOW OUR FRONTEND LOOKS LIKE:

![image](https://github.com/user-attachments/assets/07fc8dd2-35ef-4e5c-9fbe-d33d10fe7df8)
