# Extracting Insights from Filters and Feature Maps
- Classification of leaf images such as Hypersensitive response (HR), normal, mosaic virus
- Visualization of filters and feature maps in leaf disease image classifiers
- In this way, we can visually identify which features have a significant impact on classification, and further extract the visual characteristics of the three kinds of leaf states.  
- This repo is maintained by 오서영, [정명지](https://github.com/mongdii)  
- Oct. 13, 2020

## Dataset  
- 804 images belonging to 3 classes by using google image crawling

## Results
#### 1. Baseline CNN with (32, 32) target size | [Code](https://github.com/OH-Seoyoung/Extracting_insights_from_filters_and_feature_maps/blob/master/Baseline_CNN_with_leaf_dataset.ipynb)
- 50 iterations, 1 batch  
Train accuracy : 97.60%  
Val accuracy : 96.63%  

#### 2. Baseline CNN with **(128, 128)** target size | [Code](https://github.com/OH-Seoyoung/Extracting_insights_from_filters_and_feature_maps/blob/master/Baseline_CNN_with_complicated_leaf_dataset.ipynb)
- **30** iterations, 1 batch  
Train accuracy : 98.40%  
Val accuracy : 97.19%  

## Visualization  
### 0. Test sample - leaf infected with mosaic virus
<img src="https://github.com/OH-Seoyoung/Extracting_insights_from_filters_and_feature_maps/blob/master/sick_sample.jpg" width="20%">

### 1. Filters  
- First Conv2D kernel size is (5,5) and second, third are (3,3)  
<div align="center">  
<img src="https://github.com/OH-Seoyoung/Extracting_insights_from_filters_and_feature_maps/blob/master/figure/Conv1.jpg" width="25%">  
<img src="https://github.com/OH-Seoyoung/Extracting_insights_from_filters_and_feature_maps/blob/master/figure/Conv2.jpg" width="25%"> 
<img src="https://github.com/OH-Seoyoung/Extracting_insights_from_filters_and_feature_maps/blob/master/figure/Conv3.jpg" width="25%"> <br>
</div>  

### 2. Feature maps
- 3 feature maps with test sample (mosaic virus)  
<div align="center">  
<img src="https://github.com/OH-Seoyoung/Extracting_insights_from_filters_and_feature_maps/blob/master/figure/Featuremap1.jpg" width="45%">  
<img src="https://github.com/OH-Seoyoung/Extracting_insights_from_filters_and_feature_maps/blob/master/figure/Featuremap2.jpg" width="45%"> <br>
<img src="https://github.com/OH-Seoyoung/Extracting_insights_from_filters_and_feature_maps/blob/master/figure/Featuremap3.jpg" width="45%"> <br>
</div>  

