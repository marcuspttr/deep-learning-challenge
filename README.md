# deep-learning-challenge
Making a deep learning network to help a charity track funds.

## Some thoughts:
- I struggled and had to do some extra research when creating the layers and number of neurons for my neural network.
- I also had to look into creating callback steps to the fitting process.
- It was a interesting homework, try as I might, I could not improve the accuracy of my model. It hovered around 72 to 74% accuracy pretty consistently.

## The work:

### A picture of the initial data provided:
![Initial upload of data](https://github.com/marcuspttr/deep-learning-challenge/blob/main/Assets/intial_load.PNG)
The intial data set up looks at the funding dispressed by a charity. It contains a lot of information such as the name of the organization the funding was provided to,
the type of application, what the use case was, and of course money amounts and whether or not the funding was successful. 

I initially dropped the EIN and Name as they were not important factors beyond identification and tracking.

### Preview of data after cleaning & preparing:
![Overview of data](https://github.com/marcuspttr/deep-learning-challenge/blob/main/Assets/data_overview.PNG)
Here is a preview of the data at that point and how many different values were contained in each remaining column.

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
