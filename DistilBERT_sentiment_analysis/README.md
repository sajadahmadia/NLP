# Comparison of a rule-based(VADER) method and a machine-learning method (DistillBERT) in sentiment analysis
This project aims to perform comparative sentiment analysis on textual IMDB movie reviews using a machine-learning-based approach and a rule-based approach. As the rule-based approach, VADER lexicon-based algorithm is chosen and as the machine learning-based approach DistillBERT is used. The motivation behind choosing VADER is that based on this research (Hutto & Gilbert, 2014), in which it outperformed all other conventional lexicon-based algorithms. In addition, BERT has shown great performance in sentiment analysis (Alaparthi & Mishra, 2021) and DistillBERT, is the cheaper and faster version of BERT while preserving over 95% of BERT’s performance (DistilBERT, 2023). DistilBERT also showed better performance (accuracy score of 91.46%) in sentiment analysis of tweets regarding COVID-19-related hashtags on Twitter(Ranganathan & Tsahai, 2022).

## Results
The runtime for the DistilBERT model was 26 minutes, while it took 5 minutes for the VADER model. The performance metrics for the two algorithms are given in Table 1. VADER showed a lower overall accuracy score (69.6%) vs. the DistilBERT model (86.7%). Additionally, since successfully predicting positive sentiments is more important than negative sentiments due to its challenges(Alaparthi & Mishra, 2021), the precision and recall metrics for the positive class should be considered. In both metrics, DistilBERT showed a higher performance, specifically in the precision metric, in which it showed a 0.857 score (0.205 higher than VADER’s score). This score means that DistilBERT’s capability to get a better success rate among those reviews predicted to have a positive sentiment was greater than VADER.
Furthermore, the F1 score for the DistilBERT algorithm was 0.868, which was greater than VADER’s value of 0.731. This metric means considering both sides, i.e., precision and recall; the DistllBERT model showed a better performance.

Table 1: Classification performance outputs
| Approach        | Algorithm | Accuracy | Precision | Recall | F1 Score |
|-----------------|-----------|----------|-----------|--------|----------|
| Rule-based      | VADER     | 0.696    | 0.652     | 0.833  | 0.731    |
| Machine learning| DistilBERT| 0.867    | 0.857     | 0.879  | 0.868    |
