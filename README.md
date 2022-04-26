# Data Mining Project (Recommendation System)
## Aim:
The aim of this project is to build a recommendation system for
E-commerce websites like Amazon and Flipkart. We plan to extend the use
of the recommendation system to any website or application that involves
getting ratings from users like OTT platforms such as Netflix and Prime
Video. The main idea revolves around comparing user ratings for similarity
and using the coefficient we get as a result of taking the cosine product of
two vectors containing the user ratings (also known as Pearson
Correlation) as a measure to predict the expected rating of a previously
non purchased product and displaying a list of products that the
customer is most likely to purchase.


## Dataset:
Here’s the link to the dataset we plan on referring to: 

[Kaggle Dataset](https://www.kaggle.com/arhamrumi/amazon-reviews-eda-20012018)

This dataset contains more than 180M consumer reviews on different
amazon products. It is divided into 15 categories: magazine subscriptions,
beauty, fashion, appliances, cell phones and accessories, digital music, gift
cards, grocery and gourmet food, industrial and scientific, musical
instruments, software, sports and outdoors, toys and games, video games.

The dataset we use has the following attributes: rating, verification status
of the review, reviewer ID, product ID,date of review, and votes. However, for
our analysis the relevant attributes are rating, reviewer ID, product ID. To
train our model, we plan to use the Sports and Outdoors csv for our initial
analysis.

## Techniques used (state of the art):
We have identified the main algorithms involved in our project as
Collaborative Filtering using matrix factorization. The idea is to use
Collaborative filtering to build the model. Any further means of
optimization or general improvement in the project will be taken care of as
and when we go through the development phases of the project.


## Collaborative filtering:
This is an algorithm which uses the fact that certain users or certain items
can be similar to each other and their similarity could be the key to
identifying what recommendations the model would give to a certain user.
Here’s how it works -

There are two ways to look at collaborative filtering:
1) We look at the similarities between two users, also known as User -
User collaborative filtering
2) We look at the similarities between two items, also known as Item -
Item collaborative filtering

#### What’s the general idea involved?
Both methods work on the method of calculating a factor known as
Pearson correlation coefficient. We can take the ratings a certain user has
given for a set of items and make a vector of the data. We take the dot
product of the vectors of two users to calculate the Pearson coefficient.
A similar idea works for Item - Item collaborative filtering.


The method we choose is Item - Item collaborative filtering. The reason is
that the Item - Item method has been observed to be more useful in terms
of accuracy than the User - User method. An Item-based collaborative
filtering finds the utility matrix which provides us with measures of
similarity between items based on user ratings. We predict the rating which
might be given by user X to item I, by finding out the items rated by x which
are similar to I. Based on those rating values, we estimate the rating for
item I by user X.
### Advantages of Collaborative filtering system -
* There is no need to consider the features of the items while filtering
out the items.

### Disadvantages of Collaborative filtering system -
* If the data points are sparse, then we won’t get enough rating values
to predict the unknown rating. However, we resolved this issue by
taking a large enough dataset.
* Some items might be added later or they may have very few buyers. A
convenient way to resolve this by performing a linear combination of
a baseline estimate and a collaborative filtering system .

## Team Members:
* [Milind Jain - 2020A7PS0153H](https://github.com/jainmilind)
* [Ashwin Naveen Pugalia - 2020A7PS1080H](https://github.com/Ashwin-1709)
* [Ashwin Arun - 2020A7PS1291H](https://github.com/CodeFreak2002)
* [Arkishman Ghosh - 2020A7PS2077H](https://github.com/ArkiGhosh)
