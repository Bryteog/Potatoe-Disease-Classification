#### Overview

Built a model to classify potatoes leafs as either healthy or diseased, the classes are: "Healthy", "Early blight" and "Late blight". The dataset is obtained from kaggle and forms part of the [Plant Village](https://www.kaggle.com/datasets/arjuntejaswi/plant-village) directory of various plant leafs. The data directory contains leaf images belonging to the three classes split into 75, 15, 10 sizes for training, validation and testing respectively. Data analysis is done with the Pandas library.


#### Model

Image preprocessing via flipping, rescaling, normalising, zooming and rotation is applied to the train set only. The model has two versions which differ in duration of training.

The accuracy of training and testing sets for version 1 after 10 epochs is 90% and 91% respectively with losses of 0.249 and 0.1994.

Version 2 uses the mobilenet_v2 prtrained model and after training for 12 epochs had 99.3% and 95.86% accuracy and losses of 0.1672 and 0.2791 for both the training and testing sets respectively.
