# IMDB_movie_reviews_analysis
ML cleaning, modeling, and analysis of IMDB movie review dataset examing positive and negative sentiments. The file for the IMDB dataset used is linked below and was too large to host on Github.

https://drive.google.com/file/d/15DFQLC1FzDrxZeQ7CmxVJQBRS-7pfuUk/view?usp=sharing

## Conclusions

Several of the models, out of the six created, reached or exceeded the F1 threshold value of .85. In descending order, they were model_1, model_4, model_3, and model_5. Hyperparameter tuning or adding GridSearchCV to the model pipelines could result in better performing models, but there was no need for that.

Model_1 did not perform best with the sample of my_reviews. Model_3 and model_5 performed the best as shown in the graph above. The best overall model would probably be model_3 (Bag of Words and LogisticRegression) due to its performance on the test set, the my_reviews sample, and the low level of complexity and time needed for model training.

There was also no need to balance the classes in this case. Again, we could do that if we wanted to increase the performance, but it was not necessary to reach the threshold value. Both balancing the classes and hyperparameter tuning allow for east routes for improving model performance should there ever be a need to revisit and refine this code.

The BERT embeddings algorithm consistently crashed this notebook so it was not included in the final product.
