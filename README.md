<h2>Objective :</h2>
<p>To develop a gender and age detection system that can accurately determine the gender and age of the person (face) from human face images and real-time video streams from mobile camera.</p>

<h2>About the Project :</h2>
<p>We build deep learning models to predict age and gender from face pictures and real time video streams, which make use of TensorFlow and Keras. In this project, we have used MobileNetV2 as a foundational model, augmenting it with more thick layers. Custom data generators are used to apply data augmentation strategies during training. Appropriate optimization strategies, loss functions, and assessment measures are integrated into the models. To make training and monitoring more efficient, we've included callbacks like ModelCheckpoint, EarlyStopping, and ReduceLROnPlateau. Achieving an accuracy of 93.41% and a loss of 0.1737 for the gender model and a loss of 48.1983 and a mean absolute error of 4.9132 for the age model, respectively.</p>

<h2>Dataset :</h2>
<p>For this project, we have used the UTKFace dataset; the dataset is available in the public domain and you can find it <a href="https://www.kaggle.com/datasets/jangedoo/utkface-new">here</a>. 

UTKFace dataset is a large-scale face dataset with long age span (range from 0 to 116 years old). The dataset consists of over 20,000 face images with annotations of age, gender, and ethnicity. The images cover large variation in pose, facial expression, illumination, occlusion, resolution, etc. This dataset could be used on a variety of tasks, e.g., face detection, age estimation, age progression/regression, landmark localization, etc. The models I used had been trained on this dataset.</p>

<h2>Python Libraries Required :</h2>
<ul>
  <li>OpenCV</li>
  
       pip install opencv-python
</ul>
<ul>
 <li>TensorFlow</li>
  
       pip install tensorflow
</ul>
<ul>
 <li>Keras</li>
  
       pip install keras
</ul>

<h2>The contents of this Project :</h2>
<ul>
  <li>opencv_face_detector.pbtxt</li>
  <li>opencv_face_detector_uint8.pb</li>
  <li>age_deploy.prototxt</li>
  <li>age_net.caffemodel</li>
  <li>gender_deploy.prototxt</li>
  <li>gender_net.caffemodel</li>
  <li>a few pictures to try the project on</li>
  <li>detect.py</li>
 </ul>
 <p>For face detection, we have a .pb file- this is a protobuf file (protocol buffer); it holds the graph definition and the trained weights of the model. We can use this to run the trained model. And while a .pb file holds the protobuf in binary format, one with the .pbtxt extension holds it in text format. These are TensorFlow files. For age and gender, the .prototxt files describe the network configuration and the .caffemodel file defines the internal states of the parameters of the layers.</p>
 
 


