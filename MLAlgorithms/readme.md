# Supervised Machine Learning Algorithms 

This learning is defined by the use of **labeled data sets** to train algorithms that accurately classify data or predict outcomes. In this case, we will use supervised learning for **classification**, where algorithms help predict a discrete value. 

One can think of the **input data as a member of a particular class** or group. For example, if we take the photos from the fruit dataset, each photo has been labeled as a mango, an apple, and so on. In this case, the algorithm has to classify the new images into any of these categories.

**List of Algorithms we will use**
- K Nearest Neighbor
- Random Forest
- Linear Regression
- Support Vector Classifier

## What is it about?

This is an **itroductory work** to test some of the **most common supervised learning algorithms for classification** and to know how they work in a superficial way, in another repository dedicated to machine learning we will go deeper into these models. We will rely on the SkLearn library to use the models.

Also we will use the typical 'Iris' DataSet, which it includes three iris species with 50 samples each as well as some properties about each flower. One flower species is linearly separable from the other two, but the other two are not linearly separable from each other. 

To assess the models we will use the confusion matrix with the accuracy metric. 

## KNN

**KNN** tries to predict the correct class for the test data by calculating the **distance between the test data and all the training points**. Then **select the K** nearest points **to the test data**. The KNN algorithm calculates the probability of the test data belonging to the classes of ‘K’ training data and class holds the highest probability will be selected.  

## Random Forest

**Random forest classifier** creates a **set of decision trees** from randomly selected subset of training set. It then aggregates the votes from different decision trees to decide the final class of the test object. Now lets see what is a decision tree.

### Decision Tree

His idea was to **represent data as a tree** where each internal node denotes a test on an attribute (basically a condition), **each branch represents an outcome** of the test, and each leaf node (terminal node) holds a class label.

## Linear Regression

When we want to **predict** a continuous dependent variable from a number of independent variables, we used **regression**. But when it comes to **classification, it isn't the best idea**; because the predicted values are continuous and the classification values are discrete or cualitives. So we can’t get an exact class to accomplish the classification, but we can modify some things to make the regression do classification tasks, although as I said, it is not the best or the most optimal idea.

## Support Vector Classifier

The objective of the **support vector** machine algorithm is to **find a hyperplane** in an N-dimensional space (N — the number of features) that **distinctly classifies the data points**. To separate the two classes of data points, there are many possible hyperplanes that could be chosen. Our objective is to find a plane that has the maximum margin, i.e the maximum distance between data points of both classes. Maximizing the margin distance provides some reinforcement so that future data points can be classified with more confidence.

**Data points falling on either side of the hyperplane can be attributed to different classes**. Also, the dimension of the hyperplane depends upon the number of features. If the number of input features is 2, then the hyperplane is just a line. If the number of input features is 3, then the hyperplane becomes a two-dimensional plane. It becomes difficult to imagine when the number of features exceeds 3.