# Decision-Tree-Analysis-Titanic-Dataset
 Build and evaluate a decision tree using the Titanic dataset, including tree pruning through cross-validation, accuracy assessment, and comparison with a Random Forest model.

In this programming problem, you will get familiar with building a decision tree, using cross validation to prune a tree, evaluating the tree performance, and interpreting the result.
Potential packages to use and short tutorials:

(1)http://scikit-learn.org/stable/modules/tree.html

(2)http://chrisstrelioff.ws/sandbox/2015/06/25/decision_trees_in_python_again_cross_validation.html


![image](https://github.com/kashyaparun25/Decision-Tree-Analysis-Titanic-Dataset/assets/52271759/3c894a3e-0263-403b-9ec8-541d2b0f1f6c)
![image](https://github.com/kashyaparun25/Decision-Tree-Analysis-Titanic-Dataset/assets/52271759/89339b6c-2881-4079-b2df-6d38c0cb503f)

classification tree
Use the titanic.csv dataset included in the assignment.

Step 1: Read in Titanic.csv and observe a few samples, some features are categorical and others are numerical. Take a random 70% samples for training and the rest 30% for test.

Step 2: Fit a decision tree model using independent variables ‘pclass + sex + age + sibsp’ and dependent variable ‘survived’. Plot the full tree. Make sure ‘survived’ is a qualitative variable taking 1 (yes) or 0 (no) in your code. You may see a tree similar to (not necessarily the exact same as) this one:

![image](https://github.com/kashyaparun25/Decision-Tree-Analysis-Titanic-Dataset/assets/52271759/d34ac1d6-b2f4-42a4-9e92-4f49cad53e13)

Step 3: Use cross‐validation to find the best parameter to prune the tree. You should be able to plot a graph with the ‘tree size’ as the x-axis and ‘number of misclassification’ as the Y-axis. You may have a plot similar to (not necessarily the exact same as) below:
![image](https://github.com/kashyaparun25/Decision-Tree-Analysis-Titanic-Dataset/assets/52271759/9c964b12-d4cf-455a-9681-fc072430dbaf)

Step 4: Find the tree size that yields a minimum number of misclassifications. Choose the optimal tree size to prune the tree and plot the pruned tree (which shall be smaller than the tree you obtained in Step 2). Report the accuracy of pruned tree on the test set for the following:

percent survivors correctly predicted (on test set)

percent fatalities correctly predicted (on test set)

Step 5: Use the RandomForestClassifier() function to train a random forest using the optimal tree size you found in Step 4. You can set n_estimators as 50. Report the accuracy of random forest on the test set for the following:

percent survivors correctly predicted (on test set)

percent fatalities correctly predicted (on test set)

Check whether there is improvement as compared to a single tree obtained in Step 4. If not, please discuss the potential reasons.




