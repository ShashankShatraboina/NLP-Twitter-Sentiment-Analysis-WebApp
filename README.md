# Twitter Sentiment Analysis Web App

## Overview

**Twitter Sentiment Analysis Web App** is an NLP-powered project designed to analyze tweets in real time. It classifies tweets into **positive**, **negative**, or **neutral** sentiments, offering valuable insights into public opinion on topics, events, or hashtags. Built with machine learning and popular NLP libraries, the app provides an interactive interface for real-time sentiment tracking and visualization.

---

## Table of Contents

* [Overview](#overview)
* [Features](#features)
* [Tech Stack](#tech-stack)
* [Dataset](#dataset)
* [Installation](#installation)
* [Usage](#usage)
* [Modeling Approach](#modeling-approach)
* [Web App Interface](#web-app-interface)
* [Future Enhancements](#future-enhancements)
* [License](#license)

---

## Features

* Real-time sentiment classification of tweets.
* Categorizes tweets into **positive**, **negative**, or **neutral**.
* Search tweets by keyword or hashtag.
* Interactive, user-friendly web interface built with **Streamlit**.
* Visualizes sentiment distribution with charts.

---

## Tech Stack

* **Python** – Core language.
* **NLP (Natural Language Processing)** – Text preprocessing and analysis.
* **Streamlit** – Web app development.
* **Scikit-learn** – Model training and evaluation.
* **Tweepy** – Twitter API integration for real-time tweets.
* **NumPy & Pandas** – Data handling and preprocessing.
* **Matplotlib & Seaborn** – Data visualization.

---

## Dataset

* Trained on publicly available Twitter sentiment datasets.
* Tweets labeled as *positive*, *negative*, or *neutral*.
* Supports custom datasets or live tweet collection via the **Twitter API** and **Tweepy**.

---

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/NLP-Twitter-Sentiment-Analysis-WebApp.git
   cd NLP-Twitter-Sentiment-Analysis-WebApp
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Set up your Twitter Developer Account and generate API keys.

4. Create a `.env` file with your Twitter API credentials:

   ```env
   TWITTER_API_KEY=your_api_key
   TWITTER_API_SECRET_KEY=your_api_secret_key
   TWITTER_ACCESS_TOKEN=your_access_token
   TWITTER_ACCESS_TOKEN_SECRET=your_access_token_secret
   ```

5. Launch the app:

   ```bash
   streamlit run app.py
   ```

---

## Usage

1. Open the app in your browser (`http://localhost:8501`).
2. Enter a keyword or hashtag to analyze related tweets.
3. The app fetches, preprocesses, and classifies tweets.
4. Results are displayed as sentiment categories and a distribution chart.

---

## Modeling Approach

* **Preprocessing**: Remove URLs, special characters, and stopwords; tokenize text.
* **Vectorization**: Convert text into numerical features using **TF-IDF**.
* **Classification Model**: Logistic Regression is used as the baseline model.
* **Alternative Models**: Naive Bayes and SVM tested for comparison.

---

## Web App Interface

* Input field for entering hashtags/keywords.
* Fetch & analyze button for real-time tweet processing.
* Bar chart showing sentiment breakdown (positive, negative, neutral).

---

## Future Enhancements

* Integrate deep learning models (e.g., **BERT**, **LSTM**) for better accuracy.
* Enable **multilingual sentiment analysis**.
* Add **historical sentiment tracking** for trends over time.
* Implement **user authentication** for personalized dashboards.
