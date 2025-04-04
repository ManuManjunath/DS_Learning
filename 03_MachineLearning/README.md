# Machine Learning

### Supervised ML
Uses labeled datasets to train algorithms to cassify or predict outcomes.

### Unsupervised ML
Uses algorithms to analyze and cluster unlabeled datasets. 

### Feature Engineering
The process of using practical, statistical, and data science knowledge to select, transform, or extract characteristics, properties, and attributes from raw data.

### Naive Bayes
A Supervised Classification technique that is based on Bayes' Theorem with an assumption of independence among predictors.  
It gives a method of calculating the posterior probability, which is the likelyhood of an event occurring after taking into consideration new information.

### K-Means
Unsupervised Partition algorithm used to organize unlabelled data into groups or clusters.

##### Centroid
The center of a cluster determined by the mathematical mean of all the points in that cluster.

##### Steps
* Initiate K centroids - Or define the number of clusters.
* Assign all points to its nearest centroid.
* Recaculate the centroid of each cluster based on the points assigned.
* Repeat Step #2 and #3 until the data converges.

##### K-means++
It is important to run K-means test multiple times with different initialization of centroids. In scikit-learn, this implementation is called K-means++, which is the default implementation when we initiate K-means.

##### Intra cluster points
Points within a cluster

##### Inter cluster distance
Distance between the clusters

##### Inertia of K-means
Sum of the squared distances between each observation and its nearest centroid.  
Its a measure of intra cluster distance.  
If more compact the clusters, the lower the inertia, since there is less distance between each observation and its nearest centroid.  
Hence it is important for Inertia to be as close to 0 as possible.

##### Silhoutte Score
Mean of the silhoutte co-efficients of all observations in the model.  
Each observation has its own Silhoutte co-efficient.  
$S = (b-a) / max(a,b)$
* a is the mean distance from that observation to all other observations in the same cluster.
* b is the mean distance from that observation to each observation in the next clisest cluster.

A Silhoutte co-efficient can be between -1 and 1. 
* 1 means its within its own cluster and well separated from other clusters.
* 0 means the observation is on the boundary between two clusters.
* -1 means the observation may be in the wrong cluster.


### Tree based learning
A type of supervised machine learning that performs classification and regression tasks.  
 
Nodes are where the decisions are made. They're connected by edges.  
At each node, a single feature of data is considered and decided on.  
Edges direct from one node to the next during this process. Eventually, all relevant features will have been resolved, resulting in the classification prediction.

##### Decision Tree
Flow-chart-like supervised classification model, and a representative of various solutions that are available to solve a given problem, based on the possible outcomes of related choices.
* Requires no assumptions regareing distribution of data.
* Handles collinearity very easily.
Often does not require data pre-processing.

##### Root Node
The first node of the tree, where the first decision is made.

##### Decision Node
Nodes of the tree where decisions are made.  
They always point to a leaf node or other decision nodes within the tree.

##### Leaf Node
The nodes where a final prediction is made.

### Hyperparameter Tuning
Hyperparameters are parameters that can be set before the model is trained.

##### Hyperparameters for Decision Tree
* Max Depth: Defines how "long" a decision tree can get (The depth between root node and leaf nodes)
* Min Samples Leaf: Defines the minimum number of samples for a leaf node.

#### Grid Search
A tool to confirm that a model achieves its intended purpose by systematically checking every combination of hyperparameters to identify which set produces the best results based on the selected metric.

##### Model Validation
The set of processes and activities intended to verify that models are performing as expected.

##### Cross Validation
A process that uses different portions of the data to test and train a model on different iterations.

#### Ensemble learning
Building multiple models and aggregating their outputs to make a prediction.

* Each individual model that compreises an Ensemble is a "base leaner"

##### Bagging (Bootstrap + Aggregating)
* Bootstrapping means Sampling with Replacement.
* During aggregation, the predictions of all the individual models are aggregated to produce the final prediction.

#### Random Forest
Ensemble of decision trees trained on bootstrapped data with randomly selected features.

##### Hyperparameters for Random Forest
* max_features: Sepcifies the number of features that each tree randomly selects during training.
* n_estimators: Specifies the number of trees your model will build in its ensemble.

### Boosting
A technique that builds an ensemble of weak learners sequentialy, with each consequitive learner trying to correct the errors of the one that preceeded it.

#### How is boosting different from Random Forest and Bagging?
* Learners are build sequentially, not in parallel.
* Not limited to tree-based models.

### Adaptive Boosting (AdaBoost)
A boosting methodology  where each consecuitive base learner assigns greater weight to the observations incorrectly predicted by the preceeding learner.

### Gradient Boosting
A boosting methodology where each base learner in the sequence is built to predict the residual errors of the model that preceeds it.

> **GBMs or Gradient Boosting Machines**
Model ensembles that use gradient bossting.

#### Advantages of GBMs
* High accuracy
* Generally scalable
* Work well with missing data
* Don't require scaling (can handle outliers)

#### Disadvantages of GBMs
* Tuning many hyperparameters can be time consuming
* Difficult to interpret
* They're also called **Black Box Models** , which means its predictions cannot be precisely explained.
* Can have difficulty with **extrapolation**, which is a model's ability to predict new values that fall outside the range of values in the training data.
* Prone to overfitting if too many hyperparameters are tuned.

#### XGBoost (Extreme Gradient Bossting)

#### learning_rate (shrinkage)
A hyperpatameter that determines how much weight is given to each consecutive tree's prediction in the final ensemble.

#### min_child_weight
A tree will not split a node if it results in any child node with less weight than this value.