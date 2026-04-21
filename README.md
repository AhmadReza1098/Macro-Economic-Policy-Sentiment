# Macro-Economic Policy Sentiment & Sovereign Risk Engine

Macro-Policy-Risk-Engine/  
│
├── notebooks/
│   └── policy_sentiment_engine.ipynb  
│
├── images/
│   ├── sentiment_distribution.png     
│   └── sentiment_vs_volatility.png    
│
├── requirements.txt                   
└── README.md                          

## Project Overview
This project engineers a natural language processing (NLP) pipeline to extract, quantify, and analyze sentiment from Reserve Bank of India (RBI) policy documents and related financial news. The core objective is to translate qualitative central bank communication into quantitative "Hawkish" vs. "Dovish" signals, treating macroeconomic sentiment as a lead indicator for market volatility and sovereign risk.

## Quantitative Methodology
* **Data Engineering:** Automated the extraction of 200+ RBI policy-related articles and meeting summaries from the Economic Times.
* **Text Processing:** Applied financial-text tokenization and noise reduction to isolate policy-critical vocabulary.
* **Sentiment Scoring:** Utilized valence-aware dictionary reasoning (VADER) adapted for financial contexts to classify text into structured sentiment vectors, scoring exact magnitudes of policy optimism vs. pessimism.
* **Risk Visualization:** Mapped sentiment distributions to identify structural shifts in market confidence surrounding repo rate adjustments.

## Key Insights & Business Value
* **Tail-Risk Identification:** Isolated extreme negative compound sentiment scores (-0.897) during periods of high economic uncertainty, proving the model's ability to capture sudden bearish market shifts.
* **Policy Correlation:** Demonstrated that prolonged periods of positive sentiment (peaking at 0.966) directly correlated with RBI's stabilization of repo rates.
* **Strategic Application:** This pipeline provides a framework for translating unstructured central bank rhetoric into structured risk metrics, a critical input for portfolio stress testing and volatility forecasting.

## Technical Architecture
* **Language:** Python
* **Libraries:** Pandas, NLTK (VADER), BeautifulSoup, Requests, Matplotlib
* **Execution:** Jupyter Notebooks (`/notebooks` directory)
