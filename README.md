Decision Tree Classifier from Scratch

This project focuses on building a Decision Tree classifier from scratch using only pure Python and NumPy, without relying on ready-made machine learning libraries such as scikit-learn. The project is centered on diabetes prediction and covers handling continuous features as well as advanced pruning techniques.

Project Features

Key technical aspects that distinguish this project:
	•	Custom Implementation:
The core logic of fit, predict, and split is fully implemented manually based on mathematical foundations such as Entropy and Information Gain.
	•	Dynamic Thresholding (MSSD):
The Mean Squared Successive Difference (MSSD) method is used to determine the optimal split threshold for continuous features.
	•	Pruning Strategies:
	•	Pre-Pruning: Constraints on tree depth and minimum sample size are applied during tree construction.
	•	Post-Pruning: After the tree is fully grown, branches that do not improve performance on a validation set are removed.

Dataset and Preprocessing

Dataset Used: diabetes_dataset.csv
	•	Class Imbalance Handling:
Downsampling is applied to balance the Diabetes and No Diabetes classes.
	•	Encoding:
Categorical features are converted into numerical values using LabelEncoder.

Algorithm Architecture

The model operates through the following steps:
	1.	Entropy Calculation: Measures the uncertainty in the dataset.
	2.	Information Gain: Determines which feature provides the best split.
	3.	Tree Construction (Recursive): The feature with the highest information gain is selected as the root node, and branching continues until leaf nodes are reached.
	4.	Pruning: The tree is simplified to prevent overfitting.
