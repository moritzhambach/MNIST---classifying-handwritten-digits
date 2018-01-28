## MNIST

 The MNIST dataset of handwritten digits is the one of the standard benchmarks of machine learning classification. The current published record on MNIST is 99.79% (<http://rodrigob.github.io/are_we_there_yet/build/classification_datasets_results.html#4d4e495354>). This repo shows two approaches:

### 1) A neural network from scratch (98.3% accuracy on MNIST):
- build a neural network with just the numpy package
- uses mini batch-gradient descent with regularisation and momentum, flexible geometry and various activation functions
- fully vectorised and less than twice as slow as the same Keras model (see benchmark in notebook)
        

### 2) Convolutional Neural Network with Keras (99.68% accuracy on MNIST)
- VGG geometry (3x3 filters, 2x2 max pooling) with batch normalisation
- uses Adam optimisation
- increases batch size instead of reducing learning rate
