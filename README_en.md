<!-- markdownlint-disable first-line-h1 -->
<!-- markdownlint-disable html -->
[<img alt="English" src="https://img.shields.io/badge/Language-English-blue.svg">](README_en.md) [<img alt="Chinese" src="https://img.shields.io/badge/语言-简体中文-red.svg">](README.md)

# DeepSpark Open Source Community

<div align="center" style="line-height: 1;">
  <a href="https://www.deepspark.org.cn"><img alt="Homepage"
    src="https://img.shields.io/badge/DeepSpark-Homepage-blue.svg"/></a>
  <a href="./LICENSE"><img alt="LICENSE" src="https://img.shields.io/badge/license-Apache%202.0-dfd.svg"></a>
  <a href="https://gitee.com/deep-spark/deepspark/releases/latest"><img alt="Release" src="https://img.shields.io/github/v/release/deep-spark/deepspark?color=ffa"></a>
</div>
<br>

In the time when everything is computable, applications in various fields are emerging rapidly. Computing power must support practical applications, with versatility and future scalability being crucial metrics for evaluating computing capabilities. As a leading domestic provider of high-end GPGPU chips and supercomputing systems, the Iluvatar CoreX has successfully supported 400+ AI algorithm models by December 2024. We have established collaborations with 400+ customers and ecosystem partners to jointly promote the development of domestic general-purpose computing power. Our products serve multiple fields including smart cities, digital individuals, healthcare, education, telecommunications, and energy.

Guided by the principles of "co-building platforms, sharing ecosystems, and winning together in the industry," the Iluvatar CoreX is committed to collaborating with industry partners to establish the [DeepSpark Open Source Community](https://www.deepspark.org.cn/). By giving back to the open-source community through open-source contributions, we aim to gather community strength, help customers accelerate application deployment and benefit from computing power empowerment, and promote the improvement and development of the industry ecosystem.

Currently, the DeepSpark Open Source Community is primarily focused on building and promoting the [Hundreds of Applications Open Platform](#hundreds-of-applications-open-platform), In the future, more related projects and achievements will be open-sourced through the DeepSpark community.

In August 2023, the DeepSpark Open Source Community signed a strategic cooperation agreement with the [Shanghai Baiyulan Open Source Research Institute](http://baiyulan.org.cn/) to further promote the co-construction and sharing of AI open-source initiatives and drive the improvement and development of the industry ecosystem. In November 2023, the DeepSpark community collaborated with the [OpenI Community](https://openi.pcl.ac.cn/), enabling community users to train models from DeepSparkHub using the [TianGai 100 computing power](https://openi.pcl.ac.cn/iluvatar/TianGai100) provided by OpenI's cloud brain.

We welcome industry partners, community users, and developers to contribute to the DeepSpark Open Source Community in any form. Your active participation is highly anticipated.

--------

## Hundreds of Applications Open Platform

As a leading domestic AI and general-purpose computing application development and evaluation platform, the Hundreds of Applications Open Platform carefully selects hundreds of open-source algorithms and models deeply integrated with industry applications. It supports mainstream ecosystem application frameworks and builds a multi-dimensional evaluation system tailored to industry needs, widely supporting various implementation scenarios.

### Application Algorithms and Models

[DeepSparkHub](https://gitee.com/deep-spark/deepsparkhub) selects hundreds of open-source application algorithms and models, covering various fields of AI and general-purpose computing. It supports mainstream intelligent computing scenarios in the market, including smart cities, digital individuals, healthcare, education, telecommunications, and energy.

[DeepSparkInference](https://gitee.com/deep-spark/deepsparkinference) selects inference model examples and guidance documents based on the independant-developed inference engines IGIE and IxRT. Some models provide evaluation results based on the self-developed GPGPU [ZhiKai 100](https://www.iluvatar.com/productDetails?fullCode=cpjs-yj-tlxltt-zk100).

### IXUCA (Iluvatar CoreX Unified Compute Architecture)

IXUCA is compatible with mainstream GPGPU computing models, providing equivalent components, features, APIs, and algorithms that support mainstream GPU computing. It enables seamless migration of systems or applications with minimal effort. The IXUCA stack includes AI deep learning applications, mainstream frameworks, libraries, compilers and tools, as well as runtime libraries and drivers.

- IXUCA integrates mainstream deep learning frameworks such as TensorFlow, PyTorch, and PaddlePaddle, delivering operators consistent with official open-source frameworks while continuously optimizing performance for Iluvatar CoreX acceleration cards.

- IXUCA provides the IGIE inference framework and IxRT inference engine, enabling optimal inference performance on Iluvatar CoreX acceleration cards.

- The libraries in IXUCA not only support general-purpose computing but also provide fundamental operators required for deep learning application development. Developers can conveniently utilize these operators to flexibly construct various deep neural network models and other machine learning algorithms.

You can visit the [Resource Center](https://support.iluvatar.com/#/ProductLine?id=2) on Iluvatar CoreX's official website to obtain the IXUCA software stack.

### Application Frameworks

The Hundreds of Applications Open Platform supports mainstream application frameworks and toolkits both domestically and internationally.

<table border="0">
    <tr align="center">
        <td><a href="https://github.com/pytorch"><img alt="pytorch" src="resources/pytorch.png" height="25"/></td>
        <td><a href="https://github.com/tensorflow"><img alt="tensorflow" src="resources/tensorflow.png" height="25"/></td>
    </tr>
    <tr align="center">
        <td><a href="https://github.com/paddlepaddle"><img alt="paddlepaddle" src="resources/paddlepaddle.png" height="40"/></td>
        <td><a href="https://github.com/microsoft/DeepSpeed"><img alt="deepspeed" src="resources/deepspeed.png" height="40"/></td>
    </tr>
    <tr align="center">
        <td><a href="https://github.com/facebookresearch/fairseq"><img alt="fairseq" src="resources/fairseq.png" height="40"/></td>
        <td><a href="https://github.com/open-mmlab/mmdetection"><img alt="mmdetection" src="resources/mmdetection.png" height="40"/></td>
    </tr>
    <tr align="center">
        <td><a href="https://github.com/wenet-e2e/wenet"><img alt= "wenet" src="resources/wenet.png" height="40"/></td>
        <td><a href="https://github.com/hpcaitech/ColossalAI"><img alt= "colossal-ai" src="resources/colossal-ai.png" height="30"/></td>
    </tr>
    <tr align="center">
        <td><a href="https://github.com/deepmodeling"><img alt="deepmodeling" src="resources/deepmodeling.png" height="40"/></td>
        <td><a href="https://github.com/hiyouga/LLaMA-Factory"><img alt="llama-factory" src="resources/llama-factory.png" height="45"/></td>
    </tr>
</table>

### Multi-Dimensional Benchmark Standards

The benchmark standards are widely applicable to hardware platforms, featuring a comprehensive system and simple deployment.

- Support 6️⃣ dimensions

| Dimension   | Description                                                           | Data Source                      | Calculation Method                                                                   |
|-------------|-----------------------------------------------------------------------|----------------------------------|--------------------------------------------------------------------------------------|
| Speed🚀     | Computing power per second for stable model training samples          | DeepSpark training script output | Remove highest/lowest of 5 iterations, take mean of middle 3 values                  |
| Accuracy🎯  | Model convergence accuracy value                                      | DeepSpark training script output | Record accuracy value at convergence                                                 |
| Linearity📈 | Linear scaling performance for cluster training (card/node linearity) | DeepSpark training script output | Multi-card/node speed divided by card/node count, compared to single-card/node speed |
| Power🔌     | Average GPU power consumption during stable training                  | GPU monitoring tool              | Average of multiple power measurements                                               |
| Memory📊    | Average GPU memory usage during stable training                       | GPU monitoring tool              | Average of multiple memory measurements                                              |
| Stability🔧 | Convergence value stability across multiple full training runs        | DeepSpark training script output | 5 full training runs, median as baseline, 20% deduction if any value deviates by ±1% |

Reference: [Hardware Benchmark Results](#hardware-evaluation-methods-and-results)

- 1️⃣-click deployment: Fully automated ✅, reproducible data 🔁, traceable scenarios 🔎

- 0️⃣ platform dependencies: No framework restrictions, no source language restrictions, no hardware restrictions

### Multi-Dimensional Benchmark System

[Multi-Dimensional Benchmark System](https://mdb.deepspark.org.cn:8086) is an online evaluation tool developed based on the [Multi-Dimensional Benchmark Standards](#multi-dimensional-benchmark-standards). It conducts model training evaluations on BI-V100 and NV-V100 accelerator cards under equal conditions across six dimensions (speed, accuracy, linearity, power efficiency, memory efficiency, and stability), collects metrics, and displays them in six-dimensional radar charts, enabling users to comprehensively compare and evaluate the overall capabilities of GPU accelerators. Below is the list of currently supported models:

![training model list](evaluation/Iluvatar/assets/mdb_model_list_1.png)

For usage details, please refer to the [Multi-Dimensional Benchmark System User Guide](evaluation/Iluvatar/Mdims-benchmark.md).

--------

### Hardware evaluation methods and results

#### TianGai 100 GPGPU

For evaluation methods, please refer to the [TianGai 100 Six-Dimension Benchmark Guide](evaluation/Iluvatar/six_dimension_howto.md).

The results is as below:

| Task                  | Model      | Convergence Metric | Configuration(x->gpus) | Speed  | Accuracy | Power(W) | Linearity | Memory Usage(GB) | Stability |
|-----------------------|------------|--------------------|------------------------|--------|----------|----------|-----------|------------------|-----------|
| NLP                   | BERT-large | 0.72               | sdk2.2,bs:32,8x,amp    | 214    | 0.72     | 152*8    | 0.96      | 20.3*8           | 1         |
| Recommendation System | DLRM       | AUC:0.75           | sdk2.2,bs:2048,8x,amp  | 793486 | 0.75     | 60*8     | 0.97      | 3.7*8            | 1         |
| Image Classification  | ResNet50   | top1 75.9%         | sdk2.2,bs:512,8x,amp   | 5221   | 76.43%   | 128*8    | 0.97      | 29.1*8           | 1         |
| Image Segmentation    | 3D U-Net   | 0.908              | sdk2.2,bs:4,8x,fp32    | 12     | 0.908    | 152*8    | 0.85      | 19.6*8           | 1         |
| Object Detection      | YOLOv5     | mAP:0.5            | sdk2.2,bs:128,8x,amp   | 1228   | 0.56     | 140*8    | 0.92      | 27.3*8           | 1         |
| Text Detection        | SATRN      | 0.841              | sdk2.2,bs:128,8x,fp32  | 630    | 88.4     | 166*8    | 0.98      | 28.5*8           | 1         |
| Speech Recognition    | Conformer  | 3.72               | sdk2.2,bs:32,8x,fp32   | 380    | 4.79     | 113*8    | 0.82      | 21.5*8           | 1         |
| 3D Reconstruction     | ngp-nerf   | 0.0046             | sdk2.2,bs:1,8x,amp     | 10     | 19.6     | 82*8     | 0.90      | 28.1*8           | 1         |
| Object Tracking       | FairMOT    | MOTA:69.8          | sdk2.2,bs:64,8x,fp32   | 52     | 69.8     | 132*8    | 0.97      | 19.1*8           | 1         |
| Large Model           | CPM        | 0.91               | sdk2.2,bs:128,8x,amp   | 357    | 0.91     | 156*8    | 0.93      | 20.6*8           | 1         |
| Speech Synthesis      | Tacotron2  | score(MOS):4.460   | sdk2.2,bs:128,8x,amp   | 77     | 4.46     | 128*8    | 0.96      | 18.4*8           | 1         |
| New Model             | Wave-MLP   | 80.1               | sdk2.2,bs:256,8x,fp32  | 1026   | 83.1     | 198*8    | 0.98      | 29.4*8           | 1         |

--------

## Community

### Code of Conduct

See [Code of Conduct](CODE_OF_CONDUCT.md).

### Contact

Contact <contact@deepspark.org.cn>.

### Contribution

Refer to each project's Contributing Guidelines.

### License

[Apache License 2.0](LICENSE).
