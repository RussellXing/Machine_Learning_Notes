# Introduction

1. Classic and adaptive machines
	* Classic system: *input values, process and produce outputs results*
	* Adaptive system: *continuous abilit to adapt behavior to external signals*
		* Transformed our electronic tools into actual cognitive extensions
		* Achieved this goal by filling the gap between human perception, language, reasoning, and model and artificial instruments.

2. Descriptive analysis
	* The goal of **descriptive analysis** is to find out an accurate description of the phenomena that are observed and validate all the hypothesis.
	* A **diagnostic model** must be able to connect all the effecs with causes.
	
3. Predictive analysis
	* The goal of a **predictive model** is to minimize the error between actual and 	predictive value.
	* The prediction must be turned into a suggested prescription.
   
4. Supervised learning
	* A **supervised scenario** is characterized by the concept of a teacher or supervisor, whose main task is to provide the agent with a precise measure of its error (directly comparable with output values).
	* **Overfitting** causes overlearning due to an excessive capacity.
	* **Regeression**: based on continuous output values
	* **Classification**: only a dicrete number of possible outcomes
	* Common supervised learning applications:
		* Predictive analysis based on regression or categorical classification
		* Spam detection
		* Pattern detection
		* NLP Sentiment analysis 
		* Automatic image classification 
		* Automatic sequence processing

5. Unsupervised learning
	* To learn how a set of elements can be grouped (clustered)
		* In a **recommendation engine**, a group of users can be clustered according to the prederence expressed for some books.
	* Common unsupervised applications:
		* Object segmentation
		* Similarity detection
		* Automation labeling
		* Recommendation engines
		
6. Semi-supervised learning
	* A direct supervised approach is infeasible because the data used to train the model couldn't be representative of the whole distribution.
	* The reader who is interested can check out _Mastering Machine Learning Algorithms, Bonaccorso G., Packt Publishing_.
	* The main goals that a semi-supervised learning approach pursue:
		* The propagation of labels to unlabeled samples considering the graph of the whole dataset.
		* Performing a classificaion training model(**Support Vector Machines**)
		* Non-linear dimensionality reduction considering the graph structure of the dataset.
		
7. Reinforcement learning
	* The feedback is usually called **reward/penalty**, and it's usefull to understand whether a certain action performed in a state is positive or not.
	* An action can also be imperfect, but in terms of a global policy, it has to offer the highest total reward.
	* It's often very dynamic, and when it's impossible to have a precise error measure.
	* Comman examples:
		* Automatic robot control
		* Game solving
		* Stock traded analysis based on feedback signals

8. Deep learning and bio-inspired adaptive systems
	* The idea behind these techniques is to create algorithms that work like a brain, and many important advancements in this field have been achieved thanks to the contribution of neurosciences and cognitive psychology.
	* Of course, testing different architectures and optimization algorithms is rather simpler (and it can be done with parallel processing) than defining a complex model (which is also more difficult to adapt to different contexts).
	* Common deep learning applications include the following: 
		* Image classification
		* Real-time visual tracking
		* Autonomous car driving
		* Robot control
		* Logistic optimization
		* Bioinformatics
		* Speech recognition and Natural Language Understanding (NLU)
		* Natural Language Generation (NLG) and speech synthesis

9. Machine learning and big data
	* Always perform a descriptive/prescriptive analysis of the problem and the data, trying to focus on the following: 
		* The current situation Objectives (what do we need to achieve?)
		* Data and dimensionality (do we work with batch data? Do we have incoming streams?) 
		* Acceptable delays (do we need real-time? Is it possible to process once a day/week?) 
	* Big data solutions are justified, for example, when the following is the case: 
		* The dataset cannot fit in the memory of a high-end machine
		* The incoming data flow is huge, continuous, and needs prompt computations (for example, clickstreams, web analytics, message dispatching, and so on)
		* It's not possible to split the data into small chunks because the acceptable delays are minimal (this piece of information must be mathematically quantified)
		T* he operations can be parallelized efficiently (nowadays, many important algorithms have been implemented in distributed frameworks, but there are still tasks that cannot be processed by using parallel architectures)

