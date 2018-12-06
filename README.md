# Airbus Ship Detection Challenge

This is an open solution to the [Airbus Ship Detection Challenge](https://www.kaggle.com/c/airbus-ship-detection).

### Description
The project is based on [PyTorch](http://pytorch.org/) deep learning framework. For this binary segmentation task I used [U-Net](https://arxiv.org/abs/1505.04597) model. Trained the network with three weight initialization schemes: LeCun uniform, the encoder with weights from VGG11 and full network trained on the Carvana datase. For more details: [arXiv paper](https://arxiv.org/abs/1801.05746).

I also tried to train another network that detects is there any ship in a satellite image or not using transfer learing to increase accuracy of segmentation model. 
For better performance I tried to use different training tekniques like: [Cyclical Learning Rate] (https://arxiv.org/abs/1506.01186), [SGDR](https://arxiv.org/abs/1608.03983), [FGE](https://arxiv.org/abs/1802.10026), [SWA](https://arxiv.org/abs/1803.05407). However, because of the luck of time and compute power I didn't manage to use them all.
