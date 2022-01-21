# deep-learning-challenge
Making a deep learning network to help a charity track funds.

# unsupervised-learning
Using unsupervised machine learning methods to help cluster cryptocurrencies.

## Some thoughts:
- This was an intense assignment bringing together almost a "best of" our unsupervised machine learning methods.
- The overall idea of the assignment was very interesting, with reports on cryptocurrencies being somewhere between "fad" and "the future".

## The work:

### A picture of the initial data provided:
![Initial upload of data](https://github.com/marcuspttr/deep-learning-challenge/blob/main/Assets/intial_load.PNG)


### Preview of data after cleaning & preparing:
![Overview of data](https://github.com/marcuspttr/deep-learning-challenge/blob/main/Assets/data_overview.PNG)

Running the indicated dimensionality reduction to maintain 90% of the explained variance, we limited the data to 12 principal components.
Created a new clean dataframe for reference in the future calculations.

### After one hot encoding:
![One hot dataframe](https://github.com/marcuspttr/deep-learning-challenge/blob/main/Assets/onehot.PNG)

### Creating the layers of my neural network.
![NN model design](https://github.com/marcuspttr/deep-learning-challenge/blob/main/Assets/nn_model_design.PNG)

The graph definitely seems to show some distinct clusters. I have some concerns of how tightly some of the data appears, but I would claim at this point there are around 5 clusters.

![NN model parameters](https://github.com/marcuspttr/deep-learning-challenge/blob/main/Assets/parameters.PNG)

### Elbow graph showing clusters & inertia:
![Model accuracy loss](https://github.com/marcuspttr/deep-learning-challenge/blob/main/Assets/model_accuracy.PNG)

Finding the proper flattening of this curve I'd recommend to my clients that there may be 6 to 7 clusters within the data. Reflecting on the TSNE graph as well, I'd say it's safer to go with the smaller amount of clusters (6) rather than create superfluous groups.
