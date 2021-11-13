# Detect_Fake_Accounts
The project idea is to detecting fake accounts or like on any post via Instagram by simple steps, Log in by your Instagram account and then search by username to the person you want to check their followers or post's likes and then apply the model which got 95% accuracy anf finaly you got the results.

## Dataset
the dataset is very simple and does not contain alot of information, the information below explain each feature:
- profile pic: does the user have a profile picture? 1 is true, 0 otherwise
- nums/length username: ratio of numerical to alphabetical characters in the username
- fullname words: how many words are in the user's full name?
- nums/length fullname: ratio of numerical to alphabetical characters in the full name
- name==username: is the user's full name the same as the username? 1 is true, 0 otherwise
- description length: how many characters is in the user's Instagram bio?
- external URL: does the user have an external URL linked to their profile? 1 have an external URL, 0 otherwise 
- private: is the user private? 1 is private, 0 otherwise
- posts: number of posts
- followers: number of people following the user
- follows: number of people the user follows
- fake: if the user is fake, fake=1, else fake=0, This is the target

there are none Null values in the dataset, and the dataset is fully cleaned.

the information below shows the corralation of the features to the target which is fake:
fake                    1.000000
profile pic             0.637315
nums/length username    0.587687
description length      0.460825
external URL            0.362809
fullname words          0.298793
nums/length fullname    0.246782
#posts                  0.245355
#follows                0.224835
name==username          0.170695
#followers              0.093689
private                 0.028586

for that the features #followers and private are useless since its does not have huge influence to the fake feature

## Model
To choose the best answer we apply for different model and the table below shows what the results:
|  Classifier | Accuracy|recall|Precision|f1-score|
| ------------- | ------------- | ------------- | ------------- | ------------- |
|Logistic Regression|0.95|0.95|0.95|0.9501|
|KNN Classifier|0.867|0.893|0.834|0.862|
|Decision Tree  Classifier|0.91|0.89|0.933|0.911|
|Random Forest Classifier |0.916|0.916|0.916|0.916|

and from the table above its shows that the Logistic Regression is the best mocel that fit this [dataset]() and it's greate reslut


## Tools

- Numpy and Pandas for data manipulation
- Scikit-learn for modeling
- Matplotlib, Seaborn for plotting

# Communication
slides and visuals presented are avalible [here]() that present the work nicely
