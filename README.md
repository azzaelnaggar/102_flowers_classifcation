# 102_flowers_classifcation Pytorch :maple_leaf::sunflower: 
:bookmark_tabs: You can find the Data here https://www.robots.ox.ac.uk/~vgg/data/flowers/102/

:hibiscus: Oxford 102 Flower is an image classification dataset consisting of 102 flower categories.
The flowers chosen to be flowers commonly occur in the United Kingdom. Each class consists of between 40 and 258 images.

:bar_chart: The images have large scale, pose, and light variations. In addition, some categories have large variations within the category and several very similar categories.

:bulb: Udacity provided label mapping in JSON file so load it for later use.

:point_right: Using ResNet50 . In our case, I want to predict 102 flower classes so I use an ordered dictionary to create the final layers of my network with 102 outputs. So I define a new untrained feed-forward network as a classifier, using ReLU activations and dropout. 
LogSoftmax is used for the output values from the model for each image prediction.

:exclamation: For more epochs, this notebook is based on 40 epochs (data_modeling_40epoch.ipynb) the train acc increases but the test acc decrease Not much.

:bulb: To improve the model we need to perform oversampling for imbalanced classes




