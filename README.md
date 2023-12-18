# DeepSpark开源社区

在万物皆算的时代，各领域应用层出不穷，算力必须支撑实际应用，通用性和未来可扩展性是评估算力的重要指标。天数智芯作为国内头部通用GPU高端芯片及超级算力系统提供商，截止2023年6月，已成功支持200+ AI算法模型，覆盖训练和推理，与400+家客户和生态伙伴建立合作，共同促进国内通用算力的发展，产品服务于智慧城市、数字个人、医疗、教育、通信、能源等多个领域。

天数智芯本着“平台共建、生态共享、产业共赢”的原则，致力于和行业伙伴一起打造[DeepSpark开源社区](https://www.deepspark.org.cn/)，以来自开源回馈开源的方式，汇聚社区力量，助力客户加速应用落地和收获算力赋能，促进产业生态的完善和发展。

DeepSpark开源社区目前主要致力于[百大应用开放平台](#百大应用开放平台)的打造和推广。除此之外DeepSpark社区于2023年3月开源上线了适用于国产通用GPU[天垓100](https://www.iluvatar.com/productDetails?fullCode=cpjs-yj-xlxl-tg100)的CUDA应用程序调试工具[ixGDB](https://gitee.com/deep-spark/ixgdb)。将来会有更多相关的项目和成果通过DeepSpark社区开源。

2023年8月，DeepSpark开源社区与[上海白玉兰开源开放研究院](http://baiyulan.org.cn/)签署了战略合作协议，旨在进一步促进人工智能开源事业共建共享，推动产业生态的完善和发展。2023年11月，DeepSpark社区与[启智社区](https://openi.pcl.ac.cn/)开展合作，社区用户可通过启智云脑提供的[天垓100算力](https://openi.pcl.ac.cn/iluvatar/TianGai100)训练来自DeepSparkHub的模型。

欢迎行业合作伙伴、社区用户和开发者以任何形式为DeepSpark开源社区作贡献，期待您的积极参与。


--------

# 百大应用开放平台

百大应用开放平台作为国内领先的AI和通用计算应用开发及评测平台，甄选上百个与行业应用深度耦合的开源算法和模型，支持主流生态应用框架，并针对行业需求构建多维度评测体系，广泛支持各类落地场景。


## 组成部分

### 应用算法和模型

百大应用开放平台甄选上百个[应用算法和模型](https://gitee.com/deep-spark/deepsparkhub)，覆盖AI和通用计算各领域，支持主流市场智能计算场景，包括智慧城市、数字个人、医疗、教育、通信、能源等多个领域。


### 应用框架

百大应用开放平台支持国内外主流应用框架和工具箱。

<table border="0">
    <tr align="center">
        <td><a href="https://github.com/pytorch"><img src="resources/pytorch.png" height="25"/></td>
        <td><a href="https://github.com/tensorflow"><img src="resources/tensorflow.png" height="25"/></td>
    </tr>
    <tr align="center">
        <td><a href="https://github.com/paddlepaddle"><img src="resources/paddlepaddle.png" height="40"/></td>
        <td><a href="https://gitee.com/mindspore"><img src="resources/mindspore.png" height="35"/></td>
    </tr>
    <tr align="center">
        <td><a href="https://github.com/facebookresearch/fairseq"><img src="resources/fairseq.png" height="50"/></td>
        <td><a href="https://github.com/open-mmlab/mmdetection"><img src="resources/mmdetection.png" height="50"/></td>
    </tr>
    <tr align="center">
        <td><a href="https://github.com/wenet-e2e/wenet"><img src="resources/wenet.png" height="50"/></td>
        <td><a href="https://github.com/deepmodeling"><img src="resources/deepmodeling.png" height="50"/></td>
    </tr>
    <tr align="center">
        <td><a href="https://github.com/hpcaitech/ColossalAI"><img src="resources/colossal-ai.png" height="25"/></td>
        <td><a href="https://github.com/microsoft/DeepSpeed"><img src="resources/deepspeed.png" height="45"/></td>
    </tr>
</table>


### 评测体系

评测标准广泛适用于硬件平台，体系完备，部署简单。

- 提供 :six: 维度

| 维度 | 说明 | 数据来源 | 计算方法
| --- | --- | --- | --- |
| 速度<br/>:rocket:  | 模型稳定训练时每秒处理的单位样本的算力 | DeepSpark模型训练脚本输出 | 指定迭代轮次5次去掉最高最低，取中间3次的mean中值
| 准确性<br/>:dart: | 模型收敛的精度值 | DeepSpark模型训练脚本输出 | 记录模型收敛时的精度值
| 线性度<br/>:chart_with_upwards_trend: | 模型集群规模化训练算力的线性扩展性能 <br/>包括卡线性度和节点线性度 | DeepSpark模型训练脚本输出 | 用多卡/多节点的训练速度除以卡数/节点数，再对比使用单张/单节点的训练速度
| 功耗<br/>:electric_plug: | 模型稳定训练时候实际消耗的GPU平均功耗 | GPU实时状态检测工具 | 取多次的功耗数据的平均值
| 显存占用<br/>:bar_chart: | 模型稳定训练时实际消耗的GPU平均显存占用量 | GPU实时状态检测工具 | 取多次的显存占用量的平均值
| 稳定度<br/>:wrench: | 多次完整训练（均达到收敛值）的收敛值的稳定程度 | DeepSpark模型训练脚本输出 | 采用5次达到标准收敛值的完整训练，取收敛值的中值做为基准值，其它值对比基准值的差值百分比有1次不在（-0.01，+0.01）范围内，稳定度则递减20%

   参考信息：[硬件评测结果](#硬件评测结果)

- 支持 :one: 键式部署

   全自动 :white_check_mark: 、数据可复现 :repeat: 、场景可寻源 :mag_right:

- :zero: 平台依赖

   不限制框架、不限制源语、不限制硬件
   
--------

## 硬件评测方法和结果

### 天垓100通用GPU

评测方法详见 [天垓100六维度评测方法](evaluation/Iluvatar/six_dimension_howto.md)。

评测结果如下：

| 任务         | 模型       | 收敛指标         | 配置(x-\>gpus)        | 速度   | 准确度 | 功耗（W） | 线性度 | 显存占用（G） | 稳定度 |
|--------------|------------|------------------|-----------------------|--------|--------|-----------|--------|-----------|--------|
| 自然语言处理 | BERT-large | 0.72             | sdk2.2,bs:32,8x,amp   | 214    | 0.72   | 152\*8    | 0.96   | 20.3\*8   | 1      |
| 推荐系统     | DLRM       | AUC:0.75         | sdk2.2,bs:2048,8x,amp | 793486 | 0.75   | 60\*8     | 0.97   | 3.7\*8    | 1      |
| 图像分类     | ResNet50   | top1 75.9%       | sdk2.2,bs:512,8x,amp  | 5221   | 76.43% | 128\*8    | 0.97   | 29.1\*8   | 1      |
| 图像分割     | 3D U-Net   | 0.908            | sdk2.2,bs:4,8x,fp32   | 12     | 0.908  | 152\*8    | 0.85   | 19.6\*8   | 1      |
| 目标检测     | YOLOv5     | mAP:0.5          | sdk2.2,bs:128,8x,amp  | 1228   | 0.56   | 140\*8    | 0.92   | 27.3\*8   | 1      |
| 文本检测     | SATRN      | 0.841            | sdk2.2,bs:128,8x,fp32 | 630    | 88.4   | 166\*8    | 0.98   | 28.5\*8   | 1      |
| 语音识别     | Conformer  | 3.72             | sdk2.2,bs:32,8x,fp32  | 380    | 4.79   | 113\*8    | 0.82   | 21.5\*8   | 1      |
| 3D重建       | ngp-nerf   | 0.0046           | sdk2.2,bs:1,8x,amp    | 10     | 19.6   | 82\*8     | 0.90   | 28.1\*8   | 1      |
| 目标追踪     | FairMOT    | MOTA:69.8        | sdk2.2,bs:64,8x,fp32  | 52     | 69.8   | 132\*8    | 0.97   | 19.1\*8   | 1      |
| 大模型       | CPM        | 0.91             | sdk2.2,bs:128,8x,amp  | 357    | 0.91   | 156\*8    | 0.93   | 20.6\*8   | 1      |
| 语音语义     | Tacotron2  | score(MOS):4.460 | sdk2.2,bs:128,8x,amp  | 77     | 4.46   | 128\*8    | 0.96   | 18.4\*8   | 1      |
| 新兴模型     | Wave-MLP   | 80.1             | sdk2.2,bs:256,8x,fp32 | 1026   | 83.1   | 198\*8    | 0.98   | 29.4\*8   | 1      |


各维度说明，请见[评测体系](#评测体系)。


-------

# 社区

## 治理

请参见 [Code of Conduct](CODE_OF_CONDUCT.md)。

## 交流

请联系 contact@deepspark.org.cn。

## 贡献

请参见各项目的Contributing Guidelines。

# 许可证

[Apache License 2.0](LICENSE)。

