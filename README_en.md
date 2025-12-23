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

## Hundreds of Applications Open Platform

As a leading domestic AI and general-purpose computing application development and evaluation platform, the Hundreds of Applications Open Platform carefully selects hundreds of open-source algorithms and models deeply integrated with industry applications. It supports mainstream ecosystem application frameworks and builds a multi-dimensional evaluation system tailored to industry needs, widely supporting various implementation scenarios.

### Application Algorithms and Models

[DeepSparkHub](https://gitee.com/deep-spark/deepsparkhub) selects hundreds of open-source application algorithms and models, covering various fields of AI and general-purpose computing. It supports mainstream intelligent computing scenarios in the market, including smart cities, digital individuals, healthcare, education, telecommunications, and energy.

[DeepSparkInference](https://gitee.com/deep-spark/deepsparkinference) selects small inference model examples and guidance documents based on the independant-developed inference engines IGIE and ixRT, as well as large language model inference examples using mainstream open-source inference engines such as vLLM.

### Supported Application Frameworks

The Hundreds of Applications Open Platform supports mainstream application frameworks and toolkits both domestically and internationally.

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

### Open Source Projects

| Project                                                                       | Description                                                                                |
|-------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------|
| [iluvatar-corex-ixrt](https://gitee.com/deep-spark/iluvatar-corex-ixrt.git)   | Iluvatar CoreX ixRT high performance inference engine with examples.                       |
| [tis-igie-backend](https://gitee.com/deep-spark/tis-igie-backend.git)         | Iluvatar CoreX IGIE backend of Triton inference framework.                                 |
| [tis-ixrt-backend](https://gitee.com/deep-spark/tis-ixrt-backend.git)         | Iluvatar CoreX ixRT backend of Triton inference framework.                                 |
| [go-ixdcgm](https://gitee.com/deep-spark/go-ixdcgm.git)                       | Iluvatar CoreX ixDCGM (Data Center GPU Management) Golang API.                             |
| [go-ixml](https://gitee.com/deep-spark/go-ixml.git)                           | Iluvatar CoreX ixML (Management Library) Golang API.                                       |
| [ix-container-toolkit](https://gitee.com/deep-spark/ix-container-toolkit.git) | Includes a container runtime and utilities to auto-configure containers for Iluvatar GPUs. |
| [ix-device-plugin](https://gitee.com/deep-spark/ix-device-plugin.git)         | DaemonSet for Kubernetes that can help to expose the Iluvatar GPU in the K8s cluster.      |
| [ix-exporter](https://gitee.com/deep-spark/ix-exporter.git)                   | Ix Exporter is an HTTP server that exposes Iluvatar GPU node information in K8s cluster.   |
| [ix-feature-discovery](https://gitee.com/deep-spark/ix-feature-discovery.git) | Allows to auto-generate labels for the set of Iluvatar CoreX GPUs available on a node.     |
| [ix-gpu-operator](https://gitee.com/deep-spark/ix-gpu-operator.git)           | Designed to help the user to provision and configure gpu components in the K8s cluster.    |
| [ix-volcano-plugin](https://gitee.com/deep-spark/ix-volcano-plugin.git)       | Volcano scheduler extension providing optimal topology scheduling in Iluvatar GPU cluster. |
| [ixgdb](https://gitee.com/deep-spark/ixgdb.git)                               | Iluvatar GPGPU Accelerator Open-Source Debugger: A GDB Extension based on CUDA-GDB.        |
| [ixjpeg-python](https://gitee.com/deep-spark/ixjpeg-python.git)               | Python wrapper for ixJPEG that provides JPEG encoding and decoding functionality.          |

### IXUCA (Iluvatar CoreX Unified Compute Architecture)

IXUCA is compatible with mainstream GPGPU computing models, providing equivalent components, features, APIs, and algorithms that support mainstream GPU computing. It enables seamless migration of systems or applications with minimal effort. The IXUCA stack includes AI deep learning applications, mainstream frameworks, libraries, compilers and tools, as well as runtime libraries and drivers.

- IXUCA integrates mainstream deep learning frameworks such as TensorFlow, PyTorch, and PaddlePaddle, delivering operators consistent with official open-source frameworks while continuously optimizing performance for Iluvatar CoreX acceleration cards.

- IXUCA provides the IGIE inference framework and ixRT inference engine, enabling optimal inference performance on Iluvatar CoreX acceleration cards.

- The libraries in IXUCA not only support general-purpose computing but also provide fundamental operators required for deep learning application development. Developers can conveniently utilize these operators to flexibly construct various deep neural network models and other machine learning algorithms.

### How To

You can visit the [Resource Center](https://support.iluvatar.com/#/ProductLine?id=2) on Iluvatar CoreX's official website to obtain the IXUCA software stack. Then you can refer to the [quick start guide](docs/quickstart.md) to install IXUCA SDK into your environments and run training or inference samples in DeepSparkHub and DeepSparkInference modelzoo.

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
