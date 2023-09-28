# Anomaly detection in network traffic: Machine learning on NSL KDD

This notebook showcases my work with 3 machine learning algorithms on the NSL kdd Dataset.
The dataset can be found here: https://www.unb.ca/cic/datasets/nsl.html

The dataset has a separate train and test dataset, which makes the algorithm perform worse on the test dataset than on the train. Going from a ~99% accuracy to a 60-90% on the test set can be seen as bad, but I still consider my results as publishworthy. A reason for this is that the test set contains many new attack types, not seen in the train dataset.

There have been many published papers on the NSL-KDD dataset. There is a split between papers using a part of the train set as the test set, and using the test set as the test set. One could argue that using an unseen part of the train set as the test set would be considered fair for testing the performance of the model, but I would argue that this only creates a fake feeling of trust in the model. In the cyber security space, everything is a threat. Constantly there are new malicious attacks, hence the need for a model that could predict new types of attacks based on old attacks. 

This file contains three types of machine learning algorithms. Support vector machines, Decision trees, and Random Forests. Although the DT and RF models are quite similar, they are still super strong algorithms and have their strengths and weaknesses. For further work on this data set, I would consider building a deep learning model, preferably a convolutional neural network, and considering each line in the dataset as a one-dimensional image, as this as been shown promising results on similar datasets. 
