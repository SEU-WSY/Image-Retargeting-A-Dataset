# Image-Retargeting-A-Dataset-and-Metrics：RetarSet
We construct a novel dataset(RetarSet) that not only encompasses a wide range of input/output ratios, object counts, and layouts but also includes annotations on object distributions post-retargeting. <br> 
![](https://github.com/wwwwwwwsy/Image-Retargeting-A-Dataset-and-Metrics/blob/main/example.png)  <br>  
# Mask Annotation
After reformulating the annotation of image retargeting as a foreground re-layout task, we establish the following criteria for foreground objects before and after retargeting: 1) Preserve the complete and unaltered appearance of salient objects. 2) Maintain consistent inter-instance relationships and overall global layout.<br>  
To this end, we propose a novel annotation method based on the give salient object masks and ranking labels in the source datasets to determine the new distribution of foreground instances after retargeting. The detailed process is illustrated in Figure below and it contains three steps. <br> 
![](https://github.com/wwwwwwwsy/Image-Retargeting-A-Dataset-and-Metrics/blob/main/flowChart.png)  <br>  
### Step 1:Bounding. 
We first extract the foreground instances. A minimum bounding square is then placed around each salient mask to facilitate locating each instance’s center.<br> 
### Step 2:Translating and trimming. 
We design a Translate module(shown in Figure right) to maintain the completeness of salient instance masks.<br>
### Step 3:Final Adjustment and Expansion. 
During transformations, if any salient objects become cropped or partially obscured, we apply corrective measures to maintain their visibility.<br>
# Instance number
First, in terms of the number of instances, our dataset far exceeds RetargetMe in the number of instances, for example, the number of three-instance images is 15 times that of RetargetMe , indicating that this dataset can provide richer data for difficult tasks.<br>  
<img src="https://github.com/wwwwwwwsy/Image-Retargeting-A-Dataset-and-Metrics/blob/main/instance_number.png" width="500" />
  <br>  
# Aspect ratio
Second, in terms of aspect ratio distribution, our dataset covers a wider range of ratios, e.g., the number of 4:3 aspect ratio images is 18 times that of RetargetMe, and it is significantly larger in multiple aspect ratios, ensuring the balance and applicability of the data. <br>  
<img src="https://github.com/wwwwwwwsy/Image-Retargeting-A-Dataset-and-Metrics/blob/main/aspect_ratio.png" width="500" /> <br>  
# Download the data
To access our full dataset, please fill in the [form](https://github.com/wwwwwwwsy/Image-Retargeting-A-Dataset-and-Metrics/blob/main/application.xlsx) and send this form to this email(haochen303@seu.edu.cn).<br>
