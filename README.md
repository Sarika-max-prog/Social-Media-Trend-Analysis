
# Social Media Trend Analysis Dashboard

## ![image](https://github.com/user-attachments/assets/b4e19556-646b-4958-bd38-f7f1aa60b627)

- **Dashboard Overview:** Main view showing engagement, sentiment, and geographic trends.
- **Hashtag Trends:** Line chart showing hashtag usage over time.
- **Sentiment Distribution:** Pie chart displaying likes by sentiment category.

---

## 📝 Overview
This project builds an **interactive Power BI dashboard** to analyze social media trends, including hashtag usage, sentiment, geographic distribution, and engagement metrics, using a dataset fetched from Kaggle.

---

## 🚀 Process

### 1. Fetching Data from Kaggle
- Downloaded the **`cleaned_socialMedia_data.csv`** from Kaggle containing:
  - Social media posts
  - Timestamps
  - Hashtags
  - Retweets
  - Likes
  - Country information
- Initial inspection was done to understand structure and identify cleaning needs.

### 2. Data Cleaning
- Removed URLs, mentions, and special characters using Python (`pandas`, `nltk`).
- Extracted hashtags into a separate `hashtag_list` column.
- Normalized timestamps to extract **date** and **hour** for time-based analysis.
- Saved the cleaned file as **`cleaned_socialMedia_data.csv`**.

### 3. Sentiment Analysis with VADER
- Applied **VADER (Valence Aware Dictionary and sEntiment Reasoner)** to analyze post sentiments.
- Added a new column **`vader_sentiment`** with compound sentiment scores for better insights.

### 4. Exploratory Data Analysis (EDA)
- Identified key trends like:
  - Top 5 hashtags (e.g., `#Happiness`, `#Nature`)
  - Sentiment distribution (`Neutral`, `Joy`, etc.)
  - Country-wise usage trends (e.g., USA, UK)
- Used **Plotly** for visualization to guide dashboard design.

### 5. Model Accuracy and Validation
- Built a **Random Forest Classifier** to predict post virality.
- Achieved **82% model accuracy**.
- Validated results using **cross-validation** for model robustness.

### 6. Modeling with LDA and NLP
- Applied **Latent Dirichlet Allocation (LDA)** for topic modeling to discover key themes.
- Used NLP techniques like **tokenization** and **lemmatization** to preprocess text.
- Integrated topic-based insights into the dashboard.

### 7. Dashboard Creation
- Imported **`cleaned_socialMedia_data.csv`** into Power BI.
- Created key visuals:
  - Gauge chart for **total engagement** (retweets + likes)
  - Map chart for **geographic trends**
  - Pie chart for **sentiment distribution**
  - Bar chart for **platform usage**
  - Line chart for **hashtag trends over time**
- Added **interactivity** using **platform** and **year slicers**.
- Saved the final dashboard as **`Social_Media_Trend-Analysis.pbix`**.

---

## 🌟 Features
- Track top **hashtag trends** over time.
- Display **sentiment distribution** based on likes.
- Visualize **hashtag usage** by country.
- Show **platform usage** across different regions.
- Measure **total engagement** (Retweets + Likes) with a custom calculated measure.

---

## 📁 Files

| File Name | Description |
| :-------- | :----------- |
| `cleaned_socialMedia_data.csv'` | Cleaned dataset with text, hashtags, timestamps, and engagement data. |
| `Social_Media_Trend_Analysis.pbix` | Power BI file containing the final dashboard. |

---

## 🛠️ Setup

1. Install **Power BI Desktop**.
2. Place **`cleaned_socialMedia_data.csv`** in your working directory.
3. Open **`Social_Media_Trend-Analysis.pbix`** using Power BI Desktop.
4. Refresh the data if any updates are made to the CSV.

---

## 💡 Usage

- Use the **platform** and **year slicers** to filter data interactively.
- Explore different visuals for insights on **hashtags**, **sentiment**, **geography**, and **engagement**.
- Adjust filters to dive into specific countries or hashtags.

---

## 🙌 Credits

- Dataset fetched from **Kaggle**.
- Processed and built by **[sarika]**.
- Built using **Python** (`pandas`, `nltk`, `VADER`, `LDA`), **Plotly**, and **Power BI**.

---

## 📩 Contact

For any queries or questions, feel free to reach out at: **[sarikada25@gmail.com]**








