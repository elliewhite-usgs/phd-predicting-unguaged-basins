After a statistical learning method is applied, the model needs to be tested. Most statistical learning techniques used in water resources modeling employ a randomized splitting of data into k-folds to estimate model error. In each iteration, one fold is held out as a test set and others are designated as a training set. 

Such random cross-validation methods ignore structures in the data, which underestimate model error (Roberts et al., 2017). A more accurate estimate of the model error can come from techniques that block training sets in time, space, or unique structure (e.g., by hydrologic basins). 

The difficulty here lies in specifying block sizes (in time and space). Blocking potentially reduces the range of parameters seen by the model, and may exclude a particular meaningful combination of predictor variables in the training data set. Too small of a block size and the cross-validation method more closely mimics the randomized method and runs the risk of under estimating model error. Large block sizes force too much model extrapolation, and risk over estimating model errors. 

This research proposes to compare multiple cross-validation and bootstrapping strategies to assess the sensitivity of the estimated uncertainty to such resampling methods.