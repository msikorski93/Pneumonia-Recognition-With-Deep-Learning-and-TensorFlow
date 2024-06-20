# Pneumonia-Recognition-With-Deep-Learning-and-TensorFlow
In this project a convolutional neural network (CNN) was built and trained in Keras with TensorFlow as backend from scratch to predict
if patients were infected with pneumonia using their chest radiology images. The dataset contained the lungs X-ray images of both groups: normal
and pneumonia infected patients. The model used was sequential with a combination of convolutional layers, pooling layers, dropout layers, dense layers
with ReLu activation and output layer with sigmoid activation. The CNN was designed with the following architecture:

![architecture](https://user-images.githubusercontent.com/45270023/214060460-810941ae-b8e6-43c9-9a9e-695520737e33.jpg)

The learning process stopped at the 33rd epoch. The model evaluation on test data achieved 86.06% for accuracy and 93.34% for the AUC score. Finally, we
made a single image recognition on an online chest image. The algorithm performs correctly in terms of classifying patients radiology images.


### New notebook for November 2023
A new classification task was performed using transfer learning. Five different pre-trained models were generated and performed with the following evaluation metrics:
|                | accuracy | recall   | precision | auc      | f1_score | f2_score |
|----------------|----------|----------|-----------|----------|----------|----------|
| ResNet50       | 0.832532 | 0.830128 | 0.834139  | 0.875502 | 0.967742 | 0.949367 |
| VGG16          | 0.883814 | 0.889423 | 0.879556  | 0.938604 | 0.875000 | 0.875000 |
| VGG19          | 0.818109 | 0.823718 | 0.814580  | 0.904382 | 0.848485 | 0.864197 |
| InceptionV3    | 0.828526 | 0.828526 | 0.828526  | 0.853080 | 0.687500 | 0.687500 |
| EfficientNetB1 | 0.783654 | 0.783654 | 0.783654  | 0.882095 | 0.875000 | 0.875000 |

This notebook has been additionally developed with Grad-CAM visualizations for the best CNN - VGG16.

<p align='center'>
<img src='https://github.com/msikorski93/Pneumonia-Recognition-With-Deep-Learning-and-TensorFlow/assets/45270023/f43ae5a6-cf86-4b3c-a696-e69015953a84' width='400' style='background-color:white;'/>
</p>
