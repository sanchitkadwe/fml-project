# Music Genre Classification - Team Musica

## Team Details
23M0831 Chaitra Gurjar <br>
24M0836 Sanchit Kadwe<br>
24M0847 Vansil Chauhan <br>
24M0848 Shalaka Thorat

## Overview
<ul>
<li>This project aims to classify music tracks into different genres using machine learning techniques.</li>
<li>The GTZAN dataset is used, containing 10 genres with 100 tracks each, totalling 1000 tracks.
Dataset Link: <a href="https://www.kaggle.com/datasets/andradaolteanu/gtzan-dataset-music-genre-classification">Here</a></li>
<li>The 10 Prediction Categories are: Blues, Classical, Country, Disco, Hip-Hop, Jazz, Metal, Pop, Reggae, and Rock.</li>
<li>The main objectives are to preprocess the data, extract meaningful features, train a classifier using CNN, and evaluate its performance.</li>
</ul>

## Methodology
1) We first started by <a href="https://github.com/sanchitkadwe/fml-project/tree/main/Exploring%20CSV%20Data">Exploring CSV Data</a> from Data Files: features_30_sec.csv, and features_3_sec.csv, which included extracted features from the audio files.
2) We performed Feature Scaling and Data Cleaning and fed the data to various Classification Models.
3) These ML Models were: SVM, Decision Tree, Random Forest, Logistic Regression and KNN.
4) We obtained an accuracy of around 87%, but it couldn't be improved further.
5) Thus, we modified our approach to process Audio Files, <a href="https://github.com/sanchitkadwe/fml-project/tree/main/Exploring%20Mel-Spectrograms">Explore Mel-Spectrograms</a>, train them using CNN, and get accurate results.
6) In all, we achieved a Validation Accuracy of 94%, so we finalized this Classifier Model and built a web app to provide predictions on test audio files.
