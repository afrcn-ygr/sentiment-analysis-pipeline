# Sentiment Analysis Pipeline (Azure + Power BI)

## Overview

This project implements an end-to-end **Sentiment Analysis Pipeline** using cloud and Python tools. It collects real-world text data, runs sentiment analysis, ingests it into the Azure cloud, and visualizes insights in Power BI.

## Architecture

1. 🐍 Python script collects tweets/comments and calculates sentiment scores
2. ☁️ Data uploaded to Azure Blob Storage
3. 🔄 Azure Data Factory loads CSV into Azure SQL Database
4. 📊 Power BI connects to SQL and visualizes sentiment analysis

## Folder Structure

sentiment-analysis-pipeline/
├── sentiment_pipeline.py                # Sentiment scraper
├── upload_to_blob.py                    # Azure Blob uploader
├── cleaned_twitter_sentiment.csv        # Sample output
├── Sentiment_Analysis_Project_Presentation.pptx
├── azure_adf_pipeline.png               # Screenshot (ADF)
├── power_bi_dashboard.png               # Screenshot (Power BI)
├── requirements.txt
└── README.md

## Tools Used

- Python: `TextBlob`, `pandas`, `tweepy`, `requests`
- Azure Blob Storage
- Azure Data Factory (ADF)
- Azure SQL Database
- Power BI

## Results

- Sentiment scores are computed per tweet/comment
- Data flows from CSV to SQL via ADF
- Power BI shows:
  - 📈 Sentiment distribution (Positive, Negative, Neutral)
  - 📋 Table of tweets + scores
  - 📊 Sentiment trend insights

## Setup Instructions

### 1. Clone the Repo

```bash
git clone https://github.com/your-username/sentiment-analysis-pipeline.git
cd sentiment-analysis-pipeline
