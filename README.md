# Classification-problem-using-the-Clean-California-Housing-Prices-dataset
The problem consists of estimating the approximate location of housing blocks. The approximate location is called ocean_proximity which may have one of four possible values: NEAR BAY, 1H OCEAN, INLAND, and NEAR OCEAN.
    
The features variables are prepocessed and normalised in range between [-1,1]. The target variable is oneHote encoded and the all dataset is shuffled and divided in three set: trainset, validset and testset. 

The architecture of the deep artificial neural network and some hyperparameters are tuned using Hyperas. Hyperas is a convenient when try to hypertune Keras models. it's a wrapper of the famous optimisation package hyperopt.



Please Note to ensure compatibility of hyperas with hyperopt==0.2.7, modify the line 139 in optim.py in hyperas, from rstate=np.random.RandomState(rseed)
to 
rstate=np.random.default_rng(rseed).
