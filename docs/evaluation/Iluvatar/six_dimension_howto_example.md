# 天垓100六维度评测方法示例：ResNet50

使用天数智芯天垓100（BI-V100）通用GPU硬件并安装天数智芯软件栈和深度学习框架后，您可运行DeepSpark模型训练脚本，并借助于天数智芯GPU实时状态检测工具ixSMI得到天垓100硬件的六维度数据。DeepSpark六维度指标的定义请参照[评测体系](../../README.md#评测体系)。天垓100六维度具体计算方法请参照[天垓100（BI-V100）六维度评测方法](six_dimension_howto.md)。

本示例以[ResNet50模型](https://gitee.com/deep-spark/deepsparkhub/tree/master/cv/classification/resnet50/pytorch)为例，用8张天垓100（BI-V100）卡执行`amp_8card.sh`脚本进行混合精度训练。在本示例环境中，数据集所在路径为`/home/datasets/imagenet`。

具体运行和六维度的计算过程如下：

## 速度

执行DeepSpark模型训练脚本，脚本会打印训练过程中每个epoch的每秒处理的单位样本数量，例如：

```
$ bash amp_8card.sh --data-path /home/datasets/imagenet
...
Creating data loaders
read 1281167 files from 1000 directories
...
Creating model resnet50
Start training
Epoch: [0]  [  0/334]  eta: 0:38:25  lr: 0.128  img/s: 590.7051616388846  loss: 7.1621 (7.1621)  acc1: 0.0000 (0.0000)  acc5: 0.0000 (0.0000)  time: 6.9017  data: 0.0000
Epoch: [0]  [ 10/334]  eta: 0:06:47  lr: 0.128  img/s: 5625.496142412713  loss: 7.2926 (7.2497)  acc1: 0.0000 (0.1326)  acc5: 0.6250 (0.8144)  time: 1.2591  data: 0.0019
Epoch: [0]  [ 20/334]  eta: 0:05:09  lr: 0.128  img/s: 5597.293247401811  loss: 7.4071 (7.4806)  acc1: 0.0000 (0.0794)  acc5: 0.6250 (0.7639)  time: 0.6908  data: 0.0020
Epoch: [0]  [ 30/334]  eta: 0:04:30  lr: 0.128  img/s: 5445.774084325316  loss: 7.3483 (7.4083)  acc1: 0.0000 (0.1075)  acc5: 0.6250 (0.7258)  time: 0.6889  data: 0.0018
...
Epoch: [0]  [320/334]  eta: 0:00:11  lr: 0.128  img/s: 5411.016050829418  loss: 6.8285 (6.9574)  acc1: 0.2083 (0.1694)  acc5: 1.2500 (0.7976)  time: 0.8184  data: 0.0023
Epoch: [0]  [330/334]  eta: 0:00:03  lr: 0.128  img/s: 5601.840934156804  loss: 6.8106 (6.9527)  acc1: 0.4167 (0.1788)  acc5: 1.6667 (0.8283)  time: 0.7644  data: 0.0023
Epoch: [0] Total time: 0:04:38
Data loading of epoch 0: 0:00:00.759193
Epoch: [0] Avg img/s: 5060.21643823427
Test:  [ 0/14]  eta: 0:00:03  loss: 6.9883 (6.9883)  acc1: 0.0000 (0.0000)  acc5: 0.0000 (0.0000)  time: 0.2724  data: 0.0000
Test: Total time: 0:00:04
 * Acc@1 0.112 Acc@5 1.040
Epoch time 0:04:43
...
Epoch: [6] Total time: 0:04:38
Data loading of epoch 6: 0:00:00.797741
Epoch: [6] Avg img/s: 4910.795658460139
Test:  [ 0/14]  eta: 0:00:04  loss: 5.5391 (5.5391)  acc1: 8.1250 (8.1250)  acc5: 24.1667 (24.1667)  time: 0.2859  data: 0.0019
Test: Total time: 0:00:03
 * Acc@1 13.360 Acc@5 30.960
Epoch time 0:04:43
...
Epoch: [7] Total time: 0:04:36
Data loading of epoch 7: 0:00:00.770986
Epoch: [7] Avg img/s: 4980.222383258538
Test:  [ 0/14]  eta: 0:00:03  loss: 5.4844 (5.4844)  acc1: 8.1250 (8.1250)  acc5: 23.9583 (23.9583)  time: 0.2801  data: 0.0017
Test: Total time: 0:00:03
 * Acc@1 24.928 Acc@5 49.712
Epoch time 0:04:41
...
Epoch: [8] Total time: 0:04:31
Data loading of epoch 8: 0:00:00.756521
Epoch: [8] Avg img/s: 5032.905842259754
Test:  [ 0/14]  eta: 0:00:04  loss: 4.1641 (4.1641)  acc1: 29.1667 (29.1667)  acc5: 54.5833 (54.5833)  time: 0.2861  data: 0.0019
Test: Total time: 0:00:03
 * Acc@1 23.536 Acc@5 47.024
Epoch time 0:04:35
...
Epoch: [9] Total time: 0:04:39
Data loading of epoch 9: 0:00:00.761111
Epoch: [9] Avg img/s: 4925.753353494863
Test:  [ 0/14]  eta: 0:00:04  loss: 3.3516 (3.3516)  acc1: 45.4167 (45.4167)  acc5: 70.4167 (70.4167)  time: 0.3107  data: 0.0022
Test: Total time: 0:00:03
 * Acc@1 28.480 Acc@5 59.568
Epoch time 0:04:44
...
Epoch: [10] Total time: 0:04:42
Data loading of epoch 10: 0:00:00.776602
Epoch: [10] Avg img/s: 4845.4628560647725
Test:  [ 0/14]  eta: 0:00:04  loss: 3.7891 (3.7891)  acc1: 27.0833 (27.0833)  acc5: 56.4583 (56.4583)  time: 0.3491  data: 0.0028
Test: Total time: 0:00:03
 * Acc@1 33.520 Acc@5 61.264
Epoch time 0:04:47
...
Epoch: [63] Total time: 0:04:36
Data loading of epoch 63: 0:00:00.688607
Epoch: [63] Avg img/s: 4928.513448918747
Test:  [ 0/14]  eta: 0:00:03  loss: 2.3945 (2.3945)  acc1: 63.5417 (63.5417)  acc5: 85.6250 (85.6250)  time: 0.2850  data: 0.0017
Test: Total time: 0:00:03
 * Acc@1 69.104 Acc@5 89.088
Epoch time 0:04:40
...
Epoch: [64] Total time: 0:04:47
Data loading of epoch 64: 0:00:00.674387
Epoch: [64] Avg img/s: 4812.667878767461
Test:  [ 0/14]  eta: 0:00:04  loss: 1.7793 (1.7793)  acc1: 81.8750 (81.8750)  acc5: 94.7917 (94.7917)  time: 0.3257  data: 0.0019
Test: Total time: 0:00:03
 * Acc@1 77.360 Acc@5 93.120
 ...
Epoch time 0:04:52
The accuracy has been exceeded 75.9,and the training is terminated at epoch 64
Training time 5:06:03
...
```

取稳定训练的第6到第10个epoch共5个epoch：

- Epoch: [6] Avg img/s: 4910.795658460139
- Epoch: [7] Avg img/s: 4980.222383258538
- Epoch: [8] Avg img/s: 5032.905842259754
- Epoch: [9] Avg img/s: 4925.753353494863
- Epoch: [10] Avg img/s: 4845.4628560647725

最高是第8个、最低是第10个epoch，计算速度则取第6个、第7个和第9个epoch的值相加除以3，即为：

(4910+4980+4925)/3=4938.33 img/s

注：在该模型用例中，通过以上方法获取的速度，主要评估的是训练集上training的速度，而端到端(end-to-end)训练速度则包含了训练集和验证集在整个training和evaluation的全部过程中的总体速度。

训练端到端的速度计算方式为：（每个epoch的处理的样本数量*完整训练的epoch数量）/总的训练时长

1. 通过“read 1281167 files from 1000 directories”的提示得到每个epoch的处理的样本数量为1281167个。

2. 通过“Training time 5:06:03”的提示得到总的训练时长为5:06:03小时，换算成18363秒。

3. 本次`amp_8card.sh`完整训练的端到端速度为：(1281167*64)/18363=4465.2 img/s


## 准确性

执行DeepSpark模型训练脚本，脚本会打印训练过程中每个epoch的训练准确度，例如：

```
$ bash amp_8card.sh --data-path /home/datasets/imagenet
...
Epoch: [0] Total time: 0:04:38
Data loading of epoch 0: 0:00:00.759193
Epoch: [0] Avg img/s: 5060.21643823427
Test:  [ 0/14]  eta: 0:00:03  loss: 6.9883 (6.9883)  acc1: 0.0000 (0.0000)  acc5: 0.0000 (0.0000)  time: 0.2724  data: 0.0000
Test: Total time: 0:00:04
 * Acc@1 0.112 Acc@5 1.040
...
Epoch: [64] Avg img/s: 4812.667878767461
Test:  [ 0/14]  eta: 0:00:04  loss: 1.7793 (1.7793)  acc1: 81.8750 (81.8750)  acc5: 94.7917 (94.7917)  time: 0.3257  data: 0.0019
Test: Total time: 0:00:03
 * Acc@1 77.360 Acc@5 93.120
...
The accuracy has been exceeded 75.9,and the training is terminated at epoch 64
...
```

ResNet50模型收敛的标准是top1 75.9%，在第64个epoch时达到了Acc@1 77.360（百分比），超过了75.9（百分比）的阈值。所以训练的精度值为77.36%。


## 线性度

执行DeepSpark模型训练脚本，脚本会打印训练过程中每个epoch的速度，训练可以使用单卡和多卡进行，或使用单节点和多节点进行，分别可以计算出卡线性度和节点线性度。

以计算卡线性度为例：

例如，在一台服务器上使用8张天垓100加速卡训练的速度是2575 img/s：

```
$ bash fp32_8card.sh --data-path /home/datasets/imagenet
...
Epoch: [0] Total time: 0:08:37
Data loading of epoch 0: 0:00:00.745164
Epoch: [0] Avg img/s: 2575.527288024902
Test:  [ 0/21]  eta: 0:00:06  loss: 6.1528 (6.1528)  acc1: 4.3333 (4.3333)  acc5: 24.0000 (24.0000)  time: 0.3201  data: 0.0000
Test: Total time: 0:00:07
 * Acc@1 0.704 Acc@5 3.968
Epoch time 0:08:45
...
```

将2575 img/s除以多卡的卡数（即8），得到：

2575/8=321.9 img/s

再对比使用1张天垓100加速卡训练时的速度，如下所示，速度为335 img/s。

```
$ bash fp32_1card.sh --data-path /home/datasets/imagenet
...
Epoch: [0] Avg img/s: 335.40682470945455
Test:  [  0/179]  eta: 0:00:53  loss: 3.6599 (3.6599)  acc1: 36.4286 (36.4286)  acc5: 70.3571 (70.3571)  time: 0.2962  data: 0.0000
Test:  [100/179]  eta: 0:00:23  loss: 5.3622 (5.0095)  acc1: 6.4286 (12.0226)  acc5: 22.1429 (31.2907)  time: 0.2973  data: 0.0011
Test: Total time: 0:00:53
 * Acc@1 11.786 Acc@5 30.074
Epoch time 1:04:59
...
```

得到卡线性度 321.9/335=96%

## 功耗

在模型稳定训练时，使用GPU实时状态检测工具ixSMI查询实际消耗的GPU功耗并取平均值。

以运行`fp32_8card.sh`脚本使用8张天垓100加速卡训练为例，输入以下命令查询index为0的GPU的状态：

```
$ ixsmi -q -i 0 -l | grep -E 'Power Draw'
        Power Draw                              : 161 W
        Power Draw                              : 169 W
        Power Draw                              : 161 W
        Power Draw                              : 174 W
        Power Draw                              : 163 W
...
```

取多次的数据取平均值作为模型训练的功耗，例如：

平均功耗 (161+169+161+174+163)/5=165.6 W

## 显存占用

在模型稳定训练时，使用GPU实时状态检测工具ixSMI查询GPU显存占用量并取平均值。

以运行`amp_8card.sh`脚本使用8张天垓100加速卡训练为例，输入以下命令查询index为0的GPU的状态：

```
$ ixsmi -q -i 0 -l | grep Used.[^G]
   Used                                    : 30671  MiB
   Used                                    : 30670  MiB
   Used                                    : 30671  MiB
   Used                                    : 30671  MiB
   Used                                    : 30670  MiB
```

去平均值得到平均显存占用量为 (30671+30670+30671+30671+30670)/5=30670.6 MiB

## 稳定度

执行DeepSpark模型训练脚本，脚本会打印完整训练最终所达到的收敛值，例如：

```
$ bash amp_8card.sh --data-path /home/datasets/imagenet
...
Epoch: [0] Total time: 0:04:38
Data loading of epoch 0: 0:00:00.759193
Epoch: [0] Avg img/s: 5060.21643823427
Test:  [ 0/14]  eta: 0:00:03  loss: 6.9883 (6.9883)  acc1: 0.0000 (0.0000)  acc5: 0.0000 (0.0000)  time: 0.2724  data: 0.0000
Test: Total time: 0:00:04
 * Acc@1 0.112 Acc@5 1.040
...
Epoch: [64] Avg img/s: 4812.667878767461
Test:  [ 0/14]  eta: 0:00:04  loss: 1.7793 (1.7793)  acc1: 81.8750 (81.8750)  acc5: 94.7917 (94.7917)  time: 0.3257  data: 0.0019
Test: Total time: 0:00:03
 * Acc@1 77.360 Acc@5 93.120
...
The accuracy has been exceeded 75.9,and the training is terminated at epoch 64
...
```

可以得到本次的收敛精度为Acc@1 77.360，记为第1次。

再进行4次模型完整训练，每次都最终达到标准收敛值，即达到`The accuracy has been exceeded 75.9`，，Acc@1分别得到如下结果：

- 第2次：76.816
- 第3次：77.116
- 第4次：76.960
- 第5次：77.010

取5次的收敛值的中值做为基准值，即以第5次的收敛精度77.010作为基准，然后其它的4次收敛值对比基准值的差值百分比计算如下：

- 第1次：(77.360-77.010)/77.010=0.0045
- 第2次：(76.816-77.010)/77.010=-0.0025
- 第3次：(77.116-77.010)/77.010=0.0013
- 第4次：(76.960-77.010)/77.010=-0.0006

可以得到差值百分比都分布在（-0.01，+0.01）的合理区间，此时达到满分1。（当5个数据有1次不在该范围内，稳定度则递减20%。）
