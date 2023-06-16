# 102_flowers_classifcation Pytorch :maple_leaf::sunflower: 
:bookmark_tabs: You can find the Data here https://www.robots.ox.ac.uk/~vgg/data/flowers/102/
Oxford 102 Flower is an image classification dataset consisting of 102 flower categories :hibiscus: .
The flowers chosen to be flower commonly occurring in the United Kingdom. Each class consists of between 40 and 258 images.

:bar_chart: The images have large scale, pose and light variations. In addition, there are categories that have large variations within the category and several very similar categories.

:bulb: Udacity provided label mapping in JSON file so just load it for later use.

:point_right: Using ResNet50 . In our case, I want predict 102 flower classes so I use ordered dictionary to create the final layers of my network with 102 output. So I define new untrained feed-forward network as a classifier, using ReLU activations and dropout. 
LogSoftmax is used for the output values from the model for each image prediction.

:exclamation: I saved the model called (classifier_V2.pth) in the repo.

:exclamation: For more epochs this notebook based on 40 epochs (data_modeling_40epoch.ipynb) the train acc increse but test acc decrease Not much.



