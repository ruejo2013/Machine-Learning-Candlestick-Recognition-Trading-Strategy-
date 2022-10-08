# Machine-Learning-Candlestick-Recognition-Trading-Strategy-
Columbia University FinTech BootCamp Project 2

# Description

This project identifies multiple candlestick patterns using Python, which are used to feed into a machine learning model that will predict market movement based off of multiple pattern factors. While there are strategies to trade based on one candlestick pattern, using multiple patterns paired with machine learning identifies pattern confluence in the market, which can help make more confident trades.

---

# Research Questions to Answer
What candlestick formations are the best to trade? How well can we train a machine learning model to identify certain candlestick formations? Can we create a profitable trading strategy based off of the models candlestick formation identification? 

---

# Technologies
This project uses Python 3.9 and JupyterLab.

# Libraries

<img width="336" alt="image" src="https://user-images.githubusercontent.com/107157533/194448367-9e651488-0592-450d-af8f-bf65c6a9c3c7.png">

---

# Creating OHLC function to Plot Candlestick Patterns
copy right https://mikepapinski.github.io/deep%20learning/machine%20learning/python/forex/2018/12/15/Predict-Candlestick-patterns-with-Keras-and-Forex-data.md.html

![image](https://user-images.githubusercontent.com/107157533/194450870-e3c54a03-10e1-4f7d-879a-9720d98843b9.png)

---

# Identifying Candlestick Patterns

Created the Candle stick Trends:

**Candle Sticks Names | Code**

Bullish harami     : BLLHRM
Bearish harami     : BERHRM
Red hammer     : RDHM
Green hammer     : GRNHM
Bull kicker     : BLLKCK
Bear kicker     : BERKCK
Morning star     : MRNSTR
Evening star     : EVNSTR
Green shooting star     : GRNSSTR
Red shooting star     : RDSSTR

![image](https://user-images.githubusercontent.com/107157533/194451132-eba2f9d0-b31a-4a66-b01e-02bbfef34beb.png)

![image](https://user-images.githubusercontent.com/107157533/194451195-3bb68d93-3100-4389-879c-68848ea2b5c6.png)



**Candlestick Pattern Frequency**
![image](https://user-images.githubusercontent.com/107157533/194451341-9151d8b0-0d35-4008-b48a-2dbc782506af.png)

---

# Machine Learning
Steps:
- Drop columns
- Transform the Target column to dummy variable
- Scale the dataset
- Split the data tp training and testing set
- Train the model
- Test the model
- Evaluate the model

---

# Next Steps

- Further Tune the Model
- Analysis of market performance after pattern identification 
- Formulate and backtest a trading strategy
- Connect to AWS to run during market hours and identify in real time
- Connect to a broker to make automated trades

---

# License
Columbia Engineering FinTech Bootcamp




