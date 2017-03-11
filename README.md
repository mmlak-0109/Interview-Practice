# Interview-Practice
Interview practice project #1

## 1. Describe a data project you worked on recently.

  The data project I worked on most recently was one called "Explore and Summarize Data".  In this project I used R to explore a dataset containing financial contributions made by California residents to Presidential candidates in the 2016 Presidential election.  After lookin thtough the 19 variables I decided that only four of the existing variables would be useful to my analysis.  Those four variables were the names of the candidates, the cities where the contributions came from, the the occupation of the people who donated, and the donation amounts.  Howeever, because there were far too many individual occupations to easily graph and examine, I ended up writting a function that used information from the United States Census Bureau that used the North American Industry Classification System to group the occupations into categories based on industy groupings. I also wrote functions and created variable for the candidates political party.  So in total, I used five variables for my analysis.  I then began my analysis by plotting the counts of all five variables and moved on to get the total donation amounts for the other four variables.  To finish up, I analysed total donation amounts for combinations of variables (ex. donation amounts given to each political party by occupation).


## 2. You are given a ten piece box of chocolate truffles. You know based on the label that six of the pieces have an orange cream filling and four of the pieces have a coconut filling. If you were to eat four pieces in a row, what is the probability that the first two pieces you eat have an orange cream filling and the last two have a coconut filling?


| Total Pieces | Orange Cream | Coconut Filling |
| :---: | :---: | :---: |
| 10 | 6 | 4 |

| P(1st Orange Cream) | P(2nd Orange Cream) | P(1st Coconut Filling) | P(2nd Coconut Filling |
| :---: | :---: | :---: | :---: |
| 6/10 | 5/9 | 4/8 or 1/2 | 3/7 |

In order to find the probability of this exact sequence, the probabilities above need to be multiplied together:

```
6/10 * 5/9 = 30/90 or 1/3

1/2  * 3/7 = 3/14

1/3 * 3/14 = 3/42 or 1/14
```
 
| **Answer** | 
| --- |
| 1/14 or 0.07 |

### Follow-up question: If you were given an identical box of chocolates and again eat four pieces in a row, what is the probability that exactly two contain coconut filling?


## 3. Given the table users:

     Table "users"
| Column | Type |
| --- | --- |
| id | integer |
| username | character |
| email | character |
| city | character |
| state | character |
| zip | integer |
| active | boolean |

construct a query to find the top 5 states with the highest number of active users. Include the number for each state in the query result. Example result:

| state | num_active_users |
| --- | --- |
| New Mexico | 502 |
| Alabama | 495 |
| California | 300 |
| Maine | 201 |
| Texas | 189 |

```SQL
SELECT state, COUNT(*) AS num_active_users FROM users
WHERE active = TRUE
GROUP BY state
ORDER BY num_actve_users DESC
LIMIT 5
```

## 4. Define a function first_unique that takes a string as input and returns the first non-repeated (unique) character in the input string. If there are no unique characters return None. Note: Your code should be in Python.

```python
def first_unique(string):
 # Your code here
 return unique_char

> first_unique('aabbcdd123')
> c

> first_unique('a')
> a

> first_unique('112233')
> None
```
```python
def first_unique(string):
 
 return unique_char
```

## 5. What are underfitting and overfitting in the context of Machine Learning? How might you balance them?
  With machine learning, the goal is to use an algorithm to try and classify data points into groups depending on the charachteristics of the data points.  For example, let's say you have some datFirst you train your algorithm on some training data, and then you test your data on new data.
  Underfitting is when your algorithm is not able to correctly identify the
  
## 6. If you were to start your data analyst position today, what would be your goals a year from now?
