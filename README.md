
# Twitter Sentiment Analysis

[Click here to see a video about this work](https://youtu.be/BvfQq1-rpVc)

![senti](https://github.com/user-attachments/assets/ceebe3d1-7d63-4c86-957a-605c002e9235)


## Introduction
The objective of this project is to use machine learning to predict the sentiment of tweets or comments. In particular, the Twitter Sentiment dataset from Kaggle has been used to apply a **RandomForestClassifier** model. The goal is to accurately classify a tweet's sentiment as irrelevant, neutral, positive, or negative. To make the model accessible to users, **Streamlit** has been employed to develop a simple and interactive user interface.

-  **RandomForestClassifier**

As part of the ensemble learning approach, the RandomForestClassifier is a supervised machine learning algorithm used for classification tasks. Using randomly chosen portions of the training data, it generates multiple decision trees using a method known as bootstrap aggregating, or bagging. Decision trees are produced as a **"forest"** by this process. Instead of evaluating every feature as in an ordinary decision tree, the algorithm adds an extra layer of randomness during the construction of each tree by choosing a random subset of features to take into account when splitting nodes. 

The RandomForestClassifier runs each decision tree in the forest with the data to determine the classification of a new data point. A majority vote from each individual tree prediction determines the final classification. This approach ensures accuracy and robustness.

The main benefits of the RandomForestClassifier are that it can handle regression and classification problems, is more accurate than a single decision tree, and is robust to outliers and missing values. Compared to more complex models like neural networks, it is also easier to tune and understand. It also automatically manages feature importance, which makes it helpful for feature selection.

-  **Streamlit**
  
Streamlit allows for the rapid development of web applications for machine learning and data science projects. With this interface, users can enter any tweet or comment, and the application will instantly provide a sentiment prediction. This integration of Streamlit ensures that the sentiment analysis process is not only efficient but also user-friendly, enabling individuals without a technical background to easily interact with and benefit from the machine learning model.
## Documentation


- **Dataset**
[I've utilized the Twitter Sentiment dataset from Kaggle](https://www.kaggle.com/datasets/jp797498e/twitter-entity-sentiment-analysis)

## Screenshots**
- URL to visit on Streamlit UI
  
  ![Screenshot (2081)](https://github.com/user-attachments/assets/fd47c8b5-1366-4baf-ac56-9df4d0b0eac4)

- Enter your external IP address using the wget command
  
![Screenshot (2082)](https://github.com/user-attachments/assets/fdc46d4e-1457-4b24-9942-54a752ef9799)

- Streamlit UI
  
  ![Screenshot (2084)](https://github.com/user-attachments/assets/17612cfb-f5fb-4ea9-b15e-8d68d3bf97e5)


## Running Tests

- To get your external IP address, run the following command which should be pasted at Tunnel Password on URL to see UI

```bash
  !wget -q -O - ipv4.icanhazip.com
```

- To see Streamlit UI, run the following command

```bash
  !streamlit run app.py & npx localtunnel --port 8501
```
## Experimentation 
We have used 80% of our data to train the model and test it on the remaining 20%.

This approach is commonly known as an 80/20 train-test split, which is a standard practice in machine learning. It allows you to train your model on a larger portion of the data while still having a separate subset for testing to evaluate the model's performance on unseen data.
## Conclusion
In conclusion, this project successfully demonstrates the application of machine learning to predict the sentiment of tweets or comments. By leveraging the Twitter Sentiment dataset from Kaggle and implementing a RandomForestClassifier model, we have been able to classify tweets' sentiments as irrelevant, neutral, positive, or negative with a high degree of accuracy. After testing, the model has achieved an impressive **accuracy score of around 93%**. The integration of Streamlit provides a simple and interactive user interface, making the sentiment analysis tool accessible and easy to use for anyone, regardless of their technical expertise. This project not only showcases the effectiveness of ensemble learning methods in natural language processing but also highlights the importance of user-friendly applications in making advanced technologies accessible to a broader audience..

- Final prediction of some tweets....

![Screenshot (2085)](https://github.com/user-attachments/assets/317830ad-d66a-4d97-8240-7b99f244bf80)


