# **DSA210-Project**

## **Overview**
Music is a powerful cultural indicator, offering insight into a society’s collective emotions, shared values, and social climate. The genres people prefer, the emotional tone of popular songs, and the themes that resonate nationally often reveal how communities express joy, cope with stress, form identity, and experience everyday life. Because music reflects both individual tastes and broader cultural patterns, it provides a unique lens for understanding societal well-being. This project explores whether a country’s music preferences can meaningfully predict its happiness levels. Specifically, it examines whether happier nations gravitate toward particular types of music, whether emotional or stylistic patterns in popular music correlate with well-being, and whether cultural clusters emerge when music taste is compared with happiness scores. To do this, I will collect data on trending music videos from multiple countries and combine it with national happiness scores from the World Happiness Report. The music data will be processed to extract features such as genre distribution, engagement metrics, and emotional tone, followed by exploratory analysis and hypothesis testing to identify patterns and correlations. Ultimately, this project aims to reveal whether cultural insights can be inferred from music trends and provide a deeper understanding of how societies experience happiness.

---

## Structure
1) Data Cleaning
2) Feature Engineering
3) EDA
4) Statistical Testing
5) Visualization

## Objectives
1. **Understand Cultural Indicators in Music:**
  Explore the relationship between a country’s trending music features (e.g., genre distribution, engagement metrics, emotional tone) and its national happiness score, to uncover which aspects of music trends are most indicative of societal well-being.

2. **Identify Key Predictive Features:**
  Identify the music-related variables that have the strongest correlation with national happiness and determine which features are most informative for understanding cultural and emotional patterns at a country level.

3) **Insight-Driven Analysis:**
   Leverage the insights gained from the data to reveal meaningful cultural patterns and clusters, showing how music trends reflect collective mood and values in different nations.

## Motivation 
In this project, I aim to use my data skills to explore the relationship between national music preferences and societal happiness, and here is why it matters:

**Cultural Insight:**
Understanding how music trends reflect collective emotions and well-being can provide a unique lens into national culture, helping me—and others—appreciate the connection between media consumption and societal mood.

**Scientific Approach:**
I want my conclusions to be guided by data rather than intuition or anecdote. This project allows me to analyze large-scale datasets systematically, uncovering meaningful patterns and correlations between music and happiness.

**Practical Application:**
It presents an opportunity to apply the theoretical knowledge I’ve acquired in class—including data collection, cleaning, visualization, hypothesis testing, and optional predictive modeling—to a real-world and culturally relevant problem.

**Long-Term Impact:**
By revealing the music features that are most strongly associated with happiness, this project may inspire further research on cultural indicators, inform cross-country comparisons, and provide insights for media analysis, policy-making, or even music recommendation systems.

## Dataset 
1) Trending YouTube Video Statistics (113 Countries) – Kaggle:
   This dataset provides detailed statistics on trending YouTube videos across multiple countries. For my project, I will focus only on music-related videos and extract country-level aggregated features:
- **Country:** The country where the video is trending
- **Video Category:** Used to filter for music videos
- **Publish Date:** Date the video was published (helps track temporal trends)
- **Views:** Total views for each trending video
- **Likes:** Number of likes per video
- **Title / Tags / Description:** Optional for text-based analysis (e.g., genre, mood, or theme classification)
- **Engagement Metrics:** Derived measures such as like-to-view ratio, comment-to-view ratio

2) World Happiness Report (2015–2024) – Kaggle:
   This dataset provides annual happiness scores and related metrics for many countries. I will use the following variables:
- **Country:** Match the country field in the YouTube dataset
- **Year:** The year of the observation, used to align with YouTube trends
- **Happiness Score:** The main dependent variable (overall happiness/well-being score)
- **Healthy Life Expectancy:** Life expectancy in years (optional control variable)
- **GDP per Capita:** Economic factor (optional control variable)
- **Freedom to Make Life Choices:** Perceived freedom score (optional control variable)

## Tools and Technologies
I will use the following tools and technologies to collect, process, analyze, and visualize the data:
- **Python:** Primary language for data analysis and modeling
- **Pandas:** Data cleaning, transformation, and aggregation
- **NumPy and SciPy:** Statistical testing and hypothesis analysis
- **Scikit-learn** Predictive modeling (ML)
- **Matplotlib / Seaborn:** Statistical visualizations
  
## Data Collection
This project aims to analyze the relationship between a country's music preferences and its happiness score by integrating two main datasets. 

The first, YouTube Trending Music Data (sourced from Kaggle's Trending YouTube Video Statistics), will be filtered to focus exclusively on music videos using the video category and metadata (title, tags). Key features like views, and likes will be extracted and then aggregated at the country-year level. The derived metrics will include the total number of trending music videos, average engagement scores, and an analysis of genre distribution and emotional tone derived from the video text.

The second dataset is the World Happiness Report Data (2015–2024 from Kaggle), which provides a country's overall happiness score along with key explanatory variables such as GDP per capita, freedom to make life choices, and healthy life expectancy. Crucially, the country and year fields from both datasets will be used to merge and align the aggregated music trends with the corresponding happiness and economic scores. The final stage involves rigorous data preparation, including cleaning, normalization, and handling any missing or inconsistent data points, to create a singular, clean, and comprehensive dataset ready for exploratory analysis, hypothesis testing, and potential predictive modeling. This carefully constructed dataset will allow for the analysis of how national music preferences correlate with well-being.
