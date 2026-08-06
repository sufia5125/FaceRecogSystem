# Forensic Sketch-to-Photo Face Recognition

Comparative analysis of deep learning architectures VGG-16 and ResNet-50 for cross-modal forensic sketch-to-photo face recognition using batch-hard triplet loss.
## Requirements

Python 3.10 with the following packages:
* torch==2.0.1
* torchvision==0.15.2
* numpy==1.24.3
* Pillow==9.5.0
* scikit-learn
* matplotlib

## Output
<img width="2738" height="1133" alt="query_result" src="https://github.com/sufia5125/FaceRecogSystem/blob/fe7747d8852b891a218b0421abaadbac6ca1e948/query_result.png" />

## Results

Evaluated on 402 held-out test pairs from FS2K with an 80/20 train/test split.

| Metric | ResNet-50 | VGG-16 |
|---|---|---|
| Rank-1 | 27.86% | 53.73% |
| Rank-5 | 57.21% | 81.59% |
| Rank-10 | 70.40% | 89.30% |
| ROC AUC | 0.9628 | 0.9866 |
| TAR@FAR=1% | 43.28% | 73.13% |

