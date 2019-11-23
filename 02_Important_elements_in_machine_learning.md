1. Important Elements in Machine Learning

* Data Format
	* Parametric learning: Regressor or classifier depend on an internal parameter vector that determine the actual instance of a generic predictor.
	* Non-parametric learning: No initial assumptions about the family of predictors
	
* Multiclass strategies
	* One-vs-all: If there are n output classes, n classifiers will be trained in parallel considering there is always a separation between an actual class and the remaining ones.
	* One-vs-one: training a model for each pair of classes; the right class is determined by a majority vote.

* Underfitting and overfitting
	* Representational capacity: ability to learn a small/large number of possible distributions over the dataset.
	* Increasing the (representational) capacity is normally an irreversible operation.
	* Underfitting: It means that the model isn't able to capture the dynamics shown by the same training set (probably because its capacity is too limited). *high bias*
	* Overfitting: The model has an excess capacity and it's not longer  able to generalize effectively, considering the original dynamics provided by the training set. *high variance*

