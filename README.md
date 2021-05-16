# ChexNet-Keras
DELAX-TB is a deep learning tool and architecture for detection of TB in x-ray scans. It's based on CheXnet and the source is based off of  Bruce Chou's work at https://github.com/brucechou1983/CheXNet-Keras 

Refer to the README at https://github.com/brucechou1983/CheXNet-Keras

ChexNet is a deep learning algorithm that can detect and localize 14 kinds of diseases from chest X-ray images. As described in the paper, a 121-layer densely connected convolutional neural network is trained on ChestX-ray14 dataset, which contains 112,1\20 frontal view X-ray images from 30,805 unique patients. The result is so good that it surpasses the performance of practicing radiologists. 

1. We took the original model from Bruce's source and loaded the saved weights he shared
2. Replaced the last layer with a 3 node dense layer for tb,normal,uncertain categories of x-ray scans 
3. Re-trained the model with our samples 
4. Saved our new model 
5. converted the save model to tensorflowjs 
6. Use this tfjs model.json and bins for the DELAX-TB prototype


## License
MIT
