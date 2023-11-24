# p-deep-learning-classifiers-for-urban-sound-data


## MIlestones:

#### Verificar extração de features e fazer analise exploratoria com graficos e merdinhas

```
In this step, you will need to form the input of your neural networks, by processing original raw sound data.
Take into account that raw sound files will possibly have different durations and different sampling rates.
You will then need to uniformize and normalize the network input and decide if you want to give as input
of the network the raw data or some features extracted from it. You can use functions from libraries (e.g.,
librosa) to perform signal processing and feature extraction.
The class labels that will be used to train the models and evaluate their performance can be obtained from the
file UrbanSound8K.csv provided with the dataset.

```

#### Com as features finalizadas definir a arquitetura dos modelos e escolher os 2 modelos a fazer

```
In the case of the MLP, this steps consists in the definition of the number of layers, number of neurons for
each layer, and in the choice of the activation functions to adopt at each layer.
In the case of CNNs, a first design choice is related to using 1-dimensional or 2-dimensional inputs. 1D
inputs can be obtained by applying the CNN directly on portions (windows) of the original sound signal
(after downsampling and normalization). 2D representations of sounds, on the other hand, are based on timefrequency
analysis of sounds, as the Mel-frequency cepstral coefficients (MFCCs) described in http://
www.justinsalamon.com/uploads/4/3/9/4/4394963/salamon_urbansound_acmmm14.
pdf. After defining if you are using a 1D or 2D CNN, model definition involves the definition of the model
architecture to adopt (number layers, kinds of layers, filter dimensions, number of feature maps, etc.)
In the case of RNN, the design of the model architecture encompasses the kind of units used in the neural
network and kind of connections (unidirectional vs. bidirectional). Possible choice in this sense are vanilla
RNNs, gated recurrent units (GRUs), long-short term memory (LSTM) networks, etc.
3.3 Training strategy
In this part, you will need to define the details for the training strategies adopted to train the models. These
details include:
• Optimizer
2
• Learning hyperparameters (e.g., learning rate, mini-batch size, number of epochs, etc.)
• Regularization techniques to adopt (e.g., early stopping, weight regularization, dropout, data augmentation,
etc.)
• Possibility of using transfer learning

```

#### Fazer a validação como o professor disse no project:

```
The performance of the considered classifiers will be evaluated using the urbansound8k dataset taking care
of appropriately separating train, validation, and test data. In order to do that, you will need to use the 10-fold
cross-validation scheme described at https://urbansounddataset.weebly.com/urbansound8k.
html
Then, classification performance will be quantified using a confusion matrix and reporting the average classification
accuracy and its standard deviation over the 10 experiments included in the 10-fold cross-validation
scheme.

```


### If tempo: bonus