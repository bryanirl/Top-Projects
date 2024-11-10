# Social Media Sentiment Analysis on Renewable Energy Stock Prices
[!NOTE]
>This project is still under development. Some sections may be incomplete or subject to change. Please see `PROGRESS.md` for a detailed view of the project's progression.

##Table of Contents
1. [Project Overview](#project-overview)
2. [Dataset Information](#dataset-information)
3. [Project Structure](#project-structure)
4. [Requirements and Installation](#requirements-and-installation)
5. [Usage](#usage)
6. [Methodology](#methodology)
7. [Results and Insights](#results-and-insights)
8. [Future Work](#future-work)
9. [Contributing](#contributing)
10. [License](#license)

---

##Project Overview

This project analyzes how social media sentiment around renewable energy (e.g., solar, wind, renewable companies) impacts the stock prices of renewable energy firms. Sentiment is gathered from X (formerly Twitter) and correlated with stock price data to explore if and how public sentiment influences market performance.

Primary Goals:
-**Identify correlations** between social media sentiment and stock price changes.
-**Provide visual insights** on sentiment trends and stock movements over time.
-**Create a predictive model** to assess sentiment impact on stock prices.

---

##Dataset Information

1. **X Data**: Collected using the X API, focusing on keywords related to renewable energy companies and topics.
2. **Stock Price Data**: Historical daily stock prices for selected companies in the renewable energy sector (Nextera Energy, GE Vernova, Adani Green Energy, etc.) from Yahoo Finance API calls.

Data files: 
-x_sentiment_data.csv: Cleaned X data with sentiment scores.
-stock_prices.csv: Stock price data aligned with the X sentiment data

---

##Project Structure

```txt
root
│   README.md              # Project README file
│   requirements.txt       # List of dependencies
│
├── data                   # Data directory (untracked or sample data only)
│   ├── twitter_data.csv
│   └── stock_prices.csv
│
├── notebooks              # Jupyter Notebooks for analysis
│   ├── 1_data_cleaning.ipynb
│   ├── 2_sentiment_analysis.ipynb
│   └── 3_modeling.ipynb
│
├── src                    # Source code for analysis
│   ├── data_collection.py
│   ├── data_preprocessing.py
│   ├── sentiment_analysis.py
│   └── stock_analysis.py
│
└── reports                # Folder for generated reports
    └── final_report.pdf
```
[!NOTE]
>Subject to change as development continues

---

##Requirements and Installation

###Prerequisites
-Python 3.8+
-Twitter Developer Account with API Access

###Installation
1. ***Clone the Repository***:
```
git clone https://github.com/bryanirl/Top-Projects/social-media-sentiment-and-renewable-energy-stocks.git
cd social-media-sentiment-and-renewable-energy-stocks
```
2. ***Create Virtual Environment***:
```
python -m venv env
source env/bin/activate # On Windows use 'env\Scripts\activate'
```
3. ***Install Dependencies***: 
```
pip install -r requirements.txt
```
4. ***API Keys Configuration***:
-Create a `.env` file in the root directory and add your X API keys:
```
TWITTER_API_KEY=your_api_key
TWITTER_API_SECRET=your_api_secret

---

##Usage
###1. Data Collection
Run `data_collection.py` to gather the required X and stock data:
```
python src/data_collection.py
```
###2. Data Preprocessing
Process raw data to calculate daily sentiment scores:
```
python src/data_preprocessing.py
```
###3. Analysis and Visualization
-Open the Jupyter notebooks in `notebooks/` to explore data cleaning, sentiment analysis, and modeling process.
-View interactive dashboards, generated charts, or reports in the `reports/` folder. 

---

##Methodology
1. ***Data Collection***: Gathered data based on renewable energy keywords and historical stock prices.
2. ***Data Cleaning***: Processed raw text and extracted sentiment scores using VADER.
3. ***Sentiment Analysis***: Calculated daily sentiment scores to compare with stock prices.
4. ***Modeling***: Explored regression and time series models to identify sentiment-stock price correlations.

---

##Results and Insights
[!NOTE]
>Project under development

---

##Future Work
-***Expand to Additional Social Media***: Include sentiment from Reddit and other sources to increase data coverage.
-***Consideration of Financial News Media***: Include sentiment from popular financial news outlets to diversify input and broaden scope of analysis.
-***Refine Models***: Test and/or implement additional machine learning/artificial intelligence algorithms for higher predictive accuracy.
-***Real-Time Monitoring***: Explore real-time sentiment analysis for live stock prediction.

---

##Contributing

This project may be open to contribution as the scope increases. 
[!NOTE]
>Please see `CONTRIBUTING.md` for guidelines if applicable.

---

##License
This project is licensed under the MIT License. See `LICENSE` for more details.