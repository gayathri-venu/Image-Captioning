# Image Captioning

Automated image captioning using Keras and Flickr8k Dataset

### Approach

1. Loading Data : 
   Extracting captions and storing into dictionary format.

2. Preparing Sequences for training :
   Create sequences for captions adding start tag at beginning and end tag at last.

3. Processing captions :
   Create a unique list of words and convert each word into a fixed sized vector.Zero padding is done so that each sequence of captions is of equal size

4. Feature Extractor :
   Pass every image to Residual Network Model to get the corresponding 2048 length feature vector and save these encoded images in train_encoded_images.p.

5. Sequence Processor :
   This is a word embedding layer for handling the text input, followed by a Long Short-Term Memory (LSTM) recurrent neural network layer.

6. Fitting the Model :
   We fit the model on the training dataset and finally save it.

7. Prediction :
   Both the feature extractor and sequence processor output are merged together and processed by a dense layer to make a final prediction.
   
 ### Output
 
 ![Output 1](https://github.com/gayathri-venu/Image-Captioning/blob/master/output/1.png)
 
 ![Output 2](https://github.com/gayathri-venu/Image-Captioning/blob/master/output/2.png)
 
 ![Output 3](https://github.com/gayathri-venu/Image-Captioning/blob/master/output/3.png)
  
  
 
 ### Kaggle Link
 
 https://www.kaggle.com/gayathri9082/automated-image-captioning-flickr8/edit
 
 
    
  
     
    
  
