
# 📱 A Classifier Model of TikTok Application Reviews

### Can Text Mining and Machine Learning Reveal What People Think About TikTok?

An academic group project exploring public opinions about TikTok through text mining, sentiment analysis, and machine learning classification. Using Twitter posts collected through the Twitter API, the project examines sentiment patterns and compares different classification models to identify the most effective approach for classifying positive and negative opinions.

---

## 📊 Project at a Glance

| Project Metric | Result |
|---|---:|
| Raw Twitter Records | 17,166 |
| Attributes Collected | 12 |
| Final Cleaned Records | 324 |
| Positive Posts | 285 |
| Negative Posts | 39 |
| Classification Models | 3 |
| Best Cross-Validation Accuracy | **89.49%** |
| Decision Tree New-Data Accuracy | **79.13%** |

---

## 🎯 Project Objectives

This project aimed to:

- Evaluate different sentiment classification models and compare their predictive accuracy.
- Identify public perceptions of TikTok by analysing positive and negative opinions shared on Twitter.
- Apply text mining and data preprocessing techniques to transform unstructured text into data suitable for analysis.

---

## 🔍 1. From Twitter Posts to Analysable Data

How can thousands of social media posts be transformed into meaningful information?

The project began by collecting Twitter posts related to TikTok through the Twitter API using RapidMiner. Four search keywords were used to gather relevant opinions:

- TikTok best
- TikTok good
- TikTok service
- TikTok review

The initial collection contained **17,166 records with 12 attributes**. These records provided the starting point for the subsequent data preparation and sentiment analysis process.

---

## 🧹 2. Data Preparation & Text Preprocessing

Raw social media text is often inconsistent, unstructured, and difficult to analyse directly. A series of preprocessing steps was therefore performed in RapidMiner to prepare the collected posts.

The workflow included:

| Preprocessing Step | Purpose |
|---|---|
| Nominal to Text | Converted text attributes into a suitable text format |
| Abbreviation Transformation | Expanded commonly used abbreviations |
| Emoji Transformation | Converted emojis into descriptive words |
| Data Aggregation | Combined and organised relevant data |
| Data Tagging | Prepared and categorised the collected records |
| Duplicate Removal | Eliminated repeated records |
| URL and Retweet Replacement | Handled URLs and retweet references |
| Neutral Sentiment Filtering | Removed neutral records from the final dataset |
| Sentiment Extraction | Extracted sentiment scores and generated sentiment labels |

After preprocessing and filtering, the final dataset contained **324 records**, consisting of 285 positive and 39 negative posts. The cleaned dataset was then exported to Microsoft Excel for further analysis.

### Preprocessing Workflow

![Data Preparation Workflow](images/data-preparation-workflow.png)

### Text Transformation Examples

**Abbreviation Transformation**

![Abbreviation Transformation](images/text-transformation-abbreviations.png)

**Emoji Transformation**

![Emoji Transformation](images/text-transformation-emojis.png)

---

## 📈 3. Descriptive Analysis: What Were People Saying?

After preparing the dataset, descriptive analysis was conducted to explore the characteristics and sentiment patterns of the collected Twitter posts.

The analysis focused on:

- **Tweet Activity:** Examining the dates associated with the collected posts.
- **Sentiment Distribution:** Understanding the proportion of positive and negative opinions.
- **Tweet Sources:** Exploring the sources from which the posts originated.

### Key Sentiment Findings

<figure>
  <img src="images/descriptive-analytics-dashboard.png" alt="Descriptive analytics dashboard" />
</figure>

The final dataset showed a clear difference between positive and negative opinions:

| Sentiment | Number of Posts |
|---|---:|
| Positive | 285 |
| Negative | 39 |
| **Total** | **324** |

Positive posts represented the larger share of the analysed dataset. This suggests that the collected Twitter discussions contained more positive than negative opinions about TikTok.

---

## 🤖 4. Predictive Analysis: Which Model Performed Best?

Can machine learning models accurately classify the sentiment of social media posts?

Three classification algorithms were developed and evaluated using RapidMiner:

1. **Decision Tree**
2. **k-Nearest Neighbours (k-NN)**
3. **Naive Bayes**

Cross-validation was used to evaluate and compare the classification performance of the models.

### Model Comparison

| Classification Model | Accuracy |
|---|---:|
| Decision Tree | **89.49%** |
| k-Nearest Neighbours (k-NN) | 88.88% |
| Naive Bayes | 70.93% |

![Classification Model Accuracy Comparison](images/model-accuracy-comparison.png)

### Key Observation

The **Decision Tree model achieved the highest cross-validation accuracy of 89.49%**, followed closely by k-NN at 88.88%. Naive Bayes recorded the lowest accuracy among the three models at 70.93%.

Based on these results, Decision Tree was selected for further testing using new data.

---

## 🧪 5. Decision Tree: Testing with New Data

Would the best-performing model maintain its classification performance when applied to a new dataset?

To further examine its predictive capability, the Decision Tree model was tested using new data. The predicted sentiment classifications were compared against the actual sentiment labels to evaluate its performance.

<figure>
  <img src="images/decision-tree-testing-results.png" alt="Decision Tree new-data testing results" />
</figure>

The model achieved **79.13% accuracy** on the new dataset.

Although the accuracy was lower than its cross-validation result, the testing provided an additional evaluation of the model's ability to classify previously unseen data.

---

## 💡 Key Takeaways

| Area | Key Finding |
|---|---|
| Data Preparation | 17,166 raw records were processed into 324 cleaned records |
| Sentiment Analysis | Positive posts outnumbered negative posts in the final dataset |
| Model Evaluation | Decision Tree achieved the highest cross-validation accuracy |
| New-Data Testing | Decision Tree recorded 79.13% accuracy on new data |

This project demonstrated how unstructured social media text can be transformed into analysable data and used to explore public sentiment through text mining and machine learning.

---

## 🛠️ Tools & Technical Skills

| Area | Tools & Techniques |
|---|---|
| Data Collection | Twitter API |
| Data Processing | RapidMiner |
| Text Preprocessing | Text transformation, abbreviation expansion, emoji transformation, duplicate removal |
| Sentiment Analysis | Sentiment score extraction and sentiment labelling |
| Descriptive Analysis | Sentiment distribution and tweet-source analysis |
| Machine Learning | Decision Tree, k-NN, Naive Bayes |
| Model Evaluation | Cross-validation and new-data testing |
| Data Export | Microsoft Excel |
| Data Visualisation | Tableau |

### Project Workflow

1. **Data Collection** – Gathered TikTok-related Twitter posts using the Twitter API.
2. **Data Preparation** – Cleaned, transformed, and organised the collected text data.
3. **Sentiment Analysis** – Extracted sentiment scores and assigned sentiment labels.
4. **Descriptive Analysis** – Explored sentiment distribution and other characteristics of the dataset.
5. **Model Development** – Built three classification models using RapidMiner.
6. **Model Evaluation** – Compared model accuracy and tested the selected model using new data.

---

## 👥 Team Collaboration

This was a four-member academic group project. All team members worked collaboratively throughout the project, covering data collection, preprocessing, descriptive analysis, sentiment analysis, model development, and evaluation.

The project provided practical experience in applying text mining and machine learning techniques to real-world social media data.

---

## 📑 Project Presentation

For a more detailed explanation of the methodology, preprocessing workflow, descriptive analysis, and model evaluation, refer to the full project presentation.

---

## 🎓 Project Information

| Detail | Description |
|---|---|
| Course | ISP610 – Business Data Analytics |
| Programme | Bachelor of Science (Hons.) Mathematics |
| Project Type | Academic Group Project |
| Project Year | 2023 |
