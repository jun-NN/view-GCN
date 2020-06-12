# Pytorch code for view-GCN.

Xin Wei, Ruixuan Yu and Jian Sun. **View-GCN: View-based Graph Convolutional Network for 3D Shape Analysis**. CVPR, accepted, 2020. [[pdf]](http://gr.xjtu.edu.cn/c/document_library/get_file?folderId=1401787&name=DLFE-129432.pdf)

# Training

## Requiement

This code is tested on Python 3.6 and Pytorch 1.0 + 

## Dataset

First download the 20 views ModelNet40 dataset provided by [Kanezaki et al. 2018](https://github.com/kanezaki/pytorch-rotationnet) and put it under `data`

`$ wget https://data.airc.aist.go.jp/kanezaki.asako/data/modelnet40v2png_ori4.tar; tar xvf modelnet40v2png_ori4.tar`

[Kanezaki et al. 2018] Asako Kanezaki, Yasuyuki Matsushita and Yoshifumi Nishida. RotationNet: Joint Object Categorization and Pose Estimation Using Multiviews from Unsupervised Viewpoints. CVPR, 2018.

## Command for training:

`python train.py -name view-gcn -num_models 0 -weight_decay 0.001 -num_views 20 -cnn_name resnet18`

The code is heavily borrowed from [mvcnn_new](https://github.com/jongchyisu/mvcnn_pytorch).

Jong-Chyi Su, Matheus Gadelha, Rui Wang, and Subhransu Maji. A Deeper Look at 3D Shape Classifiers. Second Workshop on 3D Reconstruction Meets Semantics, ECCV, 2018.

# Citation
If you find our work useful in your research, please consider citing:
```@InProceedings{Wei_2020_CVPR,
author = {Wei, Xin and Yu, Ruixuan and Sun, Jian},
title = {View-GCN: View-Based Graph Convolutional Network for 3D Shape Analysis},
booktitle = {IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
month = {June},
year = {2020}
}
```


