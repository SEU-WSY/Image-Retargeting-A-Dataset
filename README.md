# Image-Retargeting-A-Dataset-and-Metrics：RetarSet
We construct a novel dataset(RetarSet) that not only encompasses a wide range of input/output ratios, object counts, and layouts but also includes annotations on object distributions post-retargeting. <br> 
![](https://github.com/wwwwwwwsy/Image-Retargeting-A-Dataset-and-Metrics/blob/main/example.png)  <br>  
# Mask Annotation of RetarSet
The labels are the new spatial layout of foreground instances after retargeting. The annotation process contains three steps. <br> 
### Step 1:Bounding. 
We first extract the foreground instances. A minimum bounding square is then placed around each salient mask to facilitate locating each instance’s center.<br> 
### Step 2:Translating and trimming. 
We design a Translate module(shown in Figure right) to maintain the completeness of salient instance masks.<br>
### Step 3:Final Adjustment and Expansion. 
During transformations, if any salient objects become cropped or partially obscured, we apply corrective measures to maintain their visibility.<br>
## Instance Number
First, in terms of the number of instances, our dataset far exceeds RetargetMe. For example, the number of three-instance images is **15 times** that of RetargetMe, indicating that this dataset can provide richer data for challenging tasks.

|          | 1   | 2    | 3    | 4    | 5    | 6  | 7  | 8  |
|----------|----:|-----:|-----:|-----:|-----:|---:|---:|---:|
| RetarSet | 114 | 262  | 180  | 130  | 301  |  8 |  3 |  2 |

---

## Aspect Ratio Distribution
Second, our dataset covers a wider range of aspect ratios. For example, the number of `4:3` images is **18 times** that of RetargetMe, with significant improvements across multiple ratios, ensuring better data balance and applicability.

|          | 4:3  | 2:1 | 5:4 | 5:3 | 1:1 | 4:5 | 3:5 |
|----------|-----:|----:|----:|----:|----:|----:|----:|
| RetarSet | 754  |  28 |  32 |  44 |  17 |  47 |  78 |

---

## Download the Data
To access the full dataset:  
1. Fill out the [application form](https://github.com/wwwwwwwsy/Image-Retargeting-A-Dataset-and-Metrics/blob/main/application.xlsx).  
2. Send the completed form to [cious449@gmail.com](mailto:cious449@gmail.com).  

**Citation Request**  
If you use our database, please cite our paper:  
```bibtex
@misc{dataset2025,
    author = {wwwwwwwsy},
    title  = {Image Retargeting: A Dataset and Metrics},
    year   = {2025},
    howpublished = {\url{https://github.com/wwwwwwwsy/Image-Retargeting-A-Dataset-and-Metrics}},
    note   = {Accessed: YYYY-MM-DD}  % Optional: Add access date
}
