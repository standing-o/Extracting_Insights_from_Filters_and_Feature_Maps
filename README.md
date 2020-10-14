# Extracting insights from filters and feature maps (20201013)  
- Classification of leaf images such as Hypersensitive reaction (HR), normal, mosaic virus
- Visualization of filters and feature maps in leaf disease image classifiers.
- In this way, we can visually identify which features have a significant impact on classification, and further extract the visual characteristics of the three kinds of leaf states.  
- This repo is maintained by 오서영, [정명지](https://github.com/mongdii)  

## Dataset  
- 804 images belonging to 3 classes by using google image crawling

## Results
#### 1. Baseline CNN with (32, 32) target size
- 50 iterations, 1 batch  
Train accuracy : 97.60%  
Val accuracy : 96.63%  

#### 2. Baseline CNN with **(128, 128)** target size
- **30** iterations, 1 batch  
Train accuracy : 98.40%  
Val accuracy : 97.19%  

## Visualization  
#### Test sample - leaf infected with mosaic virus
<div align="center">  
<img src="https://github.com/OH-Seoyoung/Extracting_insights_from_filters_and_feature_maps/blob/master/sick_sample.jpg" width="30%"> <br>
</div>

#### Filters  
- First Conv2D kernel size is (5,5) and second, third are (3,3)  
<div align="center">  
<img src="https://github.com/OH-Seoyoung/Extracting_insights_from_filters_and_feature_maps/blob/master/figure/Conv1.jpg" width="25%">  
<img src="https://github.com/OH-Seoyoung/Extracting_insights_from_filters_and_feature_maps/blob/master/figure/Conv2.jpg" width="25%"> <br>
<img src="https://github.com/OH-Seoyoung/Extracting_insights_from_filters_and_feature_maps/blob/master/figure/Conv3.jpg" width="25%"> <br>
</div>  

#### Feature maps
- 3 feature maps with test sample (mosaic virus)  
<div align="center">  
<img src="https://github.com/OH-Seoyoung/Extracting_insights_from_filters_and_feature_maps/blob/master/figure/Featuremap1.jpg" width="50%">  
<img src="https://github.com/OH-Seoyoung/Extracting_insights_from_filters_and_feature_maps/blob/master/figure/Featuremap2.jpg" width="50%"> <br>
<img src="https://github.com/OH-Seoyoung/Extracting_insights_from_filters_and_feature_maps/blob/master/figure/Featuremap3.jpg" width="50%"> <br>
</div>  

