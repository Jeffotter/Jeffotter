### Hi there 👋

My name is Jeff Ott, and I am a Engineer turned Data Scientist. I recently graduated USF's Masters in Data Science program. During this program, I've tackled many topics and projects. I will post what projects I can, but at the university's request, the code will not be readily available unless by specific request. I am interested in computer vision, deep learning, A/B testing, and using Data engineering to reinforce these interests.



### ADAS COG SCORE PREDICTION  <br>
Description: In work I did for the UCSF Brain Lab found here https://github.com/darenma/unet2021 we predicted ADAS Cog a memory exam given to patients to diagnose their cognative decline from 3D MRI volumes. This was done with a dual semantic segmentations unet to predict both matter types and Desikan Killany brain atlas parts. Using these data pipeline I also predicted the Adas Cog score. Below is the results from one of the segmentation pipelines <br>
Libraries Used: Pytorch, torchIO, Pytorch Lightning, Plotly, Sklearn <br>

| Parcellation | Raw MRIs
| ------------- | ------------- |
![ezgif com-gif-maker](https://user-images.githubusercontent.com/60712345/178179031-78fb6273-284e-4cc3-8ada-b003c02bdfe0.gif) | ![image](https://user-images.githubusercontent.com/60712345/178181131-31c59e98-18f3-4f42-9ac6-425507efd86b.png)



### Bot Town <br>
Description: Utilizing a GPT-2 Seq2Seq model I was able to recreate different podcast characters from the series critical role. I then added these bots to nodes which walked around and spoke to each othe. Their paths can be seen below. The full repository is found here. https://github.com/Jeffotter/BotTown <br>
Libraries Used: Pytorch,Pandas, NLTK, Matplotlib <br>


| Walking Characters | Sample Conversation 
| ------------- | ------------- |
![bottown](https://user-images.githubusercontent.com/60712345/178180541-74824dd1-03f7-4703-8be2-bed4aab27bdb.gif) | ![image](https://user-images.githubusercontent.com/60712345/178180660-5a0b65e4-8862-49b8-877d-261a7ca744e9.png)





### Data translation pipeline  <br>
Description: In this project we made some pyfiles to translate to different data types from command line <br><br>
<img width="509" alt="image" src="https://user-images.githubusercontent.com/60712345/161851380-3bef0ea3-8560-46c0-b48f-fc1c0e26d7c7.png"> <br>
*Libraries Used: sys, untangle, xmltodict, json*

### Search Engine Implementation <br>
Description: In this project we implimented a search engine with both linear search and hash table search then compared the differences between the two. We then created a local website on flask allow local users to access and use the engine <br><br>
<img width="711" alt="image" src="https://user-images.githubusercontent.com/60712345/161855175-0be40807-edf6-4241-8148-9d1938792bb5.png"><br>
*Libraries Used: Flask, doc2vec, Regex, Codecs, Numpy*

### TFIDF Document Summary <br>
Description: In this project, we processed zipped XML data (44M uncompressed, 9164 files), removed the XML, and tokenized the remaining strings. We developed a workflow that would calculate TFIDF (Term Frequency. inverse document Frequency) for each document. <br>
*Libraries Used: nltk, xml.etree.cElementTree, sklearn.feature_extraction.text, collection, zipfile, string

### Recommendation of Articles <br>
In this project, I was first introduced to word embeddings in the form of word2vec. I converted all the documents into embedding lists and found the centroids of each document. I then recommended documents based on euclidean distance. We then use flask, gunicorn, and jninja to build a scaleable website hosted on EC2 on AWS.<br><br>
![image](https://user-images.githubusercontent.com/60712345/163700421-ac099934-f0f7-4739-b00e-57118db89d7f.png)<br>
*Libraries Used: flask, doc2vec,re,string,numpy, codecs <br>

### Tweet Sentiment Analysis <br>
In this project, I learned how to mine Twitter data and perform sentiment analysis to find the user's average sentiment through a search. I then hosted this website on EC2 and let users search for the average sentiment on any public Twitter handle. This introduced me to website API and classifying sentiment from raw text. <br><br>
![image](https://user-images.githubusercontent.com/60712345/163700854-d423e284-d7e2-42c7-8ce4-e2bb6859aff0.png)<br>
*Libraries Used: flask, tweetie,colour,numpy, tweepy, vadarSentiment <br>


## Zillow Housing Prediction (Time Series) <br>
In this project, we attempted to predict median housing prices in California using the unemployment and Mortgage rate as helper variables. We tried three different models on the data ETS, SARIMAX, and FB Prophet. We were able to get a moderately good prediction with an RMSE of $7720. The methods and results are displayed in the Zillow Housing Prediction PDF. <br><br>
![image](https://user-images.githubusercontent.com/60712345/163701462-0f53bbfc-664f-4f2e-bc1e-146c0ba06792.png)<br>
*Libraires Used: Pandas, Numpy, statsmodels, fbprophet, tqdm, sklearn, pmdarmia, matplotlib

## Linear Models <br>
I implemented OLS, L2 regularization, and logistic regression in this project. I created functions to normalize the data and compute the loss gradient w/ without regularization. I then utilized these functions to make LogisticRegression, Linearegression, and Ridgeregresison classes.<br>
![image](https://user-images.githubusercontent.com/60712345/163701679-685d81f0-cbc2-4a39-aaf9-a4931e2dc267.png)<br>
*Libraries Used: pandas, numpy <br><br>

## Naive Bayes<br>
In this project, I built a multinomial Naive Bayes classifier to predict whether a movie review was positive or negative. I used Laplace smoothing to deal with missing words and vectorized operation to increase speed. I then used K_fold cross-validation class I coded to train the model and compare it against Sklearn. I was able to achieve a 80% accuracy with this model <br>
![image](https://user-images.githubusercontent.com/60712345/163702511-6f5f6740-3063-40fa-9de2-6169b8765109.png)<br>
*Libraries Used: sklearn, numpy, time, codecs, re <br><br>

## Decison Trees<br>
I attempted to recreate Sklearn Decision trees using recursively constructed trees in this project. I implemented LeafNode, DecsionNodes, Decision tree classes, and split using Gini impurity for classification and MSE for regression. I then inherited these classes in my RegressionTree and ClassifierTree functions. I compared these with the Sklearn implementations and got with a small margin of error. <br>
![image](https://user-images.githubusercontent.com/60712345/163702913-a9f92d76-3627-4832-bc5e-f7494939fb56.png)<br>
*Libraries Used: numpy, scipy.stats, lolviz <br><br>

## Random Forest<br>
Using my decision tree implementation from before. I was tasked with combining these trees with building a random forest. I built  RandomForestRegressor and RandomForestClassifier classes. I had to implement bootstrapping, subsampling, Out-of-bag error estimation, and random forest prediction to get comparable accuracy to Sklearn.<br>
![image](https://user-images.githubusercontent.com/60712345/163703319-bb065869-65d4-4513-86ad-1f919d78ac83.png)<br>
*Libraries Used: numpy, scipy.stats, lolviz <br><br>


<!-- ## OO hash table implimentation <br> 
In this 
Libraries Used:

## Clustering <br>
Libraries Used:

## Feature Importance <br>
Libraries Used:

## Multi Class Logistic Regression Implementation <br>
Libraries Used:

## Feature Engineering <br>
Libraries Used:

## ML Metric Understanding <br>
Libraries Used:

## A/B Testing hypothetical UI optimization problem inspired by Netflix <br>
Libraries Used:

## Gradient Boosted Neural Networks -->
