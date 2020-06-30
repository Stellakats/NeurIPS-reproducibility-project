# NeurIPS-reproducibility-project

 
The aim of this project was to re-implement methods discussed in the paper [Learning where to look: Semantic-Guided Multi-Attention Localization for Zero-ShotLearning] (https://arxiv.org/abs/1903.00502) from scratch using Tensorflow 2.0. The code of the original paper was written in PyTorch and had not been made publicly available.
 
The conventional image classification process is limited to classifying instances of already seen classes, although in real life scenarios there exist object classes that the model is not trained on. 
The method presented in the paper, aims to classify instances by semantic-guided Zero Shot Learning for seen and unseen data. 
This is achieved by developing a complex network that consists of three subnetworks: one that implements attention on the input image in order to focus on discriminative parts of the image. A second one that utilizes the attention maps produced, by cropping the image so that the highest value of the map is at the center of a square. And a third one, which is called “joint feature learning subnet”, receives the original images as well as the cropped ones, extracts their features and maps them to the semantic space producing a compatibility score.
Three types of losses, one of them custom-made, are employed to support the optimization of the model.
The original code can be foung [here](https://github.com/LindsayXX/DD2412_project).
 
