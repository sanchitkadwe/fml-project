# Music Genre Classification - Team Musica

## Team Details
23M0831 Chaitra Gurjar <br>
24M0836 Sanchit Kadwe<br>
24M0847 Vansil Chauhan <br>
24M0848 Shalaka Thorat

## Overview
<ul>
<li>This project aims to classify music tracks into different genres using machine learning techniques.</li>
<li>The GTZAN dataset contains 10 genres with 100 tracks each, totalling 1000 tracks.
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
6) Overall, we achieved a Validation Accuracy of 95%, so we finalized this Classifier Model and built a web app to provide predictions on test audio files.


## CNN Model Architecture
<img width="500" alt="image" src="https://github.com/sanchitkadwe/fml-project/blob/main/CNN%20Model%20Architecture/Model%20Overview.png">
Detailed Model Implementation (Layers & Parameters) : Click <a href="https://github.com/sanchitkadwe/fml-project/blob/main/CNN%20Model%20Architecture/Model%20Layers.png">Here</a>

## Results
Following are the Accuracy and Loss Plots for the Model:<br>
<img width="400" alt="image" src="https://github.com/sanchitkadwe/fml-project/blob/main/Output%20Graphs/Accuracy%20Graph.png">
<img width="420" alt="image" src="https://github.com/sanchitkadwe/fml-project/blob/main/Output%20Graphs/Loss%20Graph.png"><br>
Confusion Matrix and Classification Report can be found <a href="https://github.com/sanchitkadwe/fml-project/tree/main/Output%20Graphs">Here</a>

## Accuracy Comparison of various Algorithms
<table border="1" style="border-collapse: collapse; text-align: center;">
    <tr>
        <th>Algorithm</th>
        <th>Using 3 sec Audio File Data</th>
        <th>Using 30 sec Audio File Data</th>
    </tr>
    <tr>
        <td>SVM</td>
        <td>85.3</td>
        <td>69</td>
    </tr>
    <tr>
        <td>Decision Tree</td>
        <td>64.2</td>
        <td>46.6</td>
    </tr>
    <tr>
        <td>Random Forest</td>
        <td>86.1</td>
        <td>66.6</td>
    </tr>
    <tr>
        <td>Logistic Regression</td>
        <td>73.3</td>
        <td>69.3</td>
    </tr>
    <tr>
        <td>KNN</td>
        <td>88.7</td>
        <td>65.3</td>
    </tr>
    <tr>
        <td>CNN using Mel-Spectrograms</td>
        <td>NA</td>
        <td>95.29</td>
    </tr>
</table>


## Enhancements Done with Reference Models that boosted Accuracy:
1) Alternating Filter Sizes of 3 x 3 and 5 x 5 for Convolution Layers
2) Additional Dense Layer of 256 units in a Fully Connected Block
3) 'Padding=same' kept for all Convolutional Layers
4) Modified Random Seed for Train-Test-Split
5) Changed the Number of Epochs

## Web-App
The web app for Music Genre Classification can be accessed <a href="https://cs725-genreclassifier.streamlit.app/">HERE</a><br><br>
<img width="872" alt="image" src="https://github.com/user-attachments/assets/34cfb690-6ace-4fad-803d-d4bdada7eee0">
