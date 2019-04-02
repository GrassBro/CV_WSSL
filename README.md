# Weakly Supervised Learning in Computer Visiion (In Collecting...)

## 1. Object Detection
### 1.1 Class Label Supervision

* [Weakly supervised object detection with convex clustering](https://www.cv-foundation.org/openaccess/content_cvpr_2015/papers/Bilen_Weakly_Supervised_Object_2015_CVPR_paper.pdf), CVPR 2015.

* [Weakly Supervised Deep Detection Networks](http://homepages.inf.ed.ac.uk/hbilen/assets/pdf/Bilen16.pdf), CVPR 2016. [[code]](https://github.com/hbilen/WSDDN)
  * Perform simultaneously region selection and classification
  * Region score 

* [Multiple Instance Detection Network with Online Instance Classifier Refinement](https://arxiv.org/pdf/1704.00138.pdf), CVPR 2017.

* [Weakly Supervised Object Localization with Multi-fold Multiple Instance Learning](https://arxiv.org/pdf/1503.00949.pdf), PAMI 2017. 

* [Weakly Supervised Region Proposal Network and Object Detection](http://pengtang.xyz/publications/0640.pdf), ECCV 2018.  
  * Stage 1: Evaluating bjectness score of sliding windows based on low-level features;  
  * Stage 2: Proposal refinement based on classifier;   
  * Shared convolutional computations.

* [TS2C: Tight Box Mining with Surrounding Segmentation Context for Weakly Supervised Object Detection](), ECCV 2018.
  * Semantic Segmentation Confidence Map.
  * Compute objectness scores for the regions inside and outside the box.
  

### 1.2 Class and Count Labels as Supervision

* [C-WSL: Count-guided Weakly Supervised Localization](http://openaccess.thecvf.com/content_ECCV_2018/papers/Mingfei_Gao_C-WSL_Count-guided_Weakly_ECCV_2018_paper.pdf), ECCV 2018.
  * per-class object count
  * count-based region selection algorithm

* [Object Counting and Instance Segmentation with Image-level Supervision](https://arxiv.org/pdf/1903.02494.pdf), CVPR 2019.
  * Instance level segmentation using peak response and count knowledge
  * Only per-class counts in subitizing range are provided
  

## 2. Object Localization

* [Attention Networks for Weakly Supervised Object Localization](http://www.cs.umanitoba.ca/~ywang/papers/bmvc16_attention.pdf), BMVC 2016.
  * computes an attention score on each candidate region in the image.
  * candidate regions are combined together with their attention scores to form a whole-image feature vector. This feature vector is     used for classifying the image.

* [ContextLocNet: Context-Aware Deep Network Models for Weakly Supervised Localization](https://link.springer.com/content/pdf/10.1007%2F978-3-319-46454-1_22.pdf), ECCV 2016.
  * Leverage their surrounding context regions to improve localization.

* [Self-produced Guidance for Weakly-supervised Object Localization](http://openaccess.thecvf.com/content_ECCV_2018/papers/Xiaolin_Zhang_Self-produced_Guidance_for_ECCV_2018_paper.pdf), ECCV 2018. [[code]](https://github.com/xiaomengyc/SPG)

* [Self-Erasing Network for Integral Object Attention](https://arxiv.org/abs/1810.09821), NeurIPS 2018.
  

## 3. Semantic Segmentation

* [Seed, Expand and Constrain: Three Principles for Weakly-Supervised Image Segmentation](https://arxiv.org/pdf/1603.06098.pdf), ECCV 2016.
  * Train saliency model using Deeplab-V2 Resnet architecture based on MSRA dataset, which contains bounding box annotations.

* [Exploiting saliency for object segmentation from image level labels](https://arxiv.org/pdf/1701.08261.pdf), CVPR 2017. [[code]](https://github.com/coallaoh/GuidedLabelling)
  * Finding the object location (any point on the object)
  * Finding the object's extent = Finding the background area
  * Explore the importance of saliency for seed generation

* [Two-Phase Learning for Weakly Supervised Object Localization](https://arxiv.org/pdf/1708.02108.pdf), ICCV 2017.

## 4. Salient Object Detection

* [Multi-source Weak Supervision for saliencly detection](https://128.84.21.199/abs/1904.00566), CVPR 2019. [[code]]()


