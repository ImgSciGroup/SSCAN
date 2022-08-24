# SSCAN: Novel Spatial-Spectral Channel Attentions Neural Network for LCCD With Remote Sensing Images
#2022-8-24  @Author: LvZhiYong 
 
#The training data size channel used by our proposed method is 56*56*3
#The test set and validation set size are both 56*56*3, and the label is 56*56*1
#
# SSCAN: Novel Spatial-Spectral Channel Attentions Neural Network for LCCD With Remote Sensing Images
Change detection is a fundamental task in remote sensing image processing. The research goal is to identify interesting change information and filter out irrelevant change information as interference factors. Recently, the rise of deep learning has provided new tools for change detection with impressive results. However, existing methods mainly focus on the difference information between multi-temporal remote sensing images and lack robustness to pseudo-change information. To overcome the lack of resistance of current methods to spurious changes, in this paper, we propose a new method, the Double-Attention Fully Convolutional Siamese Network (SSCAN), for change detection in high-resolution images. Through the dual attention mechanism, long-range dependencies are captured and more discriminative feature representations are obtained, thereby improving the recognition performance of the model. Furthermore, sample imbalance is a serious problem in change detection, i.e., unchanged samples are much more abundant than changed samples, which is one of the main reasons for spurious changes. We propose a weighted bilateral distance contrast loss to address this problem by penalizing the attention on invariant feature pairs and increasing the attention on changing feature pairs. The experimental results of our method on the change detection dataset (CDD) and the landslide change detection dataset (LCCD) show that this method has the greatest improvement compared to other baseline methods.
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
