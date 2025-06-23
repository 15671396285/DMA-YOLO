# DMA-YOLO
DMA-YOLO is an advanced training framework, aiming to solve the occlusion and multi-scale problems in dense pedestrian detection, thereby achieving higher detection accuracy.

# Quick Start
## Setup
```
conda create -n dma-yolo python=3.10.12
conda activate dma-yolo
pip install -r requirements.txt
```
## Datasets
1. Download
- crowdhuman dataset : https://www.crowdhuman.org/
- widerperson dataset : http://www.cbsr.ia.ac.cn/users/sfzhang/WiderPerson/
2. Modify paths in widerperson.yaml/crowdhuman.yaml
```
path: /yourpath/data/widerperson # dataset root dir
train: train/images 
val: val/images
test:  

# Classes
names:
  0: pedestrians
```
3. Organize Images
Structure your dataset directories as follows:
```
dataset/
├── train/
│   ├── images
│       ├── image1.jpg
│       ├── image2.jpg
│       └── ...
│   └── labels/
│       ├── label1.txt
│       └── ...
├── val/
    ├── images/
        └── ...
    └── labels/
        └── ...
├── test/
    ├── images/
        └── ...
    └── labels/
        └── ...
```
## Usage
```
python train_v8.py --cfg ultralytics/cfg/models/my_cfg/dma-yolo.yaml
```





