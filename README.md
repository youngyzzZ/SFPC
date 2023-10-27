# SFPC
[BIBM 2023] Semi-supervised Medical Image Segmentation via Feature-perturbed Consistency

This codebase contains the official PyTorch implementation of our SFPC in the field of semi-supervised semantic segmentation in the **[2017 ACDC](https://humanheart-project.creatis.insa-lyon.fr/database/#) and the [BraTS](https://www.med.upenn.edu/cbica/brats2020/data.html) datasets.**

# Results
Quantitative comparisons with other state-of-the-art methods on **BraTS2020** and **2017 ACDC**  datasets. ↑ indicates that larger values are better and ↓ indicates that smaller values are better.

| Method                      | scans used|           |           |BraTS2020 (3D)|          |           |2017 ACDC (3D)|          |          
| :-------------------------: | :-------: | :-------: | :-------: | :-----------:| :-------:|:---------:|:------------:|:--------:|
|                             | Latebled  | Unlabeled |DSC(%)↑    |  95HD(mm)↓   | ASD(mm)↓ |DSC(%)↑    |  95HD(mm)↓   | ASD(mm)  |
| SASSNet                     | 10        | 90        | 82.16     | 14.86        | 4.15     | 84.26     | 6.08         | 1.76     |
| UAMT                        |           |           | 80.88     | 17.63        | 6.86     | 81.32     | 13.17        | 3.77     |
| Tri-U-MT                    |           |           | 82.70     | 15.26        | 3.62     | 83.71     | 7.54         | 2.73     |
| DTC                         |           |           | 81.86     | 16.31        | 3.67     | 82.43     | 8.82         | 3.15     |
| CoraNet                     |           |           | 81.29     | 13.97        | 3.96     | 84.17     | 6.18         | 2.41     |
|MC-Net                       |           |           | 83.75     | 13.55        | 3.34     | 86.55     | 7.01         | 2.13     |
|PLCT                         |           |           | 83.51     | 13.74        | 3.62     | 86.48     | 6.69         | 2.32     |
|URPC                         |           |           | 84.08     | 11.56        | 3.28     | 84.72     | 5.12         | 1.64     |
| **Ours**                    |           |           | **84.83** | **10.79**    | **3.07** | **87.52** | **4.96**     | **1.33** |
| SASSNet                     | 20        | 80        | 84.67     | 9.41         | 2.64     | 86.98     | 5.36         | 2.52     |
| UAMT                        |           |           | 84.86     | 12.21        | 2.19     | 85.62     | 9.31         | 1.53     |
| Tri-U-MT                    |           |           | 85.02     | 8.83         | 3.16     | 87.04     | 5.62         | 1.63     |
| DTC                         |           |           | 84.82     | 12.69        | 3.43     | 86.13     | 6.28         | 2.31     |
| CoraNet                     |           |           | 84.37     | 9.05         | 2.62     | 86.32     | 6.45         | 2.21     |
|MC-Net                       |           |           | 85.17     | 9.72         | 3.01     | 88.35     | 5.76         | 1.92     |
|PLCT                         |           |           | 85.38     | 8.72         | 2.94     | 88.26     | 5.84         | 2.11     |
|URPC                         |           |           | 85.61     | 8.91         | 2.55     | 87.18     | 5.29         | 1.61     |
| **Ours**                    |           |           | **86.35** | **8.64**     | **2.37** | **89.13** | **5.09**     | **1.48** |
|nn-UNet                      | 100       | 0         | 89.29     | 7.97         | 1.83     | 92.12     | 1.73         | 0.52     |
