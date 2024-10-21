# Financial Sentiment Analysis and Time Series Report

This project performs a comprehensive analysis of sentiment across different sectors using financial news articles. The sentiment analysis is powered by **BERT FT Finance Sentiment Analysis**, and the news articles are fetched from **NewsAPI**. The notebook automates the process of sentiment scoring, time series analysis, and report generation, using the **Gemini 1.5 Pro model** to summarize and highlight key results.

## Features

1. **Install Dependencies & Initialize**: 
   - Installs necessary Python libraries (e.g., pandas, matplotlib, seaborn, etc.).
   - Initializes the NewsAPI and defines style settings for visualizations.

2. **Fetch Articles**:
   - Utilizes a date range selector to retrieve news articles between two specific dates from the NewsAPI.

3. **Sector & Sentiment Assignment**:
   - Classifies articles into predefined sectors (e.g., Technology, Healthcare) and assigns sentiment scores to the articles using the pre-trained **BERT FT Finance Sentiment Analysis** model.

4. **All Sectors Time Series Plot**:
   - Provides a time-series analysis of sentiment trends across all sectors.
   - Allows for a date range selector to visualize sentiment trends over the desired period.

5. **Single Sector Time Series Plot**:
   - Allows selection of a specific sector and date range to visualize sentiment trends over time for that sector.

6. **Violin Plot**:
   - Displays sentiment score distributions for different sectors, providing insights into the variability and spread of sentiment within each sector.

7. **Top 3 Positive and Negative Sentiment Sectors**:
   - A bar chart that highlights the top 3 sectors with the highest positive and negative weighted sentiment scores.

8. **Sentiment Scores vs S&P 500 Index**:
   - Visualizes the relationship between sentiment scores and the performance of the S&P 500 index on corresponding dates.

9. **Granger Causality Test**:
   - Determines whether sentiment scores have predictive power over movements in the S&P 500 index.

10. **Automated Report Generation**:
    - The **Gemini 1.5 Pro model** is used to automatically summarize the analysis and generate a textual report. The report includes key highlights, trends, and any potential correlations between sentiment and market indices.

## Requirements

- Python 3.x
- Libraries:
  - pandas
  - matplotlib
  - seaborn
  - requests
  - BERT FT Finance Sentiment Analysis (pre-trained model)
  - Gemini 1.5 Pro (for summarization)
- NewsAPI Key (to fetch articles)

## How to Run

1. Clone the repository and navigate to the project directory.
2. Install all dependencies listed in `requirements.txt`.
3. Get your **NewsAPI** key and update the API call within the notebook.
4. Run the notebook cells in sequence:
   - Initialize dependencies and API.
   - Fetch articles for the desired date range.
   - Perform sentiment analysis and sector classification.
   - Visualize the results through the provided plots.
   - The final section will automatically generate a report summarizing the analysis and key insights.

## Results

The notebook provides an end-to-end solution for financial sentiment analysis, offering both visual and textual insights into how sectoral sentiment scores change over time and how they correlate with stock market indices like the S&P 500. It generates visualizations for time series analysis, sentiment distribution, and predictive capabilities, while also creating an automated report summarizing the results.
