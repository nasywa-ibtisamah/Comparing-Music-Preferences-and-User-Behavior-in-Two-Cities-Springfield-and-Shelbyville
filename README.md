# Project Description

Hello there :wave:

Hope this project finds you well!

In this project, I will compare the music preferences of users in 2 cities (let say Springfield and Shelbyville). I will test the below hypotheses and compare user behaviour in the 2 cities.

**Hypotheses**
1. User activity varies depending on the day and city.
2. On Monday mornings, residents of the both cities tune into a different genre. This also applies on Friday nights.
3. Listeners in 2 cities have different preferences. In Springfield, users prefer pop music, while in Shelbyville rap music has more fans.


# Steps

1. Exploratory Data Analysis
2. Pre-Processing Data
3. Hypothesis Testing

## 1. Exploratory Data Analysis

**Data Description** 

- `'userID'` — the unique ID of user
- `'Track'` — track name
- `'artist'` — artist name
- `'genre'` — genre name
- `'City'` — city where the user live in
- `'time'` — song duration
- `'Day'` — day name

Each of row contains data of the played song. 

## 2. Pre-Processing Data

There are several issues in dataset:
1. The naming convention is not consistent. I standardized it to snake_case and convert it to all lowercases.
2. Missing Values . I replaced the missing value with 'unknown'.
3. Duplicate Data. I removed it.
4. Duplicate Implicit in 'genre' = 'hiphop'. I made a function to standardize the duplicate implicit.

## 3. Hypothesis Testing

The result of each hypothesis:
1. User activity varies depending on the day and city. 

**In Springfield, the total number of musics played reached its peak on Monday and Friday. On Wednesday, users barely played musics**
**In Shelbyville, users played musics more often on Wednesday.**
**Overall, users activities on Monday and Friday are lesser than Wednesday**
**So, it is correct that user activity varies depending on the day and city.**

2. On Monday mornings, residents of both cities tune into a different genre. This also applies on Friday nights.

**Users that live in Springfield or live in Shelbyville mostly listen to the same genre as the top 5 most popular genres of music are mostly the same. The top genre in both cities is Pop.
BUT, due to many missing values in the data which user live in Shelbyville, 'unknown' become the 10th most popular genre.**
**This will cause bias in the hypothesis result**

3. Listeners in 2 cities have different preferences. In Springfield, users prefer pop music, while in Shelbyville rap music has more fans.

**Pop music is the most popular genre not only in Springfield, but also in Shelbyville. However, rap music is not included in the top 5 most popular in either Springfield or Shelbyville. So, the hypothesis is not correct for the music preference in Shelbyville**


# Conclusion

1. The 1st hypothesis is fully accepted.
2. The 2nd hypothesis is not accepted. 
3. The 3rd hypothesis is not accepted
4. This project has a weakness because in drawing the conclusion, I did not use Statistical Hypothesis Testing. 
