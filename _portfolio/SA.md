---
title: "Sentiment Analysis on the Impact of Autonomous Vehicle Incidents"
excerpt: "Analyzed the long-term and short-term public bias towards autonomous vehicles following incidents like the Uber pedestrian crash. Utilized advanced NLP techniques, including transformers and traditional sentiment analysis models, on data scraped from news articles and Twitter. Processed data using Apache Spark and visualized insights with Python.<br/><img src='/images/SA.jpg'>"
collection: portfolio
---

This project investigates the **long-term and short-term effects on public sentiment towards autonomous vehicles** in the aftermath of significant incidents, such as the Uber pedestrian crash. The analysis was conducted using a dataset comprised of news articles and tweets.

**Data Collection**: 
- **Twitter API with Tweepy** was employed to scrape tweets related to autonomous vehicles.
- **BeautifulSoup** was utilized to scrape news articles published around the time of the incidents.
- Additional sentiment data was sourced from **Sprinklr** to enrich the analysis.

**Data Processing**:
- The raw data was cleaned extensively to remove noise, ensuring relevance by categorizing content based on keywords directly related to autonomous vehicle incidents.
- The entire processing pipeline was managed using **Apache Spark**, facilitating efficient handling of large volumes of text data.

**Sentiment Analysis**:
- Sentiment analysis was performed using a **pretrained transformer model** from Hugging Face's **RoBERTa**.
- Additionally, traditional sentiment analysis models such as **VADER** and **TextBlob** from **NLTK** were used to provide comparative insights.
- The models assessed the sentiment polarity and subjectivity, offering a comprehensive view of public reactions.
- The results were visualized using **Python** libraries, including **Matplotlib** and **Seaborn**, to illustrate trends over time and compare sentiments across different platforms (news vs. social media).

The project reveals how public sentiment evolves following autonomous vehicle incidents and highlights differences in immediate versus long-term reactions. These insights can be crucial for policymakers and companies involved in autonomous vehicle technology.

You can view the full code and implementation details on [GitHub](https://github.com/VishnuSaiKarthikGindi/Sentiment-Analysis-on-autonomous-vehicle-technology-using-tweets).