# Kaggle-DonorsChoose-Application
It is a project on kaggle DonorsChoose.org prediction, which applies a lot of nltk and nlp knowledge.
The model might need 140 mins to train the nlp model and do predictions on kaggle, score was 0.77703(top 40%).

Since I can't upload the whole training and test dataset onto GitHub, please refer to kaggle for the code running: https://www.kaggle.com/bogikidd/nltk-and-gru-on-donorschoose-org

Will do some more data engineering to try to make the prediction better in the near future

Update: Join the numerical data into training phrase as the last dense layer and make the processing time go up to 210 mins and score improve by 0.01 (0.78922, top 30%).

Update: The model with just GRU and numerical items performed even better than the ensemble model with one more set of CNN layers. I think the main reason is that the length of the text varies a lot, and that makes the model put too much efforts on the padding words but learning nothing. So the CNN make the model kind of overfitting.
Newest try without CNN ensemble (ver.9): **0.79172**, slightly better and faster than the ensemble model (ver.8): **0.78922**
