#DELAX-TB
DELAX-TB is a deep learning tool and architecture for detection of TB in x-ray scans. It's based on CheXnet and the source is based off of  Bruce Chou's work at https://github.com/brucechou1983/CheXNet-Keras 

Refer to the README at https://github.com/brucechou1983/CheXNet-Keras for the initial setup.

[ChexNet](https://arxiv.org/pdf/1711.05225.pdf) is a deep learning algorithm that can detect and localize 14 kinds of diseases from chest X-ray images. As described in the paper, a 121-layer densely connected convolutional neural network is trained on ChestX-ray14 dataset, which contains 112,1\20 frontal view X-ray images from 30,805 unique patients. The result is so good that it surpasses the performance of practicing radiologists. 

In this project:
1. We took the original model from Bruce's source and loaded the saved "based" weights he shared
2. Employing transfer learning, we replaced the last layer with a 3 node dense layer for tb,normal,uncertain categories of x-ray scans 
3. Re-trained the model with our samples 
4. Saved our new model 
5. Converted the saved model to tensorflowjs 
6. Usec this tfjs model.json and bins for the  [DELAX-TB](https://nera-gbh.org/delax-tb.html)  prototype 


## License
MIT
