# Sentiment analysis for Youtube comments
## Introduction
This is a Big data analytics project that aim to use the sentiment analysis for youtube comments to achive two goals :
  1. Firstly, Check the level of positivity toeards the vedio.
      **Note**: positivity = the ratio between positive comments and the total number of comments
  2. Secondly, See the Category distribution of the vedio. In other words, the intersection of cateogries that the vedio belong to.
 
## Motivation 
* Comments and level of Engagement :
The level of engagement represented by the comments is much higher than by the reacts. Moreover,There is high correlation between  discussion rank and the number of comments.
In addition,The comments have more verification over the positivity or the negativity of the videos, compared  to the reacts. The following image illustrate the level of engagement on social media:

![7levels](https://github.com/MG-98/-Sentiment-analysis-for-Youtube-comments/blob/main/images/7levels.png)

* Multi-Category problem :
People ,definitely, has interest in more than one category through their  experience in Youtube
Video with one category doesn’t narrow down sufficiently for the individuals

 ## Dataset
  1. We grabbed dataset from the [Youtube API](https://developers.google.com/youtube/v3/docs).
  2. Kaggle Dataset: [Youtube video statistics for 1 million videos](https://www.kaggle.com/mattiazeni/youtube-video-statistics-1million-videos)
 
 ## Model final detials
 * Sentiment analysis for youtube comments
     1. Tokenization (text toward tokens(words))  
     2. Count vector (CountVectorizer converts text documents to vectors which give information of token counts.)
     3. idf (Numerical measure of how much information a terms provide)
     4. indexer (convert the targets into labels)
     5. Logistic regression classifier 

* Videos multi-category distribution 
        
    1. Tokenization (text toward tokens(words))  
    2. Count vector (CountVectorizer converts text documents to vectors which give information of token counts.)
    3. indexer (convert the targets into labels)
    4. Logistic regression classifier 
    
## Results 
* Sentiment analysis for youtube comments

    ```Train accuracy  : 0.7972536860089856  , Test accuracy : 0.7964978111319575```
    
 The following bar chart shows the correlation between  positivity and the average number of likes:
 Comment : This is perfect as it follows the normal distribution which gives a good intution.
 ![pos](https://github.com/MG-98/-Sentiment-analysis-for-Youtube-comments/blob/main/images/pos.png)

* Comments category distribution

    ```Train accuracy  : 0.83015 ```
    
    1. [Harry Styles - The Chain (Fleetwood Mac cover) in the Live Lounge](https://www.youtube.com/watch?v=eM_FR7I2Ttw)
   ![ex2](https://github.com/MG-98/-Sentiment-analysis-for-Youtube-comments/blob/main/images/2nd.png)
    
    2. [ What Hillary Clinton really thinks ](https://www.youtube.com/watch?v=GGm0FQ6i74U&t=9s)
        
        ![ex1](https://github.com/MG-98/-Sentiment-analysis-for-Youtube-comments/blob/main/images/1example.png)

    3. [BIG ANNOUNCEMENT ON MY POPSCICLE](https://www.youtube.com/watch?v=brfJuyTADuQ)
        
        ![ex3](https://github.com/MG-98/-Sentiment-analysis-for-Youtube-comments/blob/main/images/3rd.png)
