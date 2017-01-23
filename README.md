# Behavioral Cloning for Automated Driving Using Deep Convolutional Neural Networks

This repository provides the source codes for a Keras implementation of a deep convolutional neural network (CNN) that can autonomously drive a car in a simulated environment by learning from a set of demonestrations provided by a human driver.


#### Autonomous Driving Using the Pretrained Network:

#### Training the Network:

* **Data:** The training data collected from driving the car in the simulator can be found in `./data` directory. (acknowledgment: `./data/data_4` is a subset of this [dataset](https://github.com/matthewzimmer/CarND-BehavioralCloning-P3)).


# Method:
#### Model Architecture:
A deep neural network consists of xxx 2D convolutional layers followed by xxx fully connected layers is implemented in `shahnet(image_shape)` function in `model.py`. In order to prevent overfitting each fully connected layers are stacked with a Dropout layer that randomly sets 50% of the input stimula to zero (only) during training. Moreover, MaxPooling layers are placed after the Conv layers to downsample the images over the pipe, decrease the number of trainable parameters and as a result overfitting prevention. After some manual iterations, it turned out that 2x2 max-pooling yields to the best performance along with the othery layers.

#### Data Augmentation and Preprocessing:
crop
resize


#### Prerequisites:
* Python Packages: Keras, TensorFlow, OpenCV, flask, eventlet, python-socketio
* Simulator: Udacity has recently created a car simulator that is used here. I have used the linux version on my Ubuntu machine. Running the simulator is very straight forward and the demonestrations can be recorded for training our CNN. 





