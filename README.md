# machine learning on the NSL-KDD dataset

This notebook showcases my work with 3 machine learning algorithms on the NSL kdd Dataset.
The dataset can be found here: https://www.unb.ca/cic/datasets/nsl.html

The dataset has a separated train and test dataset, which makes the algorithm perform much worses on the test dataset than on the train. Going from a ~99% accuracy to a 60-90% on the test set can be seen as badly, but I still consider my results as publishworthy. A reason for this is because the test set contains many new attack types, not seen in the train dataset.

There has been many published papers on the NSL-KDD dataset. There is a split between papers using a part of the train set as the test set, and using the test set as the test set. One could argue that using an unseen part of the train set as the test set would be considered fair for testing the performance of the model, but I would argue that this only creates a fake feeling of trust to the model. In the cyber security space everything is a threat. Constantly there is new malicious attacks, hence the need for a model that could predict new types of attacks based off old attacks. 

This file contains three types of machine learning algorithms. Support vector machines, Decision trees and Random Forests. Although the DT and RF models are wuite similar, they are still super strong algorithms and have their strength and weaknesses. For further works on this data set I would consider building a deep learning model, prefferebly a convolutional neural network, and cosider each line in the dataset as a one dimensional image, as this as been shown promising results on similar datasets. 
