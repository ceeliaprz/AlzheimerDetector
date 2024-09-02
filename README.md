# AlzheimerDetector
The densenet 121 network is used to detect Alzheimer's brains. 

In the first training the finetuning method is used, for this, we load the convolutional network denseset 121 which is previously trained. We modify the last linear layer of the model to add ours with the 4 outputs we need according to the classes of our dataset. In addition, we set the rest of the parameters of the network to false so that they are not adjusted, making use of the characteristics that the learned network already has.

In the second training, we modify all the parameters to true, so that now all of them will be set, achieving an improvement in the generalisation of the network.
