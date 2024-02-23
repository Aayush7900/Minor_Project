model7
    added input layer and output layer with l2=0.005 regularization fine tuned at 152 layer trained over 20 epochs

model8
    added input layer and output layer with l2=0.005 regularization fine tuned at 152 layer trained over 25 epochs

model9
    added input layer and output layer with l2=0.005 regularization fine tuned at 152 layer trained over 30 epochs

model10
    added input layer and output layer with l2=0.005 regularization fine tuned at 152 layer trained over 30+5 epochs learning rate increased to 0.0001

model11
    added input layer , dense 16 layer and output layer with l2=0.005 regularization base model freezed layer trained over 30+5 epochs learning rate 0.00001

model12 
    added input layer, two 32 dense layers and output layer with l2 regularization base model freezed trained over 30 epochs learning rate 0.00001
    also added a unknown class with random  images
    
model12.1
    changed learning rate to 0.00003 and trained another 10 epochs

model12.2
    changed learning rate to 0.00003 and trained another 15 epochs

model12.3
    changed learning rate to 0.00003 and trained another 35 epochs

model13
Model: "model_1"
_________________________________________________________________
 Layer (type)                Output Shape              Param #   
=================================================================
 input_3 (InputLayer)        [(None, 224, 224, 3)]     0         
                                                                 
 mobilenetv2_1.00_224 (Funct  (None, 7, 7, 1280)       2257984   
 ional)                                                          
                                                                 
 global_max_pooling2d_1 (Glo  (None, 1280)             0         
 balMaxPooling2D)                                                
                                                                 
 dropout_2 (Dropout)         (None, 1280)              0         
                                                                 
 dense_3 (Dense)             (None, 64)                81984     
                                                                 
 dropout_3 (Dropout)         (None, 64)                0         
                                                                 
 dense_4 (Dense)             (None, 64)                4160      
                                                                 
 dense_5 (Dense)             (None, 6)                 390       
                                                                 
=================================================================
Total params: 2,344,518
Trainable params: 1,446,534
Non-trainable params: 897,984

added input layer, two 64 dense layers and output layer with l2 regularization 
base model unfreezed at 130th layer trained over 50 epochs learning rate 0.00003
also added a unknown class with random  images

