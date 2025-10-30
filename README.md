# Reddit-Driven Sector Stock Sentiment Analyzer 📈

This project is a complete end-to-end pipeline that analyzes sentiment from Reddit posts to predict daily stock market movements for major sector ETFs. It was developed as a project for the Pattern Recognition and Machine Learning (PRML) course.

This system scrapes, processes, and models thousands of Reddit comments to see if the "word on the street" can effectively predict whether a sector (like Tech, Finance, or Energy) will go up or down.

## Project Overview

The core idea is to bridge the gap between unstructured, noisy social media chatter and quantitative financial analysis. This tool automates the entire process:

1.  **Data Collection**: Fetches thousands of posts from various finance and sector-specific subreddits.
2.  **Data Integration**: Aligns the collected Reddit data with daily price data (up/down movements) for five major sector ETFs.
3.  **Feature Engineering**: Transforms raw, unstructured text into meaningful quantitative features using TF-IDF vectorization and advanced regular expressions.
4.  **Modeling**: Trains and evaluates multiple machine learning models to classify ETF returns.
5.  **Insight**: Visualizes the top predictive keywords to understand *why* the model is making its predictions, offering transparent market insights.

## Features

* **End-to-End Pipeline**: A complete, modular system for data collection, preprocessing, modeling, and evaluation.
* **Multi-Model Evaluation**: Implements, trains, and compares several ML models, including:
    * Support Vector Machine (SVM)
    * Linear Discriminant Analysis (LDA)
    * Naive Bayes
    * Neural Networks
* **Interpretability**: Not just a black box! The model visualizes top predictive keywords to enhance transparency and market insight.
* **Scalable Design**: Built with modular, reusable code that can be easily extended to new sectors, subreddits, or models.

## How to Run This Project

**1. Clone the Repository**
```bash
git clone [https://github.com/GuitarHero-28/sentimental-analysis.git](https://github.com/GuitarHero-28/sentimental-analysis.git)
cd sentimental-analysis```

**2. Set Up a Virtual Environment**
```bash
python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate````

**3. Install Dependencies All required libraries are listed in the requirements.txt file.
```bash**
pip install -r requirements.txt```

**4. Configure the Project Before running, you may need to update the config.py file with your own settings, such as:**
Reddit API credentials
File paths
Subreddits to target
ETF ticker symbols

**5. Run the Pipeline The main.py script is the entry point for the entire pipeline.**
```bash
python main.py```





