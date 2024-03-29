<p>We build deep learning models to predict age and gender from face pictures and real time video streams, which make use of TensorFlow and Keras. In this project, we have used MobileNetV2 as a foundational model, augmenting it with more thick layers. Custom data generators are used to apply data augmentation strategies during training. Appropriate optimization strategies, loss functions, and assessment measures are integrated into the models. To make training and monitoring more efficient, we've included callbacks like ModelCheckpoint, EarlyStopping, and ReduceLROnPlateau. 
The models have been trained on kaggle using Tesla P100 GPU and inferencing is performed on google colab.

with metrics, time taken to train, machine specification of training

Mention that it has been trained on kaggle, mention the gpu

Calculate the time taken to train from adding the time per epochs
Following are the specific for each model:
- Gender Model
<ul> - accuracy of 93.41% and a 
  loss of 0.1737 for the gender model
  </ul>
 -accuracy of 93.41% and a loss of 0.1737 for the gender model 
Time taken to train:


- Age Model
loss of 48.1983 and a mean absolute error of 4.9132


</p>
