Download link :https://programming.engineering/product/cse4152-hw6-imitation-learning/

# CSE4152-HW6-Imitation-Learning
CSE4152 HW6 Imitation Learning
How to install GYM and pytorch

Experiment overview

Goal: implement reinforcement learning framework that trains a driving agent.

Simulator: OpenAI GYM


https://www.gymlibrary.ml/

We will use Box2D-CarRacing

Please install gymSG

CarRacing information

Action: steering, acceleration, brake

Sensor input: 96x96x3 screen

It shows car’s states and path information.

Skeletons

Four tasks

A. Implement loading demonstrations

Given the folder of the imitations, it should load all observation and action files into two separate lists observations and actions which are returned. Implement the function load_demonstrations in demonstrations.py

B. Understand training

The module training.py contains the training loop for the network. Read and understand its function train. Why is it necessary to divide the data into batches? What is an epoch? What do lines 69 to

77 do? Please write on report precisely.

C. Conversion from action to classes and selection of action from scores

Define the set of action-classes you want to use and complete the class-methods

actions_to_classes and scores_to_action in network.py The former maps every

action to its class representation using a one-hot encoding and the latter retrieves an action from the scores predicted by the network.

Network Implementation

Design and implement an simple network architecture in network.py.

Convolution layers on the images, followed by 2 or 3 fully connected layers to extract a 1D feature vector. Let each layer be followed by a ReLU asCSE4152thenon-linear activation.

Pipeline overview


Demonstrations

➢python main.py –teach

s – store the current demonstration. They are stored in “data/teacher”

C. action to class


C. action to class

C. score to action

Network Design

Network overview

Scores Action Label


Network Specification Reference

Agent network

HW6 -submission

Deadline:  (SUN) on Cyber campus

Submission:

Python code: your implementation

Report: write answer of “task B. Understand training” on report precisely

Agent file: When training runs successfully, the model agent is automatically saved

Zip file: include three files above

File format:

Python MLP code: demonstration.py, network.py

Report: CSE4152_학번_HW06.txt

Agent file: agent.pt

Zip file: CSE4152_학번_hw6.zip

If you have any questions, feel free to ask in the cyber campus Q&A or send them to the TA’s email(kangpiljae@gmail.com)

 Tips
