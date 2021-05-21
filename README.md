# EVA6_Session4_Assigment

**<b fontsize="30">Session 4 - PyTorch
Goal
Write a neural network that has</b >
**


<b>2 inputs:</b>

an image from MNIST dataset, and

a random number between 0 and 9


<b>2 outputs:</b>

the "number" that was represented by the MNIST image, and

the "sum" of this number with the random number that was generated and sent as the input to the network**

<b>Approach Outline</b>

Created EnhancedMNIST Dataset to add the label for the random number and the sum


Neural Network Architecture

Conv layers, RELu Activation and  log_softmax for MNIST classification

One-Hot-Vector output (OHV) of MNIST is concatenated with OHV of random number input

Concatenated vector is put through <b>two</b> fully-connected layers + log_softmax to get sum prediction (OHV)
Outputs MNIST OHV and sum prediction OHV


Results
> 98% test accuracy for both tasks within 5 epochs




Snagit of the Output
--EPOCH 1:
Loss:     	 MNIST: 0.2497 	 SUM: 0.1919 	 TOTAL: 0.4416
Accuracy: 	 MNIST: %92.15 	 SUM: %19.19 	 TOTAL: %55.67
HBox(children=(FloatProgress(value=0.0, max=469.0), HTML(value='')))
--EPOCH 2:
Loss:     	 MNIST: 0.0961 	 SUM: 0.6317 	 TOTAL: 0.7278
Accuracy: 	 MNIST: %97.9 	 SUM: %63.17 	 TOTAL: %80.53
HBox(children=(FloatProgress(value=0.0, max=469.0), HTML(value='')))
--EPOCH 3:
Loss:     	 MNIST: 0.0778 	 SUM: 0.9133 	 TOTAL: 0.9911
Accuracy: 	 MNIST: %98.43 	 SUM: %91.33 	 TOTAL: %94.88
HBox(children=(FloatProgress(value=0.0, max=469.0), HTML(value='')))
--EPOCH 4:
Loss:     	 MNIST: 0.0539 	 SUM: 0.9863 	 TOTAL: 1.0402
Accuracy: 	 MNIST: %98.82 	 SUM: %98.63 	 TOTAL: %98.72
HBox(children=(FloatProgress(value=0.0, max=469.0), HTML(value='')))
--EPOCH 5:
Loss:     	 MNIST: 0.0533 	 SUM: 0.9927 	 TOTAL: 1.046
Accuracy: 	 MNIST: %98.92 	 SUM: %99.27 	 TOTAL: %99.09
