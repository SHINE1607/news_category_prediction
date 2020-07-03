# news_category_prediction
Reading news papers has always been a part of our human life from the start of civilizarion. 
But it has been always a challenge to classify the news into categories, which was done maually 
for a long period. But with the technology advancements its never been this easier to classify 
stories. Now it has become a matter of time. 

This project uses NLP and word embedfing technique to classify the new stories into 4 catgories.

## Data description
  * The train data is faily simple that has 2 columns namely, SECTION and STORY
  * The section, which is the target variable, classiifies the story into 4 categories
  * train data has 7628 rows or stories
  
## Project time line
  * the story variable that has the news articles are tokenized and lemmatized 
  using the nltk.stem.WordNetLemmatizer function
  * the tokenized data is converted into onehot representation using 10000 features or 
  vocabulary size
  * the onehot reprsented data is converted to padded sequence
  * Padded sequence data is sent to keras neural ntework model

## model architecute
  
  ![alt text](https://github.com/SHINE1607/news_category_prediction/blob/master/model/image/Screenshot%202020-07-04%20at%2012.38.00%20AM.png)
      * the model uses softmax activation function for final layer
      * the model is compiled with stochastic graient descent optimzer and sprase categorical cross entropy loss function
  
 ## Data Prediction and accuracy
 
  * Data is predicted with an validation accuracy score of 95.28% 
  



