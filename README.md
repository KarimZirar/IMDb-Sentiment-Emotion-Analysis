# IMDb-Sentiment-Emotion-Analysis
This project analyzes sentiment and fine-grained emotions in IMDb user reviews using transformer-based models. Instead of relying on star ratings, it examines how audiences actually express reactions in text — at both movie and genre levels.

What it does:
- Runs sentiment classification (positive / neutral / negative)
- Runs multi-label emotion detection (28 emotion categories)
- Compares:
 - Individual movies
 - Different genres (Drama, Horror, Comedy, Romance, Thriller)
- Aggregates model confidence scores

Models Used:
- cardiffnlp/twitter-roberta-base-sentiment-latest (RoBERTa-based sentiment model)
- SamLowe/roberta-base-go_emotions (RoBERTa-based emotion model trained on GoEmotions)
Both models are used through HuggingFace Transformers.

Dataset:
- ~1 million IMDb reviews (IEEE Dataport)
- Cleaned and filtered to ~662k English reviews
- Sampled per genre for computational feasibility

Main Findings (Brief):
- Drama, Romance, and Comedy skew strongly positive.
- Horror and Thriller show higher negative sentiment.
- Admiration is the dominant emotion across genres.
- Star ratings do not always align with emotional tone in reviews.

Structure:
- Python_code.ipynb: Main analysis and model implementation.
- Exploring Sentiment and Emotion Trends Across...: Full research paper in PDF format.

## Author

Abdelkarim Zirar  
MA Data and Discourse Studies  
Technische Universität Darmstadt
