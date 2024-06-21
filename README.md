# IMDB Movie Genre Prediction and Recommendation with BERT

## Overview
This project aims to leverage the advanced text analysis capabilities of BERT for better movie recommendations. Unstructured data, 
like movie reviews and introductions, remains underutilized despite its potential. By leveraging LLMs' sophisticated understanding of unstructured text, 
we aim to create a more nuanced recommendation system, enhancing user experience with personalized and insightful movie suggestions.

## Project Details
This project includes two parts, experimenting with two different use cases of BERT language model:

A. Semantic Search:
The first component of our recommendation system is based on semantic search. The objective is for users to input a description of the type of movies they are interested in 
(e.g., "romantic funny" or "anti-dystopian sci-fi movie"), and our database will return results that match the semantic meaning of the user's query. We use vector database ChromaDB
to store vector embeddings. There are two main differentiations. For one, our project focuses on the movie topic. We use movie synopsis as input text data. 
For another, we developed a simple web app to enable user interaction. 


B. Genre Classification:
The second part of our project aims to use the movie summary as a predictor to predict the movie genre. To do the genre classification using the BERT model, we referenced the paper 
‘Movie Genre Prediction based on the Bidirectional Encoder Representations from Transformer’. To process the image they use a CNN model, ResNet-50-2 from torchvision. 
Their experiment had an accuracy of 34.67%, a recall of 74.5%, and a F1 score of 0.4755. To improve the result, we tried another approach and method. 
It turns out that we have a better prediction accuracy of around 40%, but accuracy alone is not enough to evaluate a multi-label classification.

## Result
The details on evlauation matrix and our analysis is included in the project_report.pdf file. Please refer to the report for more detail. 

## Reference
https://medium.com/ai-science/build-semantic-search-applications-using-open-source-vector-database-chromadb-a15e9e7f14cehttps://www.kaggle.com/code/warcoder/chromadb-semantic-search
https://www.researchgate.net/publication/379004750_Movie_genre_prediction_based_on_the_bidirectional_encoder_representations_from_transformer 
https://www.kaggle.com/datasets/guru001/movie-genre-prediction/data
