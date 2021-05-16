# Exploratory analysis
##### Source: https://towardsdatascience.com/https-medium-com-skuttruf-machine-learning-in-finance-algorithmic-trading-on-energy-markets-cb68f7471475
Split your data into complementary sets for training, validation (for parameter tuning, feature selection etc) and testing. This is actually more complex than it sounds: optimally, the test set should be as ‘similar’ as possible to the present ‘state of the market’, and both validation and test set should follow the same distribution. Otherwise you might waste effort tuning the model parameters on the validation set only to find that it poorly generalizes to the test set.

Following the concept of ‘market regimes’?—?ie extended periods where a specific combination of commodities dominates the price dynamics of your target instrument?—?it might be worthwhile to first have a clustering algorithm of unsupervised learning discover defining correlations in the data and then evaluate model performance on data in the validation and test set belonging to the same clusters (see Figure 3?—?in this project, clustering increased predictive performance by 8%).

Data Transformations:
Moving averages can provide historical context and trends when your choice of learning algorithm does not have explicit memory cells like Recurrent Neural Networks or LSTMs.
Using data or derived inputs such as indicators/indices which may be less accurate than the data you have may have some use specially if other participants can influence the output you are trying to model in which case they indicators/indices can provide inputs about how other participants will behave.

Model Validation:
Genetic algorithms allow you to explore the policy space, starting from a first generation of say 100 randomly chosen policy parameters, iteratively eliminating the 80 worst performers and making the 20 survivors produce 4 offspring each. Or you can employ a grid search in the multidimensional parameter space: starting from some plausible values for the parameters of the policy, what is the best-performing setting you can achieve by varying the parameter values one-by-one.

A good measure to prevent overfitting the parameters to the validation set is a cross-validation with a ‘walk-forward-test’ (WTF) verifying the robustness of your approach: optimize the policy parameters on a validation segment, test them forward in time on data following the validation segment, shift the validation segment forward to include that test data, repeat. The basic assumption here is that the recent past is a better gauge for the future than the more distant past.

Optimisation:
Exploring the space of policy parameters in this framework is done via inefficient numerical optimisation, not with the powerful gradient optimization of your predictive Machine Learning model.
