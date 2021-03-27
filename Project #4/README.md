# Wrangle and Analyze Data Project


In this project, my goal is to wrangle and analyze @dog_rates.
@dog_rates Is a twitter account, that collects human's dog ( pics, name, stage) something like that, and write comment and rating. 



## The first step of the wrangle, is gathering :

Here I used three datasets.
1- Enhanced Twitter Archive : which contains the basics of data tweets.
2- Image Predictions File: which i loaded it programmatically from udacity server.
3- Additional Data via the Twitter API : which I read ( tweet_json.txt ) because I don't have twitter authorization yet. 


## The second step of the wrangle, is assessing :

at this step, I took an overview of datasets. Using some methods like info, describe, head, tail, and others. then I took sum assessing.


### Quality Issues: 

 at Enhanced_twitter Dataset:
Dtype of tweet_id column is int64.
181 retweeted in dataset.
There are numbers other than 10 in rating_denominator column.
"None" at name column is inconsistent, it's better to be NaN.

at Image-predictions Dataset:
Dtype of tweet_id column is int64.
There 66 duplicated at jpg_url column.
p1_dog, p2_dog, p3_dog columns have False Predicted.

at Tweet-json Dataset: 
Dtype of id column is int64.
column name of id , it's better to be tweet_id

### Tidiness Issues:
at Enhanced_twitter Dataset :
- The dog stage (doggo, floofer, pupper, and puppo) at 4 columns rather than one.
at Image-predictions Dataset
- It’s better to merge it with Enhanced_twitter Dataset
at Tweet-json Dataset
-It’s better to merge it with Enhanced_twitter Dataset

## The last step of the wrangle, is cleaning :

Which consists of three stages:
Define : Definition of the Issue and how to solve it.
Code : solve the Issue programmatically.
Test : Make sure that the issue is solved.


## By the end of these three stages, that means the wrangle stage has ended.
Next is to analyze and visualize.
