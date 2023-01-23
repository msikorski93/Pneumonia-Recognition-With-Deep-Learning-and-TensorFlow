# Pneumonia-Recognition-With-Deep-Learning-and-TensorFlow
In this project a convolutional neural network (CNN) was built and trained in Keras with TensorFlow as backend from scratch to predict
if patients were infected with pneumonia using their chest radiology images. The dataset contained the lungs X-ray images of both groups: normal
and pneumonia infected patients. The model used was sequential with a combination of convolutional layers, pooling layers, dropout layers, dense layers
with ReLu activation and output layer with sigmoid activation. The CNN was designed with the following architecture:

![architecture](https://user-images.githubusercontent.com/45270023/214060460-810941ae-b8e6-43c9-9a9e-695520737e33.jpg)

The learning process stopped at the 33rd epoch. The model evualation on test data achieved 86.06% for accuracy and 93.34% for the AUC score. Finally, we
made a single image recognition on an online chest image. The algorithm performs correctly in terms of classifying patients radiology images.
