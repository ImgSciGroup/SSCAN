# SSCAN: Novel Spatial-Spectral Channel Attentions Neural Network for LCCD With Remote Sensing Images
#2022-8-24  @Author: LvZhiYong 
 
#The training data size channel used by our proposed method is 56*56*3
#The test set and validation set size are both 56*56*3, and the label is 56*56*1
#
# SSCAN: Novel Spatial-Spectral Channel Attentions Neural Network for LCCD With Remote Sensing Images
Land cover change detection (LCCD) with remote sensing images plays an important role in observing the Earth’s surface change, and the spatial-spectral channels attention mechanism has become attractive in recent years. This paper proposed a Spatial-Spectral Channels Attentions Neural Network (SSCAN) for achieving LCCD using remote sensing images. In the proposed SSCAN, different from the traditional methods, to enhance the changed area and inhibit the unchanged area, the spatial channel attention module (SCAM) and convolution block attention module (CBAM) are employed to process the pre-event and post-event image, respectively. Moreover, a simple yet effect Batch size Dynamic Adjustment (BDA) strategy is promoted to train the proposed SSCAN for guaranteeing convergence to the global optima of the objective function. Experiments based on comparing seven cognate and state-of-art methods well demonstrated that the proposed network has some advantages in accelerating the network convergence speed, reinforcing the learning efficiency, and improving the performance of LCCD.
<!-- Pytorch implementation of change detection like [SSCAN: Novel Spatial-Spectral Channel Attentions Neural Network for LCCD With Remote Sensing Images]
## Require
Most of the problems in the problem list are caused by the version of python or pytoch.
We updated the source code to accommodate the new version of pytorch.
Hope our repo is useful to you.
- Python3.6
- Pytorch 1.3.1 (see: [pytorch installation instructions](http://pytorch.org/))
## data set
This Hong Kong Lantau landslide was constructed for remote sensing change detection. We report performance on multiple datasets.
 
### Directory Structure
 
The file structure is as follows:
#####
--data -- --- train
           ------ test
           ------ val
---image
---model
---utils
---test.py
--train.py
####
##################
## train the model
Backbone model of SSCAN
## Quote
