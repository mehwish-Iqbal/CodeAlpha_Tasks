#   Amazon Reviwes Sentiment Analysis

## 📌 Project Overview

This project focuses on **Sentiment Analysis and Emotion Detection** using Amazon customer reviews. The goal is to classify reviews into **Positive, Negative, and Neutral** sentiments and identify specific emotions expressed by customers.

The analysis also explores sentiment patterns across **customer ratings, countries, and review dates** to understand customer opinions and generate useful business insights.

---

## 🎯 Objectives

* Classify customer reviews as **Positive, Negative, or Neutral**.
* Apply **NLP techniques and a lexicon-based approach** to detect emotions.
* Analyze sentiment patterns in **Amazon reviews**.
* Explore sentiment across **customer ratings and countries**.
* Identify sentiment trends over time.
* Generate insights for **marketing, product development, and customer experience**.

---

## 📂 Dataset

**Dataset:** Amazon Reviews

The dataset contains customer review information such as:

* Reviewer Name
* Country
* Review Count
* Review Date
* Rating
* Review Title
* Review Text
* Date of Experience

After removing duplicate rows and reviews with missing review text, the dataset contained **21,055 reviews** for analysis.

---

## 🛠️ Tools & Technologies

* **Python**
* **Pandas** — Data cleaning and analysis
* **NumPy** — Numerical operations
* **NLTK / VADER** — Sentiment analysis
* **Regular Expressions (re)** — Text preprocessing
* **Plotly** — Interactive visualizations
* **Matplotlib**
* **Seaborn**
* **Jupyter Notebook**

---

## 🧹 Data Cleaning & Preprocessing

The following preprocessing steps were performed:

1. Loaded the Amazon Reviews dataset.
2. Handled malformed CSV parsing using the Python engine.
3. Removed duplicate records.
4. Removed rows with missing review text.
5. Converted review text to lowercase.
6. Removed URLs and unnecessary characters.
7. Removed extra whitespace.
8. Converted the review date into datetime format.

A new `Clean_Review` column was created for sentiment and emotion analysis.

---

## 📊 Visualizations

The project includes interactive Plotly visualizations for:

1. **Amazon Reviews Sentiment Distribution**
2. **Sentiment Percentage**
3. **Sentiment Distribution by Customer Rating**
4. **Emotion Distribution**
5. **Sentiment by Country**
6. **Monthly Sentiment Trend — 2024**

----

## 💬 Sentiment Analysis

The **VADER (Valence Aware Dictionary and sEntiment Reasoner)** sentiment analyzer was used to calculate sentiment scores.

Sentiments were classified using the compound score:

* **Positive:** Score ≥ 0.05
* **Negative:** Score ≤ -0.05
* **Neutral:** Between -0.05 and 0.05

### Sentiment Results

| Sentiment | Reviews | Percentage |
| --------- | ------: | ---------: |
| Positive  |  10,108 |     48.01% |
| Negative  |   9,394 |     44.62% |
| Neutral   |   1,553 |      7.38% |

### Key Finding

Positive reviews represent the largest group, but negative reviews are also a significant portion of customer feedback, indicating **mixed customer sentiment**.

---

## 1. Sentiment Distribution

This chart shows the number of **Positive, Negative, and Neutral** reviews in the Amazon Reviews dataset.

<img width="899" height="449" alt="Sentiment_distribution" src="https://github.com/user-attachments/assets/1acdcb3d-6ca5-45c8-91a6-2085cc57b7ea" />

**Insight:**

* **Positive** reviews represent the largest sentiment group  **10,108**, 
* closely followed by **negative** reviews  **9394**. 
* and **Neutral** reviews account are **1,553** of the dataset.

----
## 2. Sentiment Percentage

This chart shows the **percentage distribution** of Positive, Negative, and Neutral reviews.

<img width="899" height="445" alt="sentiment_percentage" src="https://github.com/user-attachments/assets/1bf73cbc-e096-4c4a-9f65-9d3069434478" />


**Key Insight:**
* Positive reviews accounted for **48.01%**,
* negative reviews for **44.62%**,
* and neutral reviews for **7.38%**,
* showing a mixed pattern of customer sentiment.

---



##  3 ⭐ Sentiment vs Customer Rating

Sentiment was compared with customer star ratings to understand the relationship between review text and ratings.

<img width="901" height="449" alt="sentiment_vs _rating" src="https://github.com/user-attachments/assets/367cdccf-0b84-4145-b6b9-def1246e741d" />



Key observations:

* **1-star reviews** contain the highest number of negative sentiments.
* **5-star reviews** contain the highest number of positive sentiments.
* Some differences exist between text sentiment and star ratings, showing that these two signals may not always completely agree.

---

## 4 😊 Emotion Detection

A **keyword-based emotion lexicon** was used to identify specific emotions in customer reviews.

The following emotions were analyzed:

* Joy
* Sadness
* Anger
* Fear
* Surprise

### Emotion Results

| Emotion  | Detected Count |
| -------- | -------------: |
| Joy      |          6,553 |
| Sadness  |          3,291 |
| Anger    |          2,520 |
| Surprise |            352 |
| Fear     |            188 |


<img width="902" height="536" alt="Emotion_distribution" src="https://github.com/user-attachments/assets/f97146f8-361d-493e-a209-730aec0e9a73" />




### Key Finding

* **Joy** was the most frequently detected emotion, followed by **Sadness** and **Anger**.
* This shows that customer reviews contain both positive and negative emotional expressions.

---

## 5 🌍 Sentiment by Country

Sentiment patterns were also analyzed across countries.

<img width="899" height="445" alt="sentiment _by_country" src="https://github.com/user-attachments/assets/de8fa5b5-9bf9-41d6-8af7-c1329bbf0701" />


### Key Findings

* **US:** Positive 4,616 vs Negative 4,118
* **GB:** Negative 3,435 vs Positive 3,351
* **India:** Positive 294 vs Negative 263
* Several European countries showed slightly more positive than negative reviews.

Overall, sentiment patterns **vary across countries**, while the US and GB contributed the highest review volumes among the analyzed countries.

---

## 6 📈 Monthly Sentiment Trend — 2024

The analysis also examined monthly sentiment patterns during 2024.

<img width="899" height="448" alt="Monthly _sentiment _trend" src="https://github.com/user-attachments/assets/61646c06-90ab-4e85-98e4-c85791237b94" />


### Key Findings

* Negative sentiment increased from **143 reviews in January** to a peak of **219 in July**.
* Positive sentiment reached its highest level of **161 reviews in July**.
* Neutral sentiment remained relatively low, ranging from **16 to 29 reviews**.
* Negative sentiment remained higher than positive sentiment in most months.



---

## 💡 Marketing, Product & Customer Insights

* **Marketing:** Positive customer feedback can be used to highlight product strengths.
* **Product Development:** Negative feedback can help identify recurring product and service issues.
* **Customer Experience:** Sadness and anger patterns can help identify areas requiring customer-service improvements.
* **Customer Engagement:** Joy and positive feedback can help businesses understand what customers appreciate.

---

## 🚀 Final Recommendations

* Monitor negative reviews regularly to identify recurring customer concerns.
* Use emotion patterns to understand customer reactions beyond simple sentiment categories.
* Identify features and services that receive positive customer feedback.
* Track sentiment trends over time to monitor changes in customer satisfaction.
* Combine sentiment, rating, and customer feedback to support data-driven decisions.

---

## 📝 Conclusion

The analysis shows that **Positive reviews (48.01%)** slightly exceed **Negative reviews (44.62%)**, while **Neutral reviews account for 7.38%**.

**Joy** was the most frequently detected emotion, followed by **Sadness** and **Anger**. Sentiment patterns also varied across customer ratings, countries, and time periods.

Overall, sentiment and emotion analysis can provide useful insights into **customer opinions, product improvement opportunities, marketing strategies, and customer experience**.


-----

## 👩‍💻 Author

**Mehwish Iqbal**

Aspiring Data Analyst | Python | Data Analysis | Data Visualization

---

## 🔗 Skills Demonstrated

**Python • Pandas • NumPy • NLP • VADER • Text Preprocessing • Sentiment Analysis • Emotion Detection • Plotly • Data Visualization • Exploratory Data Analysis**


----

## 📁 Project Structure

```text

CodeAlpha_Tasks/
└── Task_03 Sentiment analysis
    |
    |___Images
    ├── Codealph_Task_03_Sentiment_Analysis.ipynb
    ├── Amazon_Reviews.csv
    └── README.md

