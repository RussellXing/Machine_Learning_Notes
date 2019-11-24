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
	
	
5. Loss function or Cost Function: to find the global minimum or a point quite close to it
	* zero-one-loss

6. MAP learning


7. Maximum likelihood learning


8. Class Balancing
    1. Resampling with replacement
    	* After every sampling step, restart from the procedure.
