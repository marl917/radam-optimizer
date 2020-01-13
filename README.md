# Study of RAdam based on the paper "On the Variance of the Adaptive Learning Rate and Beyond" by Liu et Al. (2019a)

```
@article{liu2019radam,
  title={On the Variance of the Adaptive Learning Rate and Beyond},
  author={Liu, Liyuan and Jiang, Haoming and He, Pengcheng and Chen, Weizhu and Liu, Xiaodong and Gao, Jianfeng and Han, Jiawei},
  journal={arXiv preprint arXiv:1908.03265},
  year={2019}
}
```
I also used the code from the paper "On the adequacy of untuned warmup for adaptive optimization",  	arXiv:1910.04209, 2019, Jerry Ma and Denis Yarats, in which Adam with warmup was implemented.


In this project, I compare the performance of RAdam with Adam and Adam with warmup using the Fashion MNIST dataset. More precisely, the code evaluates the robustness of these optimization algorithms to variations of the learning rate. My report 
delves deeper in the theory and the implementation.

## Prerequisites

Here is the list of libraries on Python 3.6 needed: torch 1.3.1, torchvision 0.4.2, pytorch-warmup 0.0.4, tensorflow 2.0.0, tensorboard 2.0.2


## Results

Below are the performance obtained after training these 3 optimizers with different values for learning rate : 


Radam Train Loss             |  Radam Test Accuracy 
:---------------------:|:-------------------------:
![](https://github.com/marl917/radam-optimizer/blob/master/images/Loss_Radam_lr_r.png) |  ![](https://github.com/marl917/radam-optimizer/blob/master/images/Accuracy_Radam_lr_r.png)


Adam Train Loss             |  Adam Test Accuracy 
:---------------------:|:-------------------------:
![](https://github.com/marl917/radam-optimizer/blob/master/images/Loss_Adam_lr_r.png) |  ![](https://github.com/marl917/radam-optimizer/blob/master/images/Accuracy_Adam_lr_r.png)


Adam with warmup Train Loss            |  Adam with warmup Test Accuracy 
:---------------------:|:-------------------------:
![](https://github.com/marl917/radam-optimizer/blob/master/images/Loss_AdamW_r.png) |  ![](https://github.com/marl917/radam-optimizer/blob/master/images/Accuracy_AdamW_r.png)

![](https://github.com/marl917/radam-optimizer/blob/master/images/barres_lr.png)






