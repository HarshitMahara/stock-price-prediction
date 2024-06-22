# Stock Price Prediction using Sentiment Analysis

## Overview

This project aims to build a web application that predicts the stock prices of various Indian companies based on sentiment analysis of social media data, particularly from Twitter. The application provides real-time current stock prices and future price predictions.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Setup Instructions](#setup-instructions)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)

## Features

- Real-time current stock price display.
- Future stock price prediction based on sentiment analysis.
- Interactive dashboard with visualizations of stock trends and sentiment analysis.
- User-friendly interface for selecting stocks and viewing predictions.

## Tech Stack

### Backend
- **Language:** Python
- **Framework:** Flask

### Frontend
- **Framework:** React.js

### Databases
- **Structured Data:** PostgreSQL
- **Unstructured Data:** MongoDB

### APIs for Data Collection
- **Stock Prices:** Alpha Vantage
- **Tweets:** Twitter API

### Machine Learning & Data Processing Libraries
- TensorFlow/Keras
- Scikit-learn
- NLTK, VADER, TextBlob
- NumPy, Pandas

### Data Visualization
- Plotly

### Deployment
- Heroku

## Setup Instructions

### Prerequisites

- Python 3.8+
- Node.js
- Git
- PostgreSQL
- MongoDB

### Step 1: Clone the Repository

```sh
git clone https://github.com/yourusername/stock-price-prediction.git
cd stock-price-prediction
```

### Step 2: Set Up Python Environment

#### 1. Create and activate virtual environment:

```sh
python -m venv stock-env
source stock-env/bin/activate  # On Windows use: stock-env\Scripts\activate
```

#### 2. Install required Python packages:

```sh
pip install --upgrade pip
pip install Flask Flask-RESTful Flask-Cors
pip install numpy pandas scikit-learn tensorflow keras
pip install nltk vaderSentiment textblob
pip install plotly
pip install psycopg2-binary pymongo
pip install requests tweepy
pip install jupyterlab
```

###  Step 3: Set Up Node.js Environment

#### 1. Install required Node.js packages:

```sh
cd frontend
npm install
```

### Step 4: Set Up Databases
- PostgreSQL: Create a database for storing structured data.
- MongoDB: Set up a MongoDB database for storing unstructured data like tweets.

### Step 5: Set Up API Keys
- Alpha Vantage: Obtain an API key from Alpha Vantage.
- Twitter API: Obtain API keys from Twitter Developer.

### Step 6: Configure Environment Variables
Create a `.env` file in the project root directory and add your API keys and database credentials:

```env
ALPHA_VANTAGE_API_KEY=your_alpha_vantage_api_key
TWITTER_API_KEY=your_twitter_api_key
TWITTER_API_SECRET_KEY=your_twitter_api_secret_key
TWITTER_ACCESS_TOKEN=your_twitter_access_token
TWITTER_ACCESS_TOKEN_SECRET=your_twitter_access_token_secret
POSTGRES_DB=your_postgres_db_name
POSTGRES_USER=your_postgres_user
POSTGRES_PASSWORD=your_postgres_password
POSTGRES_HOST=your_postgres_host
MONGO_URI=your_mongo_uri
```

### Step 7: Run the Application

- Start the Flask backend:
  ```sh
  cd backend
  flask run
```
-Start the React frontend:
 ``` sh
 cd frontend
 npm start
```

## Usage
