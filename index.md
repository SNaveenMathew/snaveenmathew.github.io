# Naveen Mathew Nathan S.

## Summary

I'm an aspiring data scientist with 3.5 years of industry experience in data science R&D. I worked in service oriented settings and in product teams that delivered insights from data. I'm deeply interested in pipelining and automation of machine learning (supervised and unsupervised). In the past I worked with delivery teams to create automated pipelines for supervised and unsupervised learning ([details](#productsolution-development)).

## Product/Solution Development

Short presentations on my R&D work in industry can be found below:

- Automated pipeline for binary classification [[View presentation](supervised_slides.html)] [[View repo on GitHub](https://github.com/SNaveenMathew/EnsembleModel)]
- Automated pipeline for clustering and basket anlaysis [[View presentation](unsupervised_slides.html)] [[View repo on GitHub](https://github.com/SNaveenMathew/AutomatedClustering)] [[View use case presentation](unsupervised_use_case.html)]
- Pipeline for natural language understanding and predictive modeling [[View presentation](text_classification_presentation.html)] [[View repo on GitHub](https://github.com/SNaveenMathew/TextMining)] [[View use-case presentation](text_classification_use_case.html)][[Example notebook](https://github.com/SNaveenMathew/TextMining/blob/master/main.ipynb)]

## Research

Information on my current research work in academia can be found below:

- Unsupervised learning and crowd-sourcing for exoplanet candidate identification [[Motivation](https://snaveenmathew.github.io/Unsupervised-Exoplanet/)] [[Blog post](https://medium.com/@snaveenmathew/unsupervised-learning-in-astronomy-for-exoplanet-candidate-identification-997f3f958dae)]
    - Why do we need unsupervised learning and crowd-sourcing for exoplanet candidate identification? [[Blog post](https://medium.com/@snaveenmathew/search-for-exoplanets-humans-vs-stars-cfb2bf494317)]
    - An old version of the application is live! [[Link to the application](https://snaveenmathew.shinyapps.io/unsupervised_exoplanet/)]
        - Demo details: username: `user1`, password: `pass1`
- Reinforcement learning for traffic control [[Blog post](https://medium.com/@snaveenmathew/lessons-from-my-internship-and-immediate-aftermath-40edacfa0b85)]
    - I applied for 2 patents in reinforcement learning and federated learning respectively. I'm currently working on a publication

Information on my past research work in academia can be found below:

- Applications of machine learning and deep learning in finance
    - Applied filters, feature engineering, machine learning and stacked ensembling to predict the direction of movement of bitcoin price in real-time [[PDF Report](ML_report.pdf)] [[Technical Presentation](ml_finance.html)]
    - Used deep learning to predict the direction of movement (in next 60 seconds) of VWAP of most significant levels in limit order book [[PDF](DL_report.pdf)]
        - Feature engineering: time bar, missing value treatment
        - Sampling: first 60% for training, 60%-80% for validation, last 20% for testing
        - Machine learning: fully connected network (hyperparameters: number of layers, number of neurons, dropout), convolutional neural network (hyperparameters: number of channels, number of neurons in dense layer, dropout), LSTM (hyperparameter: number of units in dense layer, dropout), hierarchical recurrent neural network (row and column encoding - expected to work better for LOB because of the arrangement of price levels)
        - Hyperparameter tuning: randomized grid search
        - Evaluation: Multiclass accuracy, class-wise F1 score
        - Result: HRNN outperformed other models in all cases. However, it should be noted that: 1) training was very noisy because the sample size was limited to observations from 1 day, 2) HRNN was unable to outperform majority guess for ticker 3
    - Scaling up preprocessing and feature engineering of limit order book and applying deep learning across tickers to predict the direction of movement of VWAP [[PDF](research_final.pdf)]
        - Hypothesis: 1) multiprocessing is required to scale up preprocessing and feature engineering, 2) current snapshot of volumes at different price levels can be viewed as an image with colors and the variation with time can be considered as a stack of images
        - Tools and techniques for feature engineering: Python, dask, multiprocessing, R, parallel, dplyr, keras, R Shiny
        - Machine learning: deep convolutional neural network
        - Hyperparameter tuning: randomized grid search
        - Evaluation: Multiclass accuracy, class-wise F1 score
        - Result: CNN model **significantly** outperformed majority guess in all cases. But other tickers could not be added as covariates - `memoryError` on 16 GB RAM

## Knowledge Sharing

I share my knowledge through [my blog](https://medium.com/@snaveenmathew/) on Medium.com. My main focus is on the basic mathematical and statistical concepts behind machine learning. I also share my practical experience by explaining how mathematics helps in solving real-life problems.