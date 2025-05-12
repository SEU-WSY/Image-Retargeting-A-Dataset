# Image-Retargeting-A-Dataset：RetarSet
We construct a novel dataset(RetarSet) that not only encompasses a wide range of input/output ratios, object counts, and layouts but also includes annotations on object distributions post-retargeting. <br> 
RetarSet contains 4,000 images equally distributed across four aspect ratios: 1:1, 4:3, 9:16, and 16:9 (1,000 images per ratio).<br>
![](https://github.com/wwwwwwwsy/Image-Retargeting-A-Dataset-and-Metrics/blob/main/example.png)  <br>  
# Mask Annotation of RetarSet
The labels are the new spatial layout of foreground instances after retargeting. The annotation process contains three steps. <br> 
### Step 1:Bounding. 
We first extract the foreground instances. A minimum bounding square is then placed around each salient mask to facilitate locating each instance’s center.<br> 
### Step 2:Translating and trimming. 
We design a Translate module to maintain the completeness of salient instance masks.<br>
### Step 3:Final Adjustment and Expansion. 
During transformations, if any salient objects become cropped or partially obscured, we apply corrective measures to maintain their visibility.<br>
## Instance Number
First, in terms of the number of instances, our dataset can provide richer data for challenging tasks.

|          | 1   | 2    | 3    | 4    | 5    | 6  | 7  | 8  |
|----------|----:|-----:|-----:|-----:|-----:|---:|---:|---:|
| RetarSet | 114 | 262  | 180  | 130  | 301  |  8 |  3 |  2 |

---

## Aspect Ratio Distribution
Second, our dataset covers a wider range of aspect ratios. It ensures better data balance and applicability.

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
