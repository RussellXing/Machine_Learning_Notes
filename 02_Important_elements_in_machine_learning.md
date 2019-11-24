1. Data Format
	* Parametric learning: Regressor or classifier depend on an internal parameter vector that determine the actual instance of a generic predictor.
	* Non-parametric learning: No initial assumptions about the family of predictors
	
2. Multiclass strategies
	* One-vs-all: If there are n output classes, n classifiers will be trained in parallel considering there is always a separation between an actual class and the remaining ones.
	* One-vs-one: training a model for each pair of classes; the right class is determined by a majority vote.

3. Underfitting and overfitting
	* Representational capacity: ability to learn a small/large number of possible distributions over the dataset.
	* Increasing the (representational) capacity is normally an irreversible operation.
	* Underfitting: It means that the model isn't able to capture the dynamics shown by the same training set (probably because its capacity is too limited). *high bias*
	* Overfitting: The model has an excess capacity and it's not longer  able to generalize effectively, considering the original dynamics provided by the training set. *high variance*

4. Error measures and cost functions
	* Mean Square Error(MSE): 
	![MSE](https://github.com/RussellXing/Machine_Learning_Notes/blob/master/graphs/MSE.jpg)
	
5. Loss function or Cost Function: to find the global minimum or a point quite close to it
	* zero-one-loss
	![Zero_one_loss](https://github.com/RussellXing/Machine_Learning_Notes/blob/master/graphs/Zero_one_loss.jpg)

6. MAP learning
	![MAP](https://github.com/RussellXing/Machine_Learning_Notes/blob/master/graphs/MAP.jpg)

7. Maximum likelihood learning
	![ML](https://github.com/RussellXing/Machine_Learning_Notes/blob/master/graphs/Maximun_likelihood.jpg)

8. Class Balancing
	1. Resampling with replacement
		* After every sampling step, restart from the procedure.
		```
		import numpy as np
		from sklearn.utils import resample
		X_1_resampled = resample(X[Y==1], n_samples=X[Y==0].shape[0], random_state=1000)
		Xu = np.concatenate((X[Y==0], X_1_resampled))
		Yu = np.concatenate((Y[Y==0], np.ones(shape=(X[Y==0].shape[0], ), dtype=np.int32)))
		```

	2. SMOTE resampling
		* SMOTE: Synthetic Minority Over-sampling Technique
		* To consider the relationships that exist between samples and create new synthetic points along the segments connecting a group of neighbors.
		* The new dataset has a higher variance, and a generic classifier can better find a suitable separation hypersurface.
		```
		from imblearn.over_sampling import SMOTE
		smote = SMOTE(random_state=1000)
		X_resampled, Y_resampled = smote.fit_sample(X, Y)
		```
		* Parameters
			* ratio: It determines which class must be resampled (acceptable values are 'minority', 'majority', 'all', and 'not minority').
			* k_neighbors: The number of neighbors to consider. Larger values yield more dense resamplings,

9. Elenments of information theory
	* Entropy：proportional to the uncertainty of X and is measured in bits
		![Entropy](https://github.com/RussellXing/Machine_Learning_Notes/blob/master/graphs/entropy.jpg)
	* High entropy contains more information. *proportion to the variance*
	* Perplexity is very useful for assessing the amount of uncertainty in a distribution
		![Perplexity](https://github.com/RussellXing/Machine_Learning_Notes/blob/master/graphs/Perplxity.jpg)
	

