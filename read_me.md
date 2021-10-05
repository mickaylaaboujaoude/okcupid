# OKCupid Profiles Data

## Introduction
I just found this OKC profiles data on Kaggle because I was just thinking to myself how it would be fun to play around with dating profile data, and then I found some! With apparently 59946 rows! I hope the data isn't clean because it would be fun to clean it, but it probably is clean because it seems like the data is for intro stats students. We'll have to see!

This project is sort of my creative exploratory space. 

I am also still getting acquinted with best practices regarding using git and Jupyter Notebook. 


## About Data
I obtained the data from Kaggle. It was posted by Larxel. 
Link to Kaggle Source: 
https://www.kaggle.com/andrewmvd/okcupid-profiles

Originally, the data came from Professors Albert Y. Kim and Adriana Escobedo-Land, both of whom were at Reed College at the time. It appears they struck a deal with OKC and were able to obtain some OKC data for use by statistics students. Names and any other personally identifiable information were removed by data authors. 

Link to actual data source: 
https://github.com/rudeboybert/JSE_OkCupid
Link to Journal of Statistics Education article regarding data,"OkCupid Data for Introductory Statistics and Data Science Courses": https://doi.org/10.1080/10691898.2015.11889737

### The following is an excerpt form the "OkCupid Data for Introductory Statistics and Data Science Courses"
*2 Data
The data consists of the public profiles of 59,946 OkCupid users who were living within 25 miles of San
Francisco, had active profiles during a period in the 2010s, were online in the previous year, and had at least
one picture in their profile. Using a Python script, data was scraped from users’ public profiles four days
later; any non-publicly facing information such as messaging was not accessible.
Variables include typical user information (such as sex, sexual orientation, age, and ethnicity) and lifestyle
variables (such as diet, drinking habits, smoking habits). Note that random noise was added to the age
variable for de-identification purposes.*

*Furthermore, text responses to the 10 essay questions posed to all OkCupid users are included as well,
such as “My Self Summary,” “The first thing people usually notice about me,” and “On a typical Friday
night I am...” However, the essay data has been randomized by rows to decouple them from the profiles data.
In other words, the user represented in the first row of profiles_revised does not necessarily correspond
to the user that wrote the responses in the first row of essays_revised_and_shuffled.*

*For a complete list of variables and more details, see the accompanying codebook okcupid_codebook.txt.*

##### On the essay variables
Note that in the second paragraph in the excerpt above, and in okcupid_codebook.txt, it is implied that the the values for each essay question variable, while randomized to separate them from the original poster, are correctly grouped by question. 

However, Larxel implies something different in a comment on their Kaggle post. 

Larxel's comment:

*Hello,*

*You might have noticed there are 10 essay columns in this dataset and they relate to open text fields within the app.
Thing is, they are not necessarily in order, so any essay column could have any of the following open text fields:*

*About Me / Self summary
Current Goals / Aspirations
My Golden Rule / My traits
I could probably beat you at / Talent
The last show I binged / Hobbies
A perfect day / Moments
I value / Needs
The most private thing I'm willing to admit / Secrets
What I'm actually looking for / Dating
It was a choice made by the authors, and it was too much to put into the description text*

*Hope it helps*

It seems that Larxel is saying that a given essay variable might hold answers to several different questions, as opposed to just one question.I'm not sure what to make of this, and maybe I'm misunderstanding and both the data owners and Larxel are actually saying the same thing. But it seems like something I might want to explore further later when I start to play around with the essay variables. 

## Data Citation
(I'm not sure where to put this, so I'm putting it here)

@article{article,
author = {Kim, Albert and Escobedo-Land, Adriana},
year = {2015},
month = {07},
pages = {},
title = {OkCupid Data for Introductory Statistics and Data Science Courses},
volume = {23},
journal = {Journal of Statistics Education},
doi = {10.1080/10691898.2015.11889737}
}
