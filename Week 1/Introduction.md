### Machine Learning

- Grew out of work in AI
- New capability for computers

### Examples

- Database mining

      Large datasets from growth of automation/web
      
      E.g., Web click data(网络点击数据), medical records, biology, engineering

- Applications can't program by hand(不能通过手工编程实现)

      E.g., Autonomous helicopter, handwriting recognition(手写识别), most of Natural Language Processing(NLP)（自然语言处理),Computer Vision(计算机视觉). 

- Self-customizing programs

      E.g., Amazon Netflix product recommendations

- Understanding human learning(brain, real AI)

Machine Learning definition

- Arthur Samuel. Machine Learning: Field of study that gives computers the ability to learn without being explicitly programmed.
- Tom Mitchell Well -posed Learning Problem: A  computer program is said to learn from experience E with respect to some task T and some performance measure P, if its performance on T, as measured by P, improves with experience E.

Machine learning algorithms:

- Supervised learning(监督学习)
- Unsupervised learning(无监督学习)
- Others: Reinforcement learning(强化学习), recommender systems(推荐系统).
- Also talk about: Practical advice for applying learning algorithms

### Supervised Learning

---

In supervised learning, we are given a data set and already know what our correct output should look like, having the idea that there is a relationship between the input and the output.

Supervised learning problems are categorized into "regression" and "classification" problems. In a regression problem, we are trying to predict results within a continuous output, meaning that we are trying to map input variables to some continuous function. In a classification problem, we are instead trying to predict results in a discrete output. In other words, we are trying to map input variables into discrete categories.

**Example 1:**

Given data about the size of houses on the real estate market, try to predict their price. Price as a function of size is a continuous output, so this is a regression problem.

We could turn this example into a classification problem by instead making our output about whether the house "sells for more or less than the asking price." Here we are classifying the houses based on price into two discrete(离散的) categories.

**Example 2**:

(a) Regression - Given a picture of a person, we have to predict their age on the basis of the given picture

(b) Classification - Given a patient with a tumor, we have to predict whether the tumor is malignant or benign.

Exercise

![1](https://github.com/ntgoaywh/Machine-Learning-Note/blob/main/Week%201/image/example1.png?raw=true)

### Unsupervised Learning

Just give datasets. 

In unsupervised learning, we're given data that looks different than data that looks like this that doesn't have any labels or that all has the same label or really no labels.

Unsupervised Learning algorithm may break these data into these two separate clusters.(两个不同的聚类). So this is called a clustering algorithm.(聚类算法)

Eg: 

- Organize computing clusters
- Social network analysis
- Market segamentation
- Astronomical data analysis

Clustering algorithm is just one type of Unsupervised Learning. 

Eg: Cocktail party problem algorithm

Just use the following code

```python
[W,s,v]=svd((repmat(sum(x.*x,1),size(x,1),1).*x)*x'
```

[GNU Octave](https://zh.wikipedia.org/wiki/GNU_Octave)

 

![2](https://github.com/ntgoaywh/Machine-Learning-Note/blob/main/Week%201/image/example2.png?raw=true)

Summary

Unsupervised learning allows us to approach problems with little or no idea what our results should look like. We can derive structure from data where we don't necessarily know the effect of the variables.

We can derive(源于，得出) this structure by clustering the data based on relationships among the variables in the data.

With unsupervised learning there is no feedback based on the prediction results.

**Example:**

Clustering: Take a collection of 1,000,000 different genes, and find a way to automatically group these genes into groups that are somehow similar or related by different variables, such as lifespan, location, roles, and so on.

Non-clustering: The "Cocktail Party Algorithm", allows you to find structure in a chaotic environment. (i.e. identifying individual voices and music from a mesh of sounds at a [cocktail party](https://en.wikipedia.org/wiki/Cocktail_party_effect)).
