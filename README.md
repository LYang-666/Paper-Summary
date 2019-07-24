# Paper-Summary
Inspired by [Awesome Pruning](https://github.com/he-y/Awesome-Pruning#type-of-pruning).
Papers I have read and try to follow up

* [Filter Pruning via Geometric Median for Deep Convolutional Neural Networks Acceleration](https://arxiv.org/abs/1811.00250) | CVPR 2019 | [github](https://github.com/he-y/filter-pruning-geometric-median)
  
  Very good introduction and related work which divide the pruning into weight pruning and filter pruning. For the filter pruning, it's also separated to data dependent, eg., norm based regularization, and data independent, eg., directly pruning the filter by smaller-norm-less-important asumption.
  
  Tow requirments for norm-based criterion: 1. large norm deviation. 2. small minimum norm.
* Data Independent filter pruning
  * [PRUNING FILTERS FOR EFFICIENT CONVNETS](https://arxiv.org/pdf/1608.08710.pdf) | ICLR 2017 |
  
  Good analysis on sensitive of resnet layers to be pruned. 
  1. "(layers 20, 38 and 54 for ResNet-56, layer 36, 38 and 74 for      ResNet-110) lie at the residual blocks close to the layers where the number of feature maps changes, e.g., the first and the last residual blocks for each stage. We believe this happens because the precise residual errors are necessary for the newly added empty feature maps."
    Solution: The retraining performance can be improved by skipping these sensitive layers.
  
  2. " We find that deeper layers are more sensitive to pruning than layers in the earlier stages of the network."
    Solution: "we use a different pruning rate for each stage."
  
* Data dependent filter pruning
  * [Learning Efficient Convolutional Networks through Network Slimming](https://arxiv.org/pdf/1708.06519.pdf) | ICCV 2017 | [github](https://github.com/liuzhuang13/slimming)
  
# Related Repo
[Awesome Pruning](https://github.com/he-y/Awesome-Pruning#type-of-pruning)

[Awesome-model-compression-and-acceleration](https://github.com/memoiry/Awesome-model-compression-and-acceleration)

[EfficientDNNs](https://github.com/MingSun-Tse/EfficientDNNs)

[Embedded-Neural-Network](https://github.com/ZhishengWang/Embedded-Neural-Network)

[awesome-AutoML-and-Lightweight-Models](https://github.com/guan-yuan/awesome-AutoML-and-Lightweight-Models)

[Model-Compression-Papers](https://github.com/chester256/Model-Compression-Papers)

[knowledge-distillation-papers](https://github.com/lhyfst/knowledge-distillation-papers)

[Network-Speed-and-Compression](https://github.com/mrgloom/Network-Speed-and-Compression)
