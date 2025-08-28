# Image-Classification-using-CNN-MobileNetV2
INTRODUCTION 
In the era of deep learning, image classification plays a vital role in applications ranging from 
medical imaging to object detection in daily life. The goal of this project is to classify images 
of three electronic devices—Mobile Phones, Laptops, and Earpods using Convolutional 
Neural Networks (CNN) and Transfer Learning with MobileNetV2. CNNs are widely used due 
to their ability to extract spatial features from images, while transfer learning models 
leverage pre-trained weights from large datasets like ImageNet to improve performance on 
smaller, domain-specific datasets. 
OBJECTIVES 
 To build and compare two different image classification models: 
A Custom CNN trained from scratch and a MobileNetV2 Transfer Learning model
with pre-trained ImageNet weights. 
 To evaluate the performance of both models on the given dataset of Mobile, Laptop, 
and Earpod images. 
 To analyze which approach (CNN vs. MobileNetV2) provides better accuracy, 
generalization, and robustness. 
 To provide predictions on unseen images using both models. 
METHODOLOGY 
 Dataset Preparation
 Images of Mobile Phones, Laptops, and Earpods were collected and organized 
into folders. 
 Data augmentation techniques (rotation, flipping, zooming, shifting) were 
applied to increase dataset variability and avoid overfitting. 
 Model Development
 Custom CNN Model:
o Consists of convolutional layers, batch normalization, max pooling, 
dropout, and dense layers. 
o Trained from scratch on the dataset. 
 MobileNetV2 Model:
 A pre-trained MobileNetV2 model was used with ImageNet weights. 
 The base network was frozen and a custom classification head was added. 
 Training & Evaluation
 Both models were trained for 20 epochs using the Adam optimizer. 
 Sparse categorical cross-entropy loss was used since the labels were integer 
encoded. 
 Accuracy and loss were recorded for each epoch and later compared using 
plots. 
 Prediction Function
 A unified prediction function was developed to test any new image with both 
models. 
 The function displays the predicted class (Mobile, Laptop, or Earpod) along 
with the confidence score from both MobileNetV2 and CNN. 
RESULT 
 The MobileNetV2 model achieved higher accuracy and lower loss compared to the 
Custom CNN. 
 The CNN, although functional, tended to overfit and misclassified some test images 
(especially confusing between classes). 
 Transfer learning (MobileNetV2) proved more effective due to its ability to leverage 
learned representations from ImageNet, making it more robust for small datasets. 
 Visualization of training curves clearly showed better generalization in MobileNetV2 
compared to CNN. 
CONCLUSION 
This project successfully demonstrated the comparison between a Custom CNN and a 
MobileNetV2 transfer learning model for the classification of electronic device images. 
The results indicate that MobileNetV2 significantly outperforms the CNN model in terms 
of accuracy and reliability. This highlights the advantage of transfer learning when working 
with limited datasets. In practical applications, transfer learning should be preferred for 
robust and scalable solutions, while custom CNNs may still be explored for lightweight or 
highly domain-specific tasks.
