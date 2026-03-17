# **Stock Performance Dashboard** 

An interactive stock performance analysis dashboard built using Python and Tableau, designed to analyze stock price trends, trading activity, and key performance metrics over time.    

This project transforms raw financial time-series data into intuitive visual insights that help evaluate price behavior, market participation, and investment performance.    

# **Project Overview**    

This dashboard provides a comprehensive view of stock market performance by combining price analysis, technical indicators, and trading volume insights.    

Key questions the dashboard helps answer:

### **1. How has the stock price evolved over time?**    
The dashboard visualizes stock price behavior using candlestick charts that display open, high, low, and close prices. This allows users to identify market trends, volatility, and turning points in price movement.

### **2. How do short-term and long-term trends compare?**    
Moving averages are used to evaluate trend direction:

**MA5** – short-term trend

**MA20** – medium-term trend

**MA50** – long-term trend

Comparing these indicators helps reveal potential momentum shifts and trend changes.

### **3. How does trading volume support price movements?**     
Trading activity is analyzed through daily trading volume and a Volume Oscillator.

The volume oscillator compares short-term and long-term trading activity:

**Volume Oscillator = (VMA5 - VMA20) / VMA20**    

Positive values suggest stronger market participation, while negative values indicate weakening trading momentum.

### **4. How would an investment perform over time?**    
The dashboard includes an Indexed Price Performance metric, calculated as:

**Index= 100 × (Current Price / Start Date Price)**
	​
This allows users to interpret performance in a simple way:    

If $100 was invested at the selected Start Date, the index shows how much the investment would be worth at End Date.    

Data Structure Overview

The dataset includes historical stock market data with the following variables:

**Date** – Trading date

**Open Price** – Opening price of the stock

**High Price** – Highest price during the trading day

**Low Price** – Lowest price during the trading day

**Close Price** – Closing price

**Adjusted Close** – Price adjusted for corporate actions

**Volume** – Number of shares traded


# **Methodology**
### **1. Data Cleaning**

Stock price data was processed using Python to ensure consistent formatting and accurate calculations. Missing values were handled and numeric variables were converted to appropriate formats.

### **2. Feature Engineering**

Additional metrics were calculated to support analysis

Daily price change

Percentage price change

Moving averages (MA5, MA20, MA50)

Volume moving averages (VMA5, VMA20)

Volume oscillator

Indexed price performance

### **3. Time Series Analysis**

Price trends were evaluated using moving averages and candlestick visualization to capture both short-term and long-term market behavior.

### **4. Interactive Dashboard Design**

The Tableau dashboard allows users to dynamically explore data using:

Start Date and End Date parameters

Interactive tooltips

KPI summary metrics

These features enable flexible analysis of different market periods.    

# **Tools**

### **Data Processing**

Python

Pandas

NumPy

### **Visualization**

Tableau

### **Analysis Techniques**

Time series analysis

Moving average trend analysis

Volume-based momentum indicators

Financial data visualization
