# Weakly-/Semi-Supervised Learning in Computer Visiion 
  (In Collecting...)

## 1. Object Detection
### 1.1 Class Label Supervision

* [Weakly supervised object detection with convex clustering](https://www.cv-foundation.org/openaccess/content_cvpr_2015/papers/Bilen_Weakly_Supervised_Object_2015_CVPR_paper.pdf), CVPR 2015.

* [Weakly Supervised Deep Detection Networks](http://homepages.inf.ed.ac.uk/hbilen/assets/pdf/Bilen16.pdf), CVPR 2016. [[code]](https://github.com/hbilen/WSDDN)
  * Perform simultaneously region selection and classification
  * Region score 

* [Multiple Instance Detection Network with Online Instance Classifier Refinement](https://arxiv.org/pdf/1704.00138.pdf), CVPR 2017.

* [Weakly Supervised Object Localization with Multi-fold Multiple Instance Learning](https://arxiv.org/pdf/1503.00949.pdf), PAMI 2017. 

* [W2F: A Weakly-Supervised to Fully-Supervised Framework for Object Detection](http://openaccess.thecvf.com/content_cvpr_2018/papers/Zhang_W2F_A_Weakly-Supervised_CVPR_2018_paper.pdf), CVPR 2018.
  * Using generated pseudo ground-truth to train fully-supervised RPN

* [Min-Entropy Latent Model for Weakly Supervised Object Detection](http://openaccess.thecvf.com/content_cvpr_2018/papers/Wan_Min-Entropy_Latent_Model_CVPR_2018_paper.pdf), CVPR 2018.
  * Min-entropy is used as a metric to measure the randomness of object localization during learning, as well as serving as a model to learn object locations.

* [Weakly Supervised Region Proposal Network and Object Detection](http://pengtang.xyz/publications/0640.pdf), ECCV 2018.  
  * Stage 1: Evaluating bjectness score of sliding windows based on low-level features;  
  * Stage 2: Proposal refinement based on classifier;   
  * Shared convolutional computations.

* [TS2C: Tight Box Mining with Surrounding Segmentation Context for Weakly Supervised Object Detection](https://arxiv.org/pdf/1807.04897.pdf), ECCV 2018.
  * Semantic Segmentation Confidence Map.
  * Compute objectness scores for the regions inside and outside the box.
  
* [You reap what you sow: Using Videos to Generate High Precision Object Proposals for Weakly-supervised Object Detection](http://krsingh.cs.ucdavis.edu/krishna_files/papers/w-rpn/w-rpn.pdf), CVPR 2019.

* [Dissimilarity Coefficient based Weakly Supervised Object Detection](https://arxiv.org/pdf/1811.10016.pdf), CVPR 2019.
  

### 1.2 Class and Count Labels as Supervision

* [C-WSL: Count-guided Weakly Supervised Localization](http://openaccess.thecvf.com/content_ECCV_2018/papers/Mingfei_Gao_C-WSL_Count-guided_Weakly_ECCV_2018_paper.pdf), ECCV 2018.
  * per-class object count
  * count-based region selection algorithm

### 1.3 Applications

* [Cross-Domain Weakly-Supervised Object Detection through Progressive Domain Adaptation](http://openaccess.thecvf.com/content_cvpr_2018/papers/Inoue_Cross-Domain_Weakly-Supervised_Object_CVPR_2018_paper.pdf), CVPR 2018.



  

## 2. Object Localization

* [Attention Networks for Weakly Supervised Object Localization](http://www.cs.umanitoba.ca/~ywang/papers/bmvc16_attention.pdf), BMVC 2016.
  * computes an attention score on each candidate region in the image.
  * candidate regions are combined together with their attention scores to form a whole-image feature vector. This feature vector is     used for classifying the image.

* [ContextLocNet: Context-Aware Deep Network Models for Weakly Supervised Localization](https://link.springer.com/content/pdf/10.1007%2F978-3-319-46454-1_22.pdf), ECCV 2016.
  * Leverage their surrounding context regions to improve localization.

* [Self-produced Guidance for Weakly-supervised Object Localization](http://openaccess.thecvf.com/content_ECCV_2018/papers/Xiaolin_Zhang_Self-produced_Guidance_for_ECCV_2018_paper.pdf), ECCV 2018. [[code]](https://github.com/xiaomengyc/SPG)

* [Self-Erasing Network for Integral Object Attention](https://arxiv.org/abs/1810.09821), NeurIPS 2018.

* [Attention-based Dropout Layer for Weakly Supervised Object Localization](http://openaccess.thecvf.com/content_CVPR_2019/papers/Choe_Attention-Based_Dropout_Layer_for_Weakly_Supervised_Object_Localization_CVPR_2019_paper.pdf), CVPR 2019(Oral).[[code]](https://github.com/junsukchoe/ADL)
  

## 3. Semantic Segmentation

### 3.1 Class Label Supervision

* [Seed, Expand and Constrain: Three Principles for Weakly-Supervised Image Segmentation](https://arxiv.org/pdf/1603.06098.pdf), ECCV 2016.

* [Exploiting saliency for object segmentation from image level labels](https://arxiv.org/pdf/1701.08261.pdf), CVPR 2017. [[code]](https://github.com/coallaoh/GuidedLabelling)
  * Finding the object location (any point on the object)
  * Finding the object's extent = Finding the background area
  * Explore the importance of saliency for seed generation
  * Train saliency model using Deeplab-V2 Resnet based on MSRA dataset, which contains bounding box annotations.

* [Two-Phase Learning for Weakly Supervised Object Localization](https://arxiv.org/pdf/1708.02108.pdf), ICCV 2017.

### 3.2 Scribble Supervision

* [ScribbleSup: Scribble-Supervised Convolutional Networks for Semantic Segmentation](https://arxiv.org/pdf/1604.05144.pdf), CVPR 2016.

* [On Regularized Losses for Weakly-supervised CNN Segmentation](http://openaccess.thecvf.com/content_ECCV_2018/papers/Meng_Tang_On_Regularized_Losses_ECCV_2018_paper.pdf), ECCV 2018.


## 4. Instance Segmentation
* [Weakly Supervised Learning of Instance Segmentation with Inter-pixel Relations](https://arxiv.org/pdf/1904.05044.pdf), CVPR 2019(Oral).

* [Object Counting and Instance Segmentation with Image-level Supervision](https://arxiv.org/pdf/1903.02494.pdf), CVPR 2019.
  * Instance level segmentation using peak response and count knowledge
  * Only per-class counts in subitizing range are provided

* [Where are the Masks: Instance Segmentation with Image-level Supervision](https://arxiv.org/pdf/1907.01430.pdf), BMVC 2019.



## 4. Salient Object Detection

### 4.1 Image

* [Learning to Detect Salient Objects with Image-level Supervision](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8099887), CVPR 2017. [[code]](https://github.com/scott89/WSS)

* [Weakly-supervised Salient Object detection using Image Labels](https://arxiv.org/abs/1803.06503), AAAI 2018.

* [Multi-source Weak Supervision for saliencly detection](https://arxiv.org/pdf/1904.00566), CVPR 2019. [[code]](https://github.com/zengxianyu/mws)

* [Joint learning of saliency detection and weakly supervised semantic segmentation](http://ice.dlut.edu.cn/lu/publications.html), ICCV 2019 (Not released Yet).

### 4.2 Video

* [Semi-Supervised Video Salient Object Detection Using Pseudo-Labels](http://guanbinli.com/pb.html), ICCV 2019 (Not released Yet).




