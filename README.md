# AEMatter

Repository for the paper Rethinking Context Aggregation in Natural Image Matting

## Requirements
#### Hardware:

GPU memory >= 10GB for inference on the Adobe Composition-1K testing set.

#### Packages:

- torch >= 1.10
- numpy >= 1.16
- opencv-python >= 4.0
- einops >= 0.3.2
- timm >= 0.4.12

## Models
Quantitative results on Adobe Composition-1K
| Model Name  |   Size   | MSE | SAD | Grad | Conn |
| :------------: |:-----------:| :----:|:---:|:---:|:---:|
| [AEMatter] | 195MiB | 2.26 | 17.53 | 4.76 | 12.46 |
| [AEMatter+TTA] | 195MiB | 2.06 | 16.89 | 4.24 | 11.72 |
| [AEMatter (RWA)] | 195MiB | - | - | - | - |

Quantitative results on Transparent-460
| Model Name  |   Size   | MSE | SAD | Grad | Conn |
| :------------: |:-----------:| :----:|:---:|:---:|:---:|
| AEMatter | 195MiB |6.92|122.27|27.42|112.02 |

Quantitative results on AIM-500
| Model Name  |   Size   | MSE | SAD | Grad | Conn |
| :------------: |:-----------:| :----:|:---:|:---:|:---:|
| AEMatter | 195MiB | 11.69 | 14.76 | 11.20 | 14.20 | 

## Evaluation
We provide the script `eval.py`  for evaluation.


