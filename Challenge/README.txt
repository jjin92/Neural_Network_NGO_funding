Q1: How many neurons and layers did you select for your neural network model? Why?

A1: I chose 8 neurons for the first hidden layer, and 4 neurons for the second hidden layer. 
The number of input feature layer is 39, so I chose to gradually reduce the number of neurons.

Q2: Were you able to achieve the target model performance? What steps did you take to try and increase model performance?

A2: No. The accuracy of testing data stuck around 72%. 
*The origin model:* 
- 1st layer: 8 neuron, relu
- 2nd layer: 4 neuron, relu
- epochs: 50
- Accuracy: 0.7277

I had several attemps to optimize the model.
*Attempt 1: increase neurons*
- 1st layer: 12 neuron, relu
- 2nd layer: 5 neuron, relu
- epochs: 50
- Accuracy: 0.7262

*Attempt 2: increase hidden layers*
- 1st layer: 16 neuron, relu
- 2nd layer: 8 neuron, relu
- 3rd layer: 4 neuron, relu
- epochs: 50
- Accuracy: 0.7262

*Attempt 3: change activation function*
- 1st layer: 12 neuron, sigmoid
- 2nd layer: 5 neuron, sigmoid
- epochs: 50
- Accuracy: 0.7247

*Attempt 4: add more epochs*
- 1st layer: 12 neuron, relu
- 2nd layer: 5 neuron, relu
- epochs: 100
- Accuracy: 0.7233

The might be overfitting the training data as I increase parameters. 

Q3: If you were to implement a different model to solve this classification problem, which would you choose? Why?

A3: I will try SVM to solve the overfitting issue from the deep learning model. I may also try the Random Forest model as it is good in classifying data in tabular format.