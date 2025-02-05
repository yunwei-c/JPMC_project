The readme for JPMC project.
------

The exploratory data analysis is performed in the Take_home_EDA.ipynb file.
This code first loads the data from the CSV file. To gain a preliminary understanding, it prints the data types and ignores non-numerical values for later modeling.
Some data preprocessing steps are performed, such as removing duplicate values and dropping null values.
To understand the distribution of the data, a box plot is used.
------

The neural network implementation can be found in the Take_home_Train_Test_NN.ipynb file.
The code first performs the preprocessing steps introduced in the Take_home_EDA.ipynb file.
It splits the dataset into a 4:1 ratio for training and validation, converts the values into Torch tensors, and uses a dataloader to handle the data efficiently.
The model is a neural network with 16 hidden units. To predict the final binary bad_flag label, binary cross-entropy loss is used. The optimizer chosen is Adam with a learning rate of 0.001.
The training loop consists of loading the training data in batches, making predictions, and optimizing using binary cross-entropy loss.
After 50 epochs, the final model achieves 93.6% accuracy on the test set.
