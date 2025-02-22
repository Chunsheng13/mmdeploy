<div align="center">
  <img src="resources/mmdeploy-logo.png" width="450"/>
  <div>&nbsp;</div>
  <div align="center">
    <b><font size="5">OpenMMLab 官网</font></b>
    <sup>
      <a href="https://openmmlab.com">
        <i><font size="4">HOT</font></i>
      </a>
    </sup>
    &nbsp;&nbsp;&nbsp;&nbsp;
    <b><font size="5">OpenMMLab 开放平台</font></b>
    <sup>
      <a href="https://platform.openmmlab.com">
        <i><font size="4">TRY IT OUT</font></i>
      </a>
    </sup>
  </div>
  <div>&nbsp;</div>
</div>

[![docs](https://img.shields.io/badge/docs-latest-blue)](https://mmdeploy.readthedocs.io/zh_CN/latest/)
[![badge](https://github.com/open-mmlab/mmdeploy/workflows/build/badge.svg)](https://github.com/open-mmlab/mmdeploy/actions)
[![codecov](https://codecov.io/gh/open-mmlab/mmdeploy/branch/master/graph/badge.svg)](https://codecov.io/gh/open-mmlab/mmdeploy)
[![license](https://img.shields.io/github/license/open-mmlab/mmdeploy.svg)](https://github.com/open-mmlab/mmdeploy/blob/master/LICENSE)
[![issue resolution](https://img.shields.io/github/issues-closed-raw/open-mmlab/mmdeploy)](https://github.com/open-mmlab/mmdeploy/issues)
[![open issues](https://img.shields.io/github/issues-raw/open-mmlab/mmdeploy)](https://github.com/open-mmlab/mmdeploy/issues)

[English](README.md) | 简体中文

## 介绍

MMDeploy 是 [OpenMMLab](https://openmmlab.com/) 模型部署工具箱，**为各算法库提供统一的部署体验**。基于 MMDeploy，开发者可以轻松从训练 repo 生成指定硬件所需 SDK，省去大量适配时间。

## 架构简析

<div align="center">
  <img src="resources/introduction.png"/>
</div>

## 特性简介

### 支持超多 OpenMMLab 算法库

- [mmcls](docs/en/04-supported-codebases/mmcls.md)
- [mmdet](docs/en/04-supported-codebases/mmdet.md)
- [mmseg](docs/en/04-supported-codebases/mmseg.md)
- [mmedit](docs/en/04-supported-codebases/mmedit.md)
- [mmocr](docs/en/04-supported-codebases/mmocr.md)
- [mmpose](docs/en/04-supported-codebases/mmpose.md)
- [mmdet3d](docs/en/04-supported-codebases/mmdet3d.md)
- [mmrotate](docs/en/04-supported-codebases/mmrotate.md)

### 支持多种推理后端

| ONNX Runtime | TensorRT | ppl.nn | ncnn | OpenVINO | more                                              |
| ------------ | -------- | ------ | ---- | -------- | ------------------------------------------------- |
| ✔️           | ✔️       | ✔️     | ✔️   | ✔️       | [benchmark](docs/zh_cn/03-benchmark/benchmark.md) |

### SDK 可高度定制化

- Transform 数据预处理
- Net 推理
- Module 后处理

## [快速上手](docs/zh_cn/get_started.md)

- [编译](docs/zh_cn/01-how-to-build/build_from_source.md)
  - [Build from Docker](docs/zh_cn/01-how-to-build/build_from_docker.md)
  - [Build for Linux](docs/zh_cn/01-how-to-build/linux-x86_64.md)
  - [Build for Win10](docs/zh_cn/01-how-to-build/windows.md)
  - [Build for Android](docs/zh_cn/01-how-to-build/android.md)
  - [Build for Jetson](docs/en/01-how-to-build/jetsons.md)
- 使用
  - [把模型转换到推理 Backend](docs/zh_cn/02-how-to-run/convert_model.md)
  - [配置转换参数](docs/zh_cn/02-how-to-run/write_config.md)
  - [量化](docs/zh_cn/02-how-to-run/quantize_model.md)
  - [测试转换完成的模型](docs/zh_cn/02-how-to-run/profile_model.md)
- 开发指南
  - [支持新模型](docs/zh_cn/04-developer-guide/support_new_model.md)
  - [增加推理 Backend](docs/zh_cn/04-developer-guide/support_new_backend.md)
  - [回归测试](docs/zh_cn/04-developer-guide/do_regression_test.md)
- [FAQ](docs/zh_cn/faq.md)
- [贡献者手册](.github/CONTRIBUTING.md)

## 新人解说

- [01 术语解释、加载第一个模型](docs/zh_cn/05-tutorial/01_introduction_to_model_deployment.md)
- [02 转成 onnx](docs/zh_cn/05-tutorial/02_challenges.md)

## 基准与模型库

基准和支持的模型列表可以在[基准](https://mmdeploy.readthedocs.io/zh_CN/latest/benchmark.html)和[模型列表](https://mmdeploy.readthedocs.io/en/latest/supported_models.html)中获得。

## 贡献指南

我们感谢所有的贡献者为改进和提升 MMDeploy 所作出的努力。请参考[贡献指南](.github/CONTRIBUTING.md)来了解参与项目贡献的相关指引。

## 致谢

- [OpenPPL](https://github.com/openppl-public/ppl.nn): 高性能推理框架底层库
- [OpenVINO](https://github.com/openvinotoolkit/openvino): AI 推理优化和部署框架
- [ncnn](https://github.com/tencent/ncnn): 为手机端极致优化的高性能神经网络前向计算框架

## 引用

如果您在研究中使用了本项目的代码或者性能基准，请参考如下 bibtex 引用 MMDeploy:

```BibTeX
@misc{=mmdeploy,
    title={OpenMMLab's Model Deployment Toolbox.},
    author={MMDeploy Contributors},
    howpublished = {\url{https://github.com/open-mmlab/mmdeploy}},
    year={2021}
}
```

## 开源许可证

该项目采用 [Apache 2.0 开源许可证](LICENSE)。

## OpenMMLab 的其他项目

- [MMCV](https://github.com/open-mmlab/mmcv): OpenMMLab 计算机视觉基础库
- [MIM](https://github.com/open-mmlab/mim): MIM 是 OpenMMlab 项目、算法、模型的统一入口
- [MMClassification](https://github.com/open-mmlab/mmclassification): OpenMMLab 图像分类工具箱
- [MMDetection](https://github.com/open-mmlab/mmdetection): OpenMMLab 目标检测工具箱
- [MMDetection3D](https://github.com/open-mmlab/mmdetection3d): OpenMMLab 新一代通用 3D 目标检测平台
- [MMRotate](https://github.com/open-mmlab/mmrotate): OpenMMLab 旋转框检测工具箱与测试基准
- [MMSegmentation](https://github.com/open-mmlab/mmsegmentation): OpenMMLab 语义分割工具箱
- [MMOCR](https://github.com/open-mmlab/mmocr): OpenMMLab 全流程文字检测识别理解工具包
- [MMPose](https://github.com/open-mmlab/mmpose): OpenMMLab 姿态估计工具箱
- [MMHuman3D](https://github.com/open-mmlab/mmhuman3d): OpenMMLab 人体参数化模型工具箱与测试基准
- [MMSelfSup](https://github.com/open-mmlab/mmselfsup): OpenMMLab 自监督学习工具箱与测试基准
- [MMRazor](https://github.com/open-mmlab/mmrazor): OpenMMLab 模型压缩工具箱与测试基准
- [MMFewShot](https://github.com/open-mmlab/mmfewshot): OpenMMLab 少样本学习工具箱与测试基准
- [MMAction2](https://github.com/open-mmlab/mmaction2): OpenMMLab 新一代视频理解工具箱
- [MMTracking](https://github.com/open-mmlab/mmtracking): OpenMMLab 一体化视频目标感知平台
- [MMFlow](https://github.com/open-mmlab/mmflow): OpenMMLab 光流估计工具箱与测试基准
- [MMEditing](https://github.com/open-mmlab/mmediting): OpenMMLab 图像视频编辑工具箱
- [MMGeneration](https://github.com/open-mmlab/mmgeneration): OpenMMLab 图片视频生成模型工具箱
- [MMDeploy](https://github.com/open-mmlab/mmdeploy): OpenMMLab 模型部署框架

## 欢迎加入 OpenMMLab 社区

扫描下方的二维码可关注 OpenMMLab 团队的 [知乎官方账号](https://www.zhihu.com/people/openmmlab)，加入 OpenMMLab 团队的 [官方交流 QQ 群](https://jq.qq.com/?_wv=1027&k=MSMAfWOe)，或添加微信小助手”OpenMMLabwx“加入官方交流微信群。

<div align="center">
  <img src="https://raw.githubusercontent.com/open-mmlab/mmcv/master/docs/en/_static/zhihu_qrcode.jpg" height="400" />
  <img src="resources/qq_group_qrcode.jpg" height="400" />
  <img src="https://raw.githubusercontent.com/open-mmlab/mmcv/master/docs/en/_static/wechat_qrcode.jpg" height="400" />
</div>

我们会在 OpenMMLab 社区为大家

- 📢 分享 AI 框架的前沿核心技术
- 💻 解读 PyTorch 常用模块源码
- 📰 发布 OpenMMLab 的相关新闻
- 🚀 介绍 OpenMMLab 开发的前沿算法
- 🏃 获取更高效的问题答疑和意见反馈
- 🔥 提供与各行各业开发者充分交流的平台

干货满满 📘，等您来撩 💗，OpenMMLab 社区期待您的加入 👬
