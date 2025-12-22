<!-- markdownlint-disable no-duplicate-heading -->
<!-- markdownlint-disable html -->
# Releasing DeepSpark

## Release Versioning

本项目采用基于发布年月的版本号命名策略，格式为 YY.MM，发布节奏为按季度发布，一般在每年的 3/6/9/12 月发布正式版本，版本号对应为 YY.03/YY.06/YY.09/YY.12。

## Release Notes

### DeepSpark 25.12

#### 特性和增强

* DeepSpark 新增了在天数智芯加速卡环境上[快速开始](docs/quickstart.md)的指导文档
* DeepSparkHub 新增了8个使用LLaMA-Factory工具箱的大模型训练微调示例。详见[25.12](https://gitee.com/deep-spark/deepsparkhub/releases/tag/25.12)版本日志。
* DeepSparkInference 新增了15个推理小模型示例，涵盖视觉分类，对象检测和多目标跟踪等领域，同时新增了8个大语言模型的推理示例，涉及vLLM和Diffusers框架。详见[25.12](https://gitee.com/deep-spark/deepsparkinference/releases/tag/25.12)版本日志。

<table>
    </tr>
        <tr align="left"><th colspan=5>LLM (LLaMA-Factory)</th></tr>
    <tr>
        <td>Llama3-8B-DPO</td>
        <td>Llama3-8B-Full-SFT</td>
        <td>Llama3-8B-KTO</td>
    </tr>
    <tr>
        <td>LlaMA3-8B-LoRA-Pretrain</td>
        <td>Llama3-8B-LoRA-Reward</td>
        <td>Llama3-8B-LoRA-SFT</td>
    </tr>
    <tr>
        <td>Qwen2.5-VL-LoRA-DPO</td>
        <td>Qwen2.5-VL-LoRA-SFT</td>
        <td></td>
    </tr>
  <th colspan=3>ixRT (Inference)</th>
  <tr>
      <td>DeepSort</td>
      <td>FastReID</td>
      <td>Transformer</td>
  </tr>
  <tr>
      <td>YOLOF </td>
      <td>YOLOv12</td>
      <td>YOLOv13</td>
  </tr>
  <th colspan=3>IGIE (Inference)</th>
  <tr>
      <td>EfficientNet-B7</td>
      <td>FreeAnchor</td>
      <td>RegNet_X_800MF </td>
  </tr>
  <tr>
      <td>RegNet_X_8GF</td>
      <td>PISA</td>
      <td>YOLOv8-N </td>
  </tr>
  <tr>
    <td>YOLOv9</td>
    <td>YOLOv10</td>
    <td>YOLOv11</td>
  </tr>
  <th colspan=3>LLM (Inference)</th>
  <tr>
      <td>NVLM-D (vLLM)</td>
      <td>PaliGemma (vLLM)</td>
      <td>Phi-3 Vision (vLLM)</td>
  </tr>
  <tr>
      <td>Pixtral (vLLM)</td>
      <td>Qwen3Moe (vLLM)</td>
      <td>Stable Diffusion 3 (Diffusers)</td>
  </tr>
  <tr>
      <td>Step3-VL (vLLM)</td>
      <td>XLM-RoBERTa (vLLM)</td>
      <td></td>
</table>

#### 贡献者

感谢以下人员做出的贡献：

sanghui_ilu，李一力，fanglaipeng，YoungPeng，anders，fhfang，郭寒冰，qiang.zhang，majorli6，honglyua。

欢迎以任何形式向DeepSpark社区贡献。

### DeepSpark 25.09

#### 特性和增强

* DeepSpark 修复了README文档中的markdownlint问题。
* DeepSparkHub 新增了10个大模型训练微调示例，其中7个为强化学习相关示例，使用了OpenRLHF和verl工具箱。详见[25.09版本日志](https://gitee.com/deep-spark/deepsparkhub/releases/tag/25.09)。
* DeepSparkInference 新增了19个推理小模型示例，涵盖视觉分类，对象检测和语义分割等领域，并新增了11个大语言模型的推理示例，涉及FastDeploy、LMDeploy和vLLM等框架。详见[25.09版本日志](https://gitee.com/deep-spark/deepsparkinference/releases/tag/25.09)。

#### 贡献者

感谢以下人员做出的贡献：

YoungPeng，fhfang，郭寒冰，qiang.zhang，sanghui_ilu，李一力，郝燕龙，胡方健，lsy789，张汉涛，fanglaipeng，majorli6，honglyua。

欢迎以任何形式向DeepSpark社区贡献。

### DeepSpark 25.06

#### 特性和增强

* DeepSpark 增加了首页的英文版README文档。
* DeepSparkHub 新增了1个小模型示例和5个大模型的强化学习微调示例，使用了verl和OpenRLHF工具箱。详见[25.06版本日志](https://gitee.com/deep-spark/deepsparkhub/releases/tag/25.06)。
* DeepSparkInference 新增了24个推理小模型示例，涵盖视觉分类，对象检测和语义分割等领域，并新增了6个基于vLLM的大语言模型的推理示例，其中3个为多模态模型。详见[25.06版本日志](https://gitee.com/deep-spark/deepsparkinference/releases/tag/25.06)。

#### 贡献者

感谢以下人员做出的贡献：

YoungPeng，张文风，qiang.zhang，李一力，sanghui-ilu，honglyua，majorli6，吴永乐。

欢迎以任何形式向DeepSpark社区贡献。

### DeepSpark 25.03

#### 特性和增强

* 首页README文档添加了天数智算软件栈IXUCA的介绍。
* DeepSparkHub 25.03版本新增了9个基于MoE-LLaVA，DeepSpeed和LLaMA-Factory的大语言模型的训练示例。具体详见DeepSparkHub 25.03版本日志。
* DeepSparkInference 25.03版本新增了25个推理小模型，涵盖图片分类，对象检测和姿态估计等领域，并新增了11个基于vLLM的大语言模型的推理示例，其中6个为DeepSeek-R1蒸馏模型。具体详见DeepSparkInference 25.03版本日志。

#### 贡献者

感谢以下人员做出的贡献：

YoungPeng，xinchi.tian，xiaomei.wang，qiang.zhang，李一力，sanghui-ilu，honglyua，majorli6，吴永乐。

欢迎以任何形式向DeepSpark社区贡献。

### DeepSpark 24.12

#### 特性和增强

* DeepSparkHub 24.12版本新增了4个PyTorch模型，其中2个为Multimodal模型，同时新增了5个基于ColossalAI，Megatron-LM和LLaMA-Factory的大语言模型的训练示例。具体详见DeepSparkHub 24.12版本日志。
* DeepSparkInference 24.12版本新增了24个推理小模型，涵盖图片分类，对象检测和文字识别等领域，并新增了9个基于vLLM和ixFormer的大语言模型的推理示例。具体详见DeepSparkInference 24.12版本日志。

#### 贡献者

感谢以下人员做出的贡献：

YoungPeng，xinchi.tian，xiaomei.wang，qiang.zhang，李一力，sanghui-ilu，honglyua，majorli6，吴永乐。

欢迎以任何形式向DeepSpark社区贡献。

### DeepSpark 24.09

#### 特性和增强

* DeepSparkHub 24.09版本新增了5个PyTorch模型，其中3个为Stable Diffusion模型，同时新增了4个基于DeepSpeed、Megatron DeepSpeed和Firefly的大语言模型的训练示例，并修复了一些模型执行步骤和版本兼容相关的问题。具体详见DeepSparkHub 24.09版本日志。
* DeepSparkInference 24.09版本新增了29个推理模型示例和对ByteMLPerf工具箱的支持，涵盖计算机视觉，自然语言处理和语音识别等领域，同时新增了5个基于vLLM，TensorRT-LLM和Text Generation Inference的大语言模型的推理示例。具体详见DeepSparkInference 24.09版本日志 。

#### 贡献者

感谢以下人员做出的贡献：

majorli。

欢迎以任何形式向DeepSpark社区贡献。

---

### DeepSpark 24.06

#### 特性和增强

* DeepSparkHub 24.06版本新增了7个PyTorch训练模型和对OpenPCDet工具箱的支持，同时新增了8个基于DeepSpeed，Megatron DeepSpeed和Firefly的大语言模型的训练示例，并修复了一些模型执行步骤和版本兼容相关的问题。具体详见DeepSparkHub 24.06版本日志。
* DeepSparkInference 24.06版本新增了31个推理模型示例，其中支持IGIE推理引擎的16个，支持IxRT推理引擎的15个，涵盖计算机视觉，自然语言处理等领域。同时新增了4个基于vLLM，TensorRT-LLM和Text Generation Inference的大语言模型的推理示例。具体详见DeepSparkInference 24.06版本日志 。

#### 贡献者

感谢以下人员做出的贡献：

majorli。

欢迎以任何形式向DeepSpark社区贡献。

---

### DeepSpark 24.03

#### 特性和增强

* DeepSparkHub 24.03版本新增了10个基于PyTorch和PaddlePaddle框架的算法模型，涉及计算机视觉、多模态领域。同时新增了大语言模型Megatron-DeepSpeed Llama-2-7B SFT和DeepSpeed Llama-2-7B Reward Model Finetuning的训练示例，并修复了一些模型执行步骤和版本兼容相关的问题。具体详见DeepSparkHub 24.03版本日志。

#### 贡献者

感谢以下人员做出的贡献：

majorli。

欢迎以任何形式向DeepSpark社区贡献。

---

### DeepSpark 23.12

#### 特性和增强

* DeepSparkHub 23.12版本新增了30个基于PyTorch和PaddlePaddle框架的算法模型，涉及计算机视觉、自然语言处理、语音识别、多模态、图神经网络、推荐和强化学习等领域。同时新增了基于分布式训练框架Megatron-DeepSpeed的大语言模型LLaMA2-7B的训练示例，并修复了一些模型执行步骤和版本兼容相关的问题。具体详见DeepSparkHub 23.12版本日志。

#### 贡献者

感谢以下人员做出的贡献：

majorli。

欢迎以任何形式向DeepSpark社区贡献。

---

### DeepSpark 23.09

#### 特性和增强

* DeepSparkHub新增了30个基于PyTorch/TensorFlow/MindSpore/PaddlePaddle的算法模型，涉及计算机视觉，图神经网络，自然语言处理，语音识别等领域。同时新增了基于分布式训练框架Colossal-AI和DeepSpeed的大语言模型LLaMA-7B和ChatGLM-6B的训练示例，以及基于深度学习分子动力学套件DeePMD-kit的水分子模型训练示例。同时修复了一些模型数据集和执行步骤相关的问题。具体详见DeepSparkHub 23.09版本日志 。

#### 贡献者

感谢以下人员做出的贡献：

majorli，tonychen。

欢迎以任何形式向DeepSpark社区贡献。

---

### DeepSpark 23.06

#### 特性和增强

* 添加了30个基于PyTorch框架的算法模型，新增了网络剪枝、自监督学习、知识蒸馏这3种模型类别。
* 新增30个模型中有12个使用了开源工具箱：
  * Transformer，U2++ Conformer，Unified Conformer模型基于开源的WeNet工具箱。
  * ATSS，Cascade R-CNN，CornerNet，DCNV2，RepPoints模型基于开源的MMDetection工具箱。
  * BART，Convoluntional，RoBERTa，Transformer模型基于开源的Fairseq工具箱。

#### 贡献者

感谢以下人员做出的贡献：

majorli。

欢迎以任何形式向DeepSpark社区贡献。

---

### DeepSpark 23.03

#### 特性和增强

* 新增了对TensorFlow和MindSpore的支持。

* 新增基于TensorFlow和MindSpore的模型各5个，PaddlePaddle模型10个，PyTorch模型15个。

#### 贡献者

感谢以下人员做出的贡献：

chenyingtony。

欢迎以任何形式向DeepSpark社区贡献。

---

### DeepSpark 22.12

#### 特性和增强

* SATRN，Conformer和ngp-nerf模型更新[六维度评测数据](README.md#硬件评测方法和结果)。
* 添加了基于国产通用GPU天垓100的六维度评测[方法](evaluation/Iluvatar/six_dimension_howto.md)和[示例](evaluation/Iluvatar/six_dimension_howto_example.md)。
* 应用开放平台新增基于PaddlePaddle框架的19个[模型](https://gitee.com/deep-spark/deepsparkhub)。

#### 贡献者

感谢以下人员做出的贡献：

li-shi-kun，tonychen，majorli，李睿，Jeff Guo。

欢迎以任何形式向DeepSpark社区贡献。
