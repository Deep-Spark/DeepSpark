<!-- markdownlint-disable first-line-h1 -->
<!-- markdownlint-disable html -->
[<img alt="English" src="https://img.shields.io/badge/Language-English-blue.svg">](README_en.md) [<img alt="Chinese" src="https://img.shields.io/badge/语言-简体中文-red.svg">](README.md)

# DeepSpark开源社区

<div align="center" style="line-height: 1;">
  <a href="https://www.deepspark.org.cn"><img alt="Homepage"
    src="https://img.shields.io/badge/DeepSpark-Homepage-blue.svg"/></a>
  <a href="./LICENSE"><img alt="LICENSE" src="https://img.shields.io/badge/license-Apache%202.0-dfd.svg"></a>
  <a href="https://gitee.com/deep-spark/deepspark/releases/latest"><img alt="Release" src="https://img.shields.io/github/v/release/deep-spark/deepspark?color=ffa"></a>
</div>
<br>

在万物皆算的时代，各领域应用层出不穷，算力必须支撑实际应用，通用性和未来可扩展性是评估算力的重要指标。天数智芯作为国内头部通用GPU高端芯片及超级算力系统提供商，截止2024年12月，已成功支持 400+ AI算法模型，覆盖训练和推理，与 400+ 家客户和生态伙伴建立合作，共同促进国内通用算力的发展，产品服务于智慧城市、数字个人、医疗、教育、通信、能源等多个领域。

天数智芯本着“平台共建、生态共享、产业共赢”的原则，致力于和行业伙伴一起打造[DeepSpark开源社区](https://www.deepspark.org.cn/)，以来自开源回馈开源的方式，汇聚社区力量，助力客户加速应用落地和收获算力赋能，促进产业生态的完善和发展。

DeepSpark开源社区目前主要致力于[百大应用开放平台](#百大应用开放平台)的打造和推广，将来会有更多相关的项目和成果通过DeepSpark社区开源。

2023年8月，DeepSpark开源社区与[上海白玉兰开源开放研究院](http://baiyulan.org.cn/)签署了战略合作协议，旨在进一步促进人工智能开源事业共建共享，推动产业生态的完善和发展。2023年11月，DeepSpark社区与[启智社区](https://openi.pcl.ac.cn/)开展合作，社区用户可通过启智云脑提供的[天垓100算力](https://openi.pcl.ac.cn/iluvatar/TianGai100)训练来自DeepSparkHub的模型。

欢迎行业合作伙伴、社区用户和开发者以任何形式为DeepSpark开源社区作贡献，期待您的积极参与。

--------

## 百大应用开放平台

百大应用开放平台作为国内领先的AI和通用计算应用开发及评测平台，甄选上百个与行业应用深度耦合的开源算法和模型，支持主流生态应用框架，并针对行业需求构建多维度评测体系，广泛支持各类落地场景。

### 应用算法和模型

- [DeepSparkHub](https://gitee.com/deep-spark/deepsparkhub)甄选上百个开源应用算法和模型，覆盖AI和通用计算各领域，支持主流市场智能计算场景，包括智慧城市、数字个人、医疗、教育、通信、能源等多个领域。

- [DeepSparkInference](https://gitee.com/deep-spark/deepsparkinference)精选基于国产推理引擎IGIE和ixRT的小模型推理示例，以及使用vLLM等主流开源推理引擎的大语言模型推理示例。

### 支持的应用框架

百大应用开放平台支持国内外主流应用框架和工具箱。

<table border="0">
    <tr align="center">
        <td><a href="https://github.com/pytorch"><img alt="pytorch" src="https://github.com/pytorch/pytorch/raw/main/docs/source/_static/img/pytorch-logo-dark.png" height="30"/></td>
        <td><a href="https://github.com/tensorflow"><img alt="tensorflow" src="https://www.tensorflow.org/images/tf_logo_horizontal.png" height="50"/></td>
        <td><a href="https://github.com/paddlepaddle"><img alt="paddlepaddle" src="https://raw.githubusercontent.com/PaddlePaddle/Paddle/refs/heads/develop/doc/imgs/logo.png" height="45"/></td>
    </tr>
    <tr align="center">
        <td><a href="https://github.com/facebookresearch/fairseq"><img alt="fairseq" src="https://raw.githubusercontent.com/facebookresearch/fairseq/refs/heads/main/docs/fairseq_logo.png" height="35"/></td>
        <td><a href="https://github.com/wenet-e2e/wenet"><img alt= "wenet" src="resources/wenet.png" height="40"/></td>
        <td><a href="https://github.com/microsoft/DeepSpeed"><img alt="deepspeed" src="https://raw.githubusercontent.com/deepspeedai/DeepSpeed/refs/heads/master/docs/assets/images/DeepSpeed_light.svg" height="55"/></td>
    </tr>
    <tr align="center">
        <td><a href="https://github.com/hpcaitech/ColossalAI"><img alt= "colossal-ai" src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/colossal-ai_logo_vertical.png" height="25"/></td>
        <td><a href="https://github.com/volcengine/verl"><img alt="verl" src="resources/verl.png" height="40"/></td>
        <td><a href="https://github.com/hiyouga/LLaMA-Factory"><img alt="llama-factory" src="https://raw.githubusercontent.com/hiyouga/LLaMA-Factory/refs/heads/main/assets/logo.png" height="45"/></td>
    </tr>
    <tr align="center">
        <td><a href="https://github.com/microsoft/onnxruntime"><img alt="ONNXRUNTIME" src="https://raw.githubusercontent.com/microsoft/onnxruntime/refs/heads/main/docs/images/ONNX_Runtime_logo.png" height="55"/></td>
        <td><a href="https://github.com/vllm-project/vllm"><img alt="vLLM" src="https://raw.githubusercontent.com/vllm-project/vllm/main/docs/assets/logos/vllm-logo-text-light.png" height="35"/></td>
        <td><a href="https://github.com/InternLM/lmdeploy"><img alt="LMDeploy" src="https://raw.githubusercontent.com/InternLM/lmdeploy/refs/heads/main/docs/en/_static/image/lmdeploy-logo.svg" height="40"/></td>
    </tr>
</table>

### 已开源软件项目

| 项目名称                                                                      | 项目类别   | 项目简介                                                                                          |
|-------------------------------------------------------------------------------|------------|---------------------------------------------------------------------------------------------------|
| [iluvatar-corex-ixrt](https://gitee.com/deep-spark/iluvatar-corex-ixrt.git)   | 推理引擎   | 天数智芯Iluvatar CoreX ixRT高性能推理引擎的开源代码部分，含插件、部署工具和应用示例。             |
| [tis-igie-backend](https://gitee.com/deep-spark/tis-igie-backend.git)         | 推理后端   | 天数智芯IGIE推理引擎对接Triton推理服务框架的推理后端                                              |
| [tis-ixrt-backend](https://gitee.com/deep-spark/tis-ixrt-backend.git)         | 推理后端   | 天数智芯ixRT推理引擎对接Triton推理服务框架的推理后端                                              |
| [go-ixdcgm](https://gitee.com/deep-spark/go-ixdcgm.git)                       | 云原生支持 | 提供天数智芯ixDCGM（数据中心GPU管理软件）的Golang API接口                                         |
| [go-ixml](https://gitee.com/deep-spark/go-ixml.git)                           | 云原生支持 | 提供天数智芯加速卡的ixML系统管理接口的Golang API接口                                              |
| [ix-container-toolkit](https://gitee.com/deep-spark/ix-container-toolkit.git) | 云原生支持 | 帮助用户快速构建和运行天数加速卡容器的工具集，提供容器运行时支持                                  |
| [ix-device-plugin](https://gitee.com/deep-spark/ix-device-plugin.git)         | 云原生支持 | 针对天数智芯GPGPU的Kubernetes集群设备扩展插件，通过DaemonSet部署调度GPU资源                       |
| [ix-exporter](https://gitee.com/deep-spark/ix-exporter.git)                   | 云原生支持 | Kubernetes集群资源监控插件，为天数智芯GPGPU提供远程实时指标统计                                   |
| [ix-feature-discovery](https://gitee.com/deep-spark/ix-feature-discovery.git) | 云原生支持 | 自动为K8S集群节点上可用的天数智芯加速卡生成标签                                                   |
| [ix-gpu-operator](https://gitee.com/deep-spark/ix-gpu-operator.git)           | 云原生支持 | 帮助用户在Kubernetes集群配置和管理天数智芯GPGPU加速卡                                             |
| [ix-volcano-plugin](https://gitee.com/deep-spark/ix-volcano-plugin.git)       | 云原生支持 | 基于Volcano调度器的扩展，为天数GPU集群多节点多GPU任务提供最优拓扑调度策略                         |
| [ixgdb](https://gitee.com/deep-spark/ixgdb.git)                               | 工具       | 基于CUDA-GDB开发的天数智芯通用GPU加速卡开源调试工具，是GDB的扩展                                  |
| [ixjpeg-python](https://gitee.com/deep-spark/ixjpeg-python.git)               | 工具       | 基于ixJPEG库的Python封装，提供JPEG图像编码和解码功能                                              |

## 天数智芯智算平台 IXUCA

IXUCA兼容主流GPU通用计算模型，提供支持主流GPU通用计算模型的等效组件、特性、API和算法，可助力用户便捷地实现系统或应用的无痛迁移。天数智算软件栈包括人工智能深度学习应用、主流框架、函数库、编译器及工具、运行时库及驱动。

- IXUCA集成了TensorFlow、PyTorch、百度飞桨PaddlePaddle等国内外主流的深度学习框架，提供与官方开源框架一致的算子，并针对天数智芯加速卡持续优化性能。

- IXUCA提供IGIE推理框架和ixRT推理引擎，支持在天数智芯加速卡上实现最优推理性能。

- IXUCA的函数库不仅支持通用计算还提供了深度学习应用开发所需的基础算子，开发者可以便捷地调用这些算子灵活地构造各类深度神经网络模型以及其他机器学习领域的算法。

您可前往天数智芯官方网站的[资源中心](https://support.iluvatar.com/#/ProductLine?id=2)获取天数智算软件栈。

--------

## 社区

### 治理

请参见 [Code of Conduct](CODE_OF_CONDUCT.md)。

### 交流

请联系 <contact@deepspark.org.cn>。

### 贡献

请参见各项目的Contributing Guidelines。

### 许可证

[Apache License 2.0](LICENSE)。
