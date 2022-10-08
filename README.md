# Machine-Learning-Candlestick-Recognition-Trading-Strategy-
Columbia University FinTech BootCamp Project 2

# Description

This project identifies multiple candlestick patterns using Python, which are used to feed into machine learning models (Naive Bayes Model and Artificial Neural Network Model) that will predict market movement based off of multiple pattern factors. While there are strategies to trade based on one candlestick pattern, using multiple patterns paired with machine learning gives us the confluence needed to make more confident trades.

---

# Research Questions to Answer
How well can we train a machine learning model to identify certain candlestick formations? Can we create a profitable trading strategy based off the model's candlestick formation identification?

---

# Technologies
This project uses Python 3.9 and JupyterLab.

# Libraries

<img width="336" alt="image" src="https://user-images.githubusercontent.com/107157533/194448367-9e651488-0592-450d-af8f-bf65c6a9c3c7.png">
<img width="152" alt="image" src="https://user-images.githubusercontent.com/107157533/194719822-f4d31bd1-7a05-43a7-9c2a-ec94d623eb61.png">


---

# Data
S&P500 high, low, open, and close prices downloaded from TradingView

---

# Creating OHLC function to Plot Candlestick Patterns

![image](https://user-images.githubusercontent.com/107157533/194716331-03963e7a-6de2-434c-84da-01abc0393894.png)


---

# Identifying Candlestick Patterns

Created the Candle stick Trends:

**Candle Sticks Names | Code**

- Bullish harami: BLLHRM
- Bearish harami: BERHRM
- Red hammer: RDHM
- Green hammer: GRNHM
- Bull kicker: BLLKCK
- Bear kicker: BERKCK
- Morning star: MRNSTR
- Evening star: EVNSTR
- Green shooting star: GRNSSTR
- Red shooting star: RDSSTR

![image](https://user-images.githubusercontent.com/107157533/194451132-eba2f9d0-b31a-4a66-b01e-02bbfef34beb.png)

![image](https://user-images.githubusercontent.com/107157533/194451195-3bb68d93-3100-4389-879c-68848ea2b5c6.png)



**Candlestick Pattern Frequency**
![image](https://user-images.githubusercontent.com/107157533/194451341-9151d8b0-0d35-4008-b48a-2dbc782506af.png)

---

# Machine Learning Models

1. Training Naive Bayes Model with Sklearn
- CategoricalNB
- GaussianNB

2. Artificial Neural Network Model

**Steps:**
- Drop columns
- Transform the Target column to dummy variable
- Scale the dataset
- Split the data tp training and testing set
- Train the model
- Test the model
- Evaluate the model
- Reduce the target class to two
- Train new models
- Evaluate the model

**Evaluating Model Performance:**
We found that GaussianNB model was accurate 28% of the time, the Naive Bayes CategoricalNB model only performed at 26%, and the ANN was 51% accurate.

---

# Conclusion

After applying various data preprocessing, model training and testing approach our best accuracy score was 51%. We conclude that the small target dataset, and the non-evenly distrubuted frequencies of the targets resulted in the models poor performances.

**Approach to solving the issues**
- Class imbalance issue: Included 'stratification' when doing train test split of the dataset.
- Data encoding and scaling: Scaled the dataset when neccessary, encode the label as binary or as 'numeric categories'
- Model Accuracy: Use different models and tuning technique to improve model accuracy.

---

# Next Steps

- Enrich our dataset
- Further Tune the Model
- Incorporating the model into our trading strategies
- Analysis of market performance after pattern identification 
- Formulate and backtest a trading strategy
- Connect to AWS to run during market hours and identify in real time
- Connect to a broker to make automated trades

---

# License & Credits
- Columbia Engineering FinTech Bootcamp
- Credit to https://github.com/aliisoli/candlesticks_study/blob/master/Candlesticks_Historical_Analysis.ipynb for candlestick identification functions



