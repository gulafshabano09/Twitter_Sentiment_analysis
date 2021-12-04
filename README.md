# Twitter_Sentiment_analysis
Twitter Sentiment Analysis is the process of computationally identifying and categorizing tweets expressed in a piece of text, especially in order to determine whether the writer’s attitude towards a particular topic, product, etc. is positive, negative, or neutral.

## Twitter Sentiment Analysis

**Lets start with importing the libraries**
![t1](https://user-images.githubusercontent.com/95492893/144718252-bf442964-e5f1-42ac-b400-8d9649cfc80a.PNG)

## Download the data set

![t2](https://user-images.githubusercontent.com/95492893/144718280-c3e713c9-7918-4df6-9cd4-3d673ebd8230.PNG)

**First of all, splitting the data set into a training and a testing set. The test set is the 10% of the original data set.**

**For this particular analysis I dropped the neutral tweets, as my goal was to only differentiate positive and negative tweets.**
![t3](https://user-images.githubusercontent.com/95492893/144718324-22c0ae7b-a806-4152-8c21-174095666fb3.PNG)

As a next step I separated the Positive and Negative tweets of the training set in order to easily visualize their contained words.

After that I cleaned the text from hashtags, mentions and links. Now they were ready for a WordCloud visualization which shows only the most emphatic words of the Positive and Negative tweets.

![t4](https://user-images.githubusercontent.com/95492893/144718375-a892ecaf-7828-4f22-8f36-bec8d3b9ab19.PNG)
![t5](https://user-images.githubusercontent.com/95492893/144718405-adac097b-0781-4b22-83cd-ba742627c1e3.PNG)

![image](https://user-images.githubusercontent.com/95492893/144718413-0067b4b3-009e-4ff4-9551-9352ec0009b2.png)

![image](https://user-images.githubusercontent.com/95492893/144718422-b95755b2-300f-4dbf-ad70-ef9ab37378e4.png)

Interesting to notice the following words and expressions in the positive word set: truth, strong, legitimate, together, love, job

In my interpretation, people tend to believe that their ideal candidate is truthful, legitimate, above good and bad.

At the same time, negative tweets contains words like: influence, news, elevatormusic, disappointing, softball, makeup, cherry picking, trying

In my understanding people missed the decisively acting and considered the scolded candidates too soft and cherry picking.

After the vizualization, I removed the hashtags, mentions, links and stopwords from the training set.


Stop Word: Stop Words are words which do not contain important significance to be used in Search Queries.

Usually these words are filtered out from search queries because they return vast amount of unnecessary information. ( the, for, this etc. )

![t6](https://user-images.githubusercontent.com/95492893/144718483-5bf72c5e-22ed-4486-8c00-019b6930ff14.PNG)
![t7](https://user-images.githubusercontent.com/95492893/144718538-2adf44c7-5393-4d14-bd42-6977640f6590.PNG)

As a next step I extracted the so called features with nltk lib, first by measuring a frequent distribution and by selecting the resulting keys.

![t8](https://user-images.githubusercontent.com/95492893/144718581-0bdc07d4-0894-4dc9-b894-345b20b5288a.PNG)
![t9](https://user-images.githubusercontent.com/95492893/144718612-00ee48e2-48a3-44ff-84af-e0a35cec5691.PNG)

Hereby I plotted the most frequently distributed words. The most words are centered around debate nights.

**wordcloud_draw(w_features)**
Using the nltk NaiveBayes Classifier I classified the extracted tweet word features.

![t10](https://user-images.githubusercontent.com/95492893/144718708-2829da48-3dc7-4d64-a7d7-5b82033d6fea.PNG)

Finally, with not-so-intelligent metrics, I tried to measure how the classifier algorithm scored.

![t11](https://user-images.githubusercontent.com/95492893/144718755-d771a16a-97c3-43fe-a0e2-382629fe8d38.PNG)











