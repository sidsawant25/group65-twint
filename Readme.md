### Multi Class Classifier
Python Jupyter Notebook with Convolutional Neural Network implemented in Keras.


### Structure of Data
/
	train.csv
    test.csv

    
### Libraries Required:-
pandas, numpy, matplotlib, sklearn, tensorflow

###Installation Commands:-
pip install pandas
pip install matplotlib
pip install scikit-learn
pip install tensorflow


### Dataset:-
In train.csv each row corresponds to one sequence sample, with sample ID, features of all frames and label ID.
Each sequence contains 16 frames.  Each frame contains the motion features of 20 skeleton joints of a human body.
More specifically, each joint is represented with features in x, y, z axes in 3D space.  Thus each frame contains 20×3 = 60 features.

### Performance:-

Model Summary
Model: "sequential_8"
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
_________________________________________________________________
conv2d_24 (Conv2D)           (None, 16, 60, 64)        640       
_________________________________________________________________
batch_normalization_38 (Batc (None, 16, 60, 64)        256       
_________________________________________________________________
max_pooling2d_24 (MaxPooling (None, 8, 30, 64)         0         
_________________________________________________________________
dropout_24 (Dropout)         (None, 8, 30, 64)         0         
_________________________________________________________________
conv2d_25 (Conv2D)           (None, 8, 30, 128)        73856     
_________________________________________________________________
batch_normalization_39 (Batc (None, 8, 30, 128)        512       
_________________________________________________________________
max_pooling2d_25 (MaxPooling (None, 4, 15, 128)        0         
_________________________________________________________________
dropout_25 (Dropout)         (None, 4, 15, 128)        0         
_________________________________________________________________
conv2d_26 (Conv2D)           (None, 4, 15, 256)        295168    
_________________________________________________________________
batch_normalization_40 (Batc (None, 4, 15, 256)        1024      
_________________________________________________________________
max_pooling2d_26 (MaxPooling (None, 2, 7, 256)         0         
_________________________________________________________________
dropout_26 (Dropout)         (None, 2, 7, 256)         0         
_________________________________________________________________
flatten_8 (Flatten)          (None, 3584)              0         
_________________________________________________________________
dense_24 (Dense)             (None, 128)               458880    
_________________________________________________________________
batch_normalization_41 (Batc (None, 128)               512       
_________________________________________________________________
dense_25 (Dense)             (None, 112)               14448     
_________________________________________________________________
batch_normalization_42 (Batc (None, 112)               448       
_________________________________________________________________
dense_26 (Dense)             (None, 49)                5537      
_________________________________________________________________
Total params: 851,281
Trainable params: 849,905
Non-trainable params: 1,376
_________________________________________________________________

#### Model1 - Accuracy
![Model 1](https://i.ibb.co/PzT1bHR/plot.jpg)

#### Model2 - Accuracy
![Model 2](https://i.ibb.co/PzT1bHR/plot.jpg)

#### Model3 - Accuracy
![Model 3](https://i.ibb.co/PzT1bHR/plot.jpg)

#### Model4 - Accuracy
![Model 4](https://i.ibb.co/PzT1bHR/plot.jpg)

#### Model5 - Accuracy
![Model 5](https://i.ibb.co/PzT1bHR/plot.jpg)

#### Model6 - Accuracy
![Model 6](https://i.ibb.co/PzT1bHR/plot.jpg)

#### Model7 - Accuracy
![Model 7](https://i.ibb.co/PzT1bHR/plot.jpg)

#### Model8 - Accuracy
![Model 8](https://i.ibb.co/PzT1bHR/plot.jpg)

#### Model9 - Accuracy
![Model 9](https://i.ibb.co/PzT1bHR/plot.jpg)

