# Recurrent Neural Networks course project: time series prediction and text generation (RNN)
RNN for times series prediction and sequence generation 

### Problem 1: Perform time series prediction¶
In the first problem, the code performs time series prediction using a Recurrent Neural Network regressor. In particular it re-creates the figure where the stock price of Apple is forecasted (or predicted) 7 days in advance. The code constructs RNNs using Keras.
The particular network architecture employed for the RNN is known as Long Term Short Memory (LTSM), which helps significantly avoid technical problems with optimization of RNNs.

### Problem 2: Create a sequence generator
In this project, the code implements a popular Recurrent Neural Network (RNN) architecture to create an English language sequence generator capable of building semi-coherent English sentences from scratch by building them up character-by-character. This requires a substantial amount amount of parameter tuning on a large training corpus (at least 100,000 characters long). In particular for this project we are using a complete version of Sir Arthur Conan Doyle's classic book The Adventures of Sherlock Holmes.
The machine learning model is trained to generate text automatically, character-by-character by showing the model many training examples so it can learn a pattern between input and output. With this type of text generation each input is a string of valid characters like this one
dogs are grea
whlie the corresponding output is the next character in the sentence - which here is 't' (since the complete sentence is 'dogs are great'). Many such examples are shown to the model in order for it to make reasonable predictions.


## Install 
Install tensorflow
`conda install -c conda-forge tensorflow=1.0.0`

If necessary use

```sudo pip install keras```

```KERAS_BACKEND=tensorflow python -c "from keras import backend"```

## Run
open the notebook RNN_project.ipynb in a terminal
```jupyter notebook RNN_project.ipynb```

## Accelerating the Training Process 

If your code is taking too long to run, you will need to either reduce the complexity of your chosen RNN architecture or switch to running your code on a GPU.  If you'd like to use a GPU, you have two options:

#### Build your Own Deep Learning Workstation

If you have access to a GPU, you should follow the Keras instructions for [running Keras on GPU](https://keras.io/getting-started/faq/#how-can-i-run-keras-on-gpu).

#### Amazon Web Services

Instead of a local GPU, you could use Amazon Web Services to launch an EC2 GPU instance. (This costs money.)

**License**

The files are private domain works.
