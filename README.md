# DMML2022_-Orange-

### Team members : 
Aïssa Meziani and Anaïs Bodénès

### Project description : 
The goal of this project is to create a classifier that predicts how the level of some text in French (A1,..., C2).

### Approach :

1) First we upload all data and patterns needed.

2) We analyse the data for checking if there were problems in our dataset, however there was nothing to check (NaN values, outliers...) so it was quick.

3) Then we applied models studied in lectures and Lab : logistic regression, KNN, decision tree and random forest. We have started by vectoring our text data with the pipeline vectorizer.

4) We looked for hyperparameters for kNN, Decision tree and random forest classifier. It gives the same results for kNN classifier, with decision tree it gives us more realistic results and with random forest we note an negligeable reduction of accuracy train score otherwise the rest of results was the same.

5) We found an other model which reveals being our best model : "the support vector classifier".

6) We combined our best models : logistic regression and SVC, but the result was just lower than with the SVC's model.

7) We had until there a classical approach but it wasn't enough efficiency to achieve the project, so we decided to use text embeddings.
Nevertheless, it wasn't so efficient for one of our best model (logistic regression), then we didn't used it for the rest of our models.
Meanwhile, we tried to implement data embeddings with the method "Word2Vec" and "Doc2Vec", but we met many problems and the results were worst than our original ones so we decided to not inculde this part of our work into our project.

8) Finally we fitted our model for the entire dataset, it rises from 2% to 4% our rank for all of our models.

### Summary of the results :

| | Logistic regression |kNN	| Decision Tree | Random Forests | SVC | Combination |
| ------------- | ------------- |----------| ------------- | ------------- |----------| -------|
| Precision |46.15|36.97| 29.15 | 37.19 |47.83| 46.54|
| Recall |46.46|34.84| 29.27 | 37.18 |47.60| 46.46|
| F1-score | 46.16|33.53| 28.98 | 36.87 |47.48| 46.17|
| Accuracy | 46.45 |34.89| 29.27 | 37.18 |47.61| 46.45|

### Link to explanatory video :

https://www.youtube.com/watch?v=E0DqL9c4aIU
