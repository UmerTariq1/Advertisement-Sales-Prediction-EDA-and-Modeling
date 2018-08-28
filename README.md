# Sales-Prediction
Implementation of Advertisement dataset

   bcf-usc advertisement dataset is a famous dataset for a regression problem. Data has 4 features TV,radio,newspaper and sale. The number of observations are 200. First 3 featuers are the advertisements shown in each sector (tv, newspaper or radio) and 4th feature i.e sales is the number of sales after the advertisement. The goal is to find the find the realtionship between advertisement and sales, and to predict the sales for a particular number of advertisement in each sector. 

I used Scikit-Learn, Pandas and numpy for this project.

 First I made a pairplot using seaborn library to find the realtionship between each feature manually and then I used pandas corealtion function to find the corealtion between each feature all toghether. I found that TV advertisments has the biggest impact on sales, then radio and then newspapaer has the lowest affect on the sales. Then I used linear regression model to predict the sales using different combination of features (considering the result we got in last of finding realtionship between features). 
  I ran linear regression 1000 times and calculated the average mean squared error (used it as a metric to calculate error) which was around 1.7 , I noticed that when I used only TV and radio features to predcit sales, I got better result than when used all features. Then I tried cross validation technique to find the best features for predicting the most accurate sales. I got 1.69 root mean squared error when I used all features and 1.67 when i used only tv and radio. 

This was one of the first datasets that I implemented and one of my first ML project, so I learnt many new things doing this project.

Dataset link: https://www.kaggle.com/purbar/advertising-data

