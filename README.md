# Reddit Topic Modeling and Comparison with Mainstream News using BERT

## Project Overview
This project aims to apply NLP techniques to Reddit data to analyze discussion trends in pregnancy-related subreddits and compare common themes against topics covered by mainstream news.

## Dataset
- Reddit Data: Collected via [Python Reddit API Wrapper (PRAW)](https://praw.readthedocs.io/en/stable/). One year of posts and comments were collected from the following subreddits: `r/pregnant`, `r/babybumps`, `r/beyondthebump`, `r/pregnancyproblems`, `r/pregnancyafterloss`, `r/newparents`, `r/postpartum_depression`, `r/postpartum_anxiety`, `r/fitpregnancy`, `r/newborns`.
- News Data: Collected via [NewsAPI](https://newsapi.org/docs) with pregnancy-related keywords.
  
## Methodology
### Data Collection and Preprocessing
- Store data using `pandas`
- Remove stop words, apply lemmatization
- Group Reddit comments by post

### Topic Modeling
- Apply [BERTopic](https://maartengr.github.io/BERTopic/index.html) to extract discussion themes
- Remove noise-related topics, like moderation-related discussions

### Emotion Analysis
- Apply emotion classification model and extract top emotion from each text (title + post + comment)
- Model derived from the [GoEmotions](https://research.google/blog/goemotions-a-dataset-for-fine-grained-emotion-classification/) dataset, with labels Anger, Disgust, Fear, Joy, Neutral, Sadness, Surprise

### Comparative Analysis
**TBD**

## Results
