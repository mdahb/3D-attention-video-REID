# 3D-Attention-Video-Person-ReID



### Introduction
This repository contains PyTorch implementations of temporal modeling methods for video-based person reID. It is forked from [deep-person-reid](https://github.com/KaiyangZhou/deep-person-reid).. Based on that, I implement (1) video sampling strategy for training and testing, (2) temporal modeling methods including temporal pooling, temporal attention, RNN and 3D conv. The base loss function and basic training framework remain the same as [deep-person-reid](https://github.com/KaiyangZhou/deep-person-reid). **PyTorch 1.2.0, Torchvision 0.4.0 and Python 3.7** is used.

### Dataset
All experiments are done on MARS, as it is the largest dataset available to date for video-based person reID. Please follow [deep-person-reid](https://github.com/KaiyangZhou/deep-person-reid) to prepare the data. The instructions are copied here: 

1. Create a directory named `mars/` under `data/`.
2. Download dataset to `data/mars/` from http://www.liangzheng.com.cn/Project/project_mars.html.
3. Extract `bbox_train.zip` and `bbox_test.zip`.
4. Download split information from https://github.com/liangzheng06/MARS-evaluation/tree/master/info and put `info/` in `data/mars` (we want to follow the standard split in [8]). The data structure would look like:
```
mars/
    bbox_test/
    bbox_train/
    info/
```
5. Use `-d mars` when running the training code.

### Usage
To test the model, please run

   test.sh


For trained model, please download the model in the following google drive [3D-attention-PyTorch](https://drive.google.com/drive/folders/1IFj17LP1q9ddkHEtRkaLgDK99q7dRd09?usp=sharing).

