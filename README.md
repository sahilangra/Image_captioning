Project Overview
In this project, you will create a neural network architecture to automatically generate captions from images.

After using the Microsoft Common Objects in COntext (MS COCO) dataset to train your network, you will test your network on novel images!

Image Captioning Model Image Captioning Model

LSTM Inputs/Outputs
LSTM Decoder
In the project, we pass all our inputs as a sequence to an LSTM. A sequence looks like this: first a feature vector that is extracted from an input image, then a start word, then the next word, the next word, and so on!

Embedding Dimension
The LSTM is defined such that, as it sequentially looks at inputs, it expects that each individual input in a sequence is of a consistent size and so we embed the feature vector and each word so that they are embed_size.

Sequential Inputs
So, an LSTM looks at inputs sequentially. In PyTorch, there are two ways to do this.
