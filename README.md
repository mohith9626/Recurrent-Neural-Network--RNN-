# Recurrent-Neural-Network--RNN-
action recognition using RNN, (Long-Short Term Memory) LSTM in particular

The given dataset is called UCF101, which consists of 101 different actions/classes and for each action, there will be 145 samples. We tagged each sample into either training
or testing. Each sample is supposed to be a short video, but we sampled 25 frames from each videos to reduce the amount of data. Consequently, a training sample is an image 
tuple that forms a 3D volume with one dimension encoding temporal correlation between frames and a label indicating what action it is.

To tackle this problem, we aim to build a neural network that can not only capture spatial information of each frame but also temporal information between frames. 
Fortunately, we don't have to do this on our own. RNN — a type of neural network designed to deal with time-series data — is right here for us to use. In particular, 
we will be using LSTM for this task.

Instead of training an end-to-end neural network from scratch whose computation is prohibitively expensive, we divide this into two steps: feature extraction and modelling.
