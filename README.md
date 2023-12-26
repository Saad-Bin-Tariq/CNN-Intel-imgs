# Intel Image Classification
This project is an image classification task using the Intel Image Classification dataset. The goal is to classify images into specific categories such as buildings, forests, glaciers, mountains, seas, and streets.

# Overview
The repository contains a deep learning model trained on the Intel Image Classification dataset. The model is built using a convolutional neural network (CNN) architecture to classify images into different categories.

# Requirements
Keras:
keras==2.6.0

OpenCV (cv2):
opencv-python==4.5.3.56

Matplotlib:
matplotlib==3.4.3

NumPy:
numpy==1.21.2

scikit-learn:
scikit-learn==0.24.2

# Features
Utilizes a CNN architecture for image classification.
Handles multi-class classification for various environmental scenes.
Implements data preprocessing, model training, and evaluation.
Copy code

# Clone the repository
$ git clone https://github.com/Saad-Bin-Tariq/CNN-Intel-imgs.git

# Navigate to the project directory
$ cd intel-image-classification


Usage
To use the project:

Download the Intel Image Classification dataset and place it in the appropriate directory.
Run the data preprocessing scripts to prepare the dataset.
Train the model using the provided scripts or Jupyter notebooks.
Evaluate the model's performance on the test dataset.
bash
Copy code
# Example commands for usage
$ python ML_Assignment_3_340594_SaadBinTariq.ipynb
# Intel Data 
![image](https://github.com/Saad-Bin-Tariq/CNN-Intel-imgs/assets/87191427/bde6a373-7160-451e-8c92-a74abb259e48)
# Model Architecture
![image](https://github.com/Saad-Bin-Tariq/CNN-Intel-imgs/assets/87191427/7e811b37-cd5e-424b-8f8e-4d3096aa85d1)
# Pre-trained Model weights 
Model Architecture:
________________________________________________________________
 Layer (type)                Output Shape              Param   
=================================================================
 conv2d (Conv2D)             (None, 148, 148, 200)     5600      
                                                                 
 conv2d_1 (Conv2D)           (None, 146, 146, 180)     324180    
                                                                 
 max_pooling2d (MaxPooling2  (None, 29, 29, 180)       0         
 D)                                                              
                                                                 
 conv2d_2 (Conv2D)           (None, 27, 27, 180)       291780    
                                                                 
 conv2d_3 (Conv2D)           (None, 25, 25, 140)       226940    
                                                                 
 conv2d_4 (Conv2D)           (None, 23, 23, 100)       126100    
                                                                 
 conv2d_5 (Conv2D)           (None, 21, 21, 50)        45050     
                                                                 
 max_pooling2d_1 (MaxPoolin  (None, 4, 4, 50)          0         
 g2D)                                                            
                                                                 
 flatten (Flatten)           (None, 800)               0         
                                                                 
 dense (Dense)               (None, 180)               144180    
                                                                 
 dense_1 (Dense)             (None, 100)               18100     
                                                                 
 dense_2 (Dense)             (None, 50)                5050      
                                                                 
 dropout (Dropout)           (None, 50)                0         
                                                                 
 dense_3 (Dense)             (None, 6)                 306       

Weights for each layer:
----------------------------------------
conv2d_1: (3, 3, 3, 200)
conv2d_2: (3, 3, 200, 180)
...
dense_1: (800, 180)
dense_2: (180, 100)
dense_3: (100, 50)
dense_4: (50, 6)
----------------------------------------


These details provide an overview of the model architecture and the shapes of the weights for each layer. Replace the (None, ...) output shapes with the actual output shapes if they're known. This information helps users understand the structure of your model and the dimensions of weights associated with each layer.
# Accuracy Graphs 
![image](https://github.com/Saad-Bin-Tariq/CNN-Intel-imgs/assets/87191427/2bd80b20-4def-4329-9ce7-22eed661feaf)
# Predicted Output Classes
![image](https://github.com/Saad-Bin-Tariq/CNN-Intel-imgs/assets/87191427/38dd1b01-fe6e-4fa4-947b-bce60b3fec28)

Contributing
Contributions are welcome! If you wish to contribute to this project:

# Fork the repository.
Create a new branch (git checkout -b feature-branch).
Make your changes and commit them (git commit -am 'Add feature').
Push to the branch (git push origin feature-branch).
Create a new Pull Request.
# License
This project is licensed under the MIT License. For more details, see the LICENSE file.
