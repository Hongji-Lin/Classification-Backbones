Awesome backbones for image classification
===========================

<div align="center">
![](https://img.shields.io/badge/Awesome%20Backbones-v0.6.2-brightgreen)
![](https://img.shields.io/badge/PyTorch-%3E%3Dv1.7.1-green)
![](https://img.shields.io/badge/Python-%3E%3Dv3.6-yellowgreen)
[![GitHub forks](https://img.shields.io/github/forks/Fafa-DL/Awesome-Backbones)](https://github.com/Fafa-DL/Awesome-Backbones)
[![GitHub stars](https://img.shields.io/github/stars/Fafa-DL/Awesome-Backbones)](https://github.com/Fafa-DL/Awesome-Backbones)
![Visitors](https://visitor-badge.glitch.me/badge?page_id=Fafa-DL.Awesome-Backbones&right_color=yellow)

</div>

## 更新日志

**`2022.11.06`** 
- 新增**HorNet**, **EfficientFormer**, **SwinTransformer V2**, **MViT**模型

**`2022.09.13`** 
- 新增可视化数据增强pipeline功能，详见[Pipeline visualization](https://github.com/Fafa-DL/Awesome-Backbones/blob/main/datas/docs/Pipeline_visualization.md)
- 很有必要预览整个数据集的数据增强结果，如果遮挡/变形失真的图片比例`占据较多`，很有可能导致准确率下降，因为其主导了训练loss走向!
- ![](https://raw.githubusercontent.com/Fafa-DL/readme-data/main/backbones/fail01.jpg) ![](https://raw.githubusercontent.com/Fafa-DL/readme-data/main/backbones/fail02.jpg) ![](https://raw.githubusercontent.com/Fafa-DL/readme-data/main/backbones/fail03.jpg)

**`2022.09.09`** 
- 新增计算模型参数量Parameters与浮点运算量Flops功能，详见[Calculate Flops](https://github.com/Fafa-DL/Awesome-Backbones/blob/main/datas/docs/Calculate_Flops.md)

## 测试环境

- Pytorch      1.7.1+
- Python       3.6+

## 资料
|数据集|视频教程|人工智能技术探讨群|
|---|---|---|
|[`花卉数据集` 提取码：0zat](https://pan.baidu.com/s/1137y4l-J3AgyCiC_cXqIqw)|[点我跳转](https://www.bilibili.com/video/BV1SY411P7Nd)|[1群：78174903](https://jq.qq.com/?_wv=1027&k=lY5KVICA)<br/>[3群：584723646](https://jq.qq.com/?_wv=1027&k=bakez5Yz)

## 快速开始

- 遵循[环境搭建](https://github.com/Fafa-DL/Awesome-Backbones/blob/main/datas/docs/Environment_setting.md)完成配置
- 下载[MobileNetV3-Small](https://download.openmmlab.com/mmclassification/v0/mobilenet_v3/convert/mobilenet_v3_small-8427ecf0.pth)权重至**datas**下
- **Awesome-Backbones**文件夹下终端输入
```bash
python tools/single_test.py datas/cat-dog.png models/mobilenet/mobilenet_v3_small.py --classes-map datas/imageNet1kAnnotation.txt
```

## 教程
- [环境搭建](https://github.com/Fafa-DL/Awesome-Backbones/blob/main/datas/docs/Environment_setting.md)
- [数据集准备](https://github.com/Fafa-DL/Awesome-Backbones/blob/main/datas/docs/Data_preparing.md)
- [配置文件解释](https://github.com/Fafa-DL/Awesome-Backbones/blob/main/datas/docs/Configs_description.md)
- [训练](https://github.com/Fafa-DL/Awesome-Backbones/blob/main/datas/docs/How_to_train.md)
- [模型评估](https://github.com/Fafa-DL/Awesome-Backbones/blob/main/datas/docs/How_to_eval.md)
- [计算Flops&Params](https://github.com/Fafa-DL/Awesome-Backbones/blob/main/datas/docs/Calculate_Flops.md)
- [添加新的模型组件](https://github.com/Fafa-DL/Awesome-Backbones/blob/main/datas/docs/Add_modules.md)
- [类别激活图可视化](https://github.com/Fafa-DL/Awesome-Backbones/blob/main/datas/docs/CAM_visualization.md)
- [学习率策略可视化](https://github.com/Fafa-DL/Awesome-Backbones/blob/main/datas/docs/Lr_visualization.md)

## 模型
- [x] [LeNet5](https://ieeexplore.ieee.org/document/6795724)
- [x] [AlexNet](https://blog.csdn.net/zzh516451964zzh/article/details/124461111)
- [x] [VGG](https://blog.csdn.net/zzh516451964zzh/article/details/124477080)
- [x] [DenseNet](https://blog.csdn.net/zzh516451964zzh/article/details/124630832)
- [x] [ResNet](https://blog.csdn.net/zzh516451964zzh/article/details/124477575)
- [x] [Wide-ResNet](https://blog.csdn.net/zzh516451964zzh/article/details/124754437)
- [x] [ResNeXt](https://blog.csdn.net/zzh516451964zzh/article/details/124477919)
- [x] [SEResNet](https://blog.csdn.net/zzh516451964zzh/article/details/124478157)
- [x] [SEResNeXt](https://blog.csdn.net/zzh516451964zzh/article/details/124478347)
- [x] [RegNet](https://blog.csdn.net/zzh516451964zzh/article/details/124478426)
- [x] [MobileNetV2](https://blog.csdn.net/zzh516451964zzh/article/details/124478681)
- [x] [MobileNetV3](https://blog.csdn.net/zzh516451964zzh/article/details/124478770)
- [x] [ShuffleNetV1](https://blog.csdn.net/zzh516451964zzh/article/details/124479156)
- [x] [ShuffleNetV2](https://blog.csdn.net/zzh516451964zzh/article/details/124479336)
- [x] [EfficientNet](https://blog.csdn.net/zzh516451964zzh/article/details/124754493)
- [x] [RepVGG](https://blog.csdn.net/zzh516451964zzh/article/details/124479644)
- [x] [Res2Net](https://blog.csdn.net/zzh516451964zzh/article/details/124479467)
- [x] [ConvNeXt](https://blog.csdn.net/zzh516451964zzh/article/details/124481466)
- [x] [HRNet](https://blog.csdn.net/zzh516451964zzh/article/details/124481590)
- [x] [ConvMixer](https://blog.csdn.net/zzh516451964zzh/article/details/124481766)
- [x] [CSPNet](https://blog.csdn.net/zzh516451964zzh/article/details/124481930)
- [x] [Swin-Transformer](https://blog.csdn.net/zzh516451964zzh/article/details/124538198)
- [x] [Vision-Transformer](https://blog.csdn.net/zzh516451964zzh/article/details/124567953)
- [x] [Transformer-in-Transformer](https://blog.csdn.net/zzh516451964zzh/article/details/124596023)
- [x] [MLP-Mixer](https://blog.csdn.net/zzh516451964zzh/article/details/124596093)
- [x] [DeiT](https://blog.csdn.net/zzh516451964zzh/article/details/124591888)
- [x] [Conformer](https://blog.csdn.net/zzh516451964zzh/article/details/124596343)
- [x] [T2T-ViT](https://blog.csdn.net/zzh516451964zzh/article/details/124596425)
- [x] [Twins](https://blog.csdn.net/zzh516451964zzh/article/details/124596619)
- [x] [PoolFormer](https://blog.csdn.net/zzh516451964zzh/article/details/124596740)
- [x] [VAN](https://blog.csdn.net/zzh516451964zzh/article/details/124630541)
- [x] [HorNet](https://arxiv.org/pdf/2207.14284v2.pdf)
- [x] [EfficientFormer](https://arxiv.org/abs/2206.01191)
- [x] [Swin Transformer V2](https://arxiv.org/abs/2111.09883.pdf)
- [x] [MViT V2](http://openaccess.thecvf.com//content/CVPR2022/papers/Li_MViTv2_Improved_Multiscale_Vision_Transformers_for_Classification_and_Detection_CVPR_2022_paper.pdf)

## 预训练权重

| 名称 | 权重 | 名称 | 权重 | 名称 | 权重 |
| :-----: | :-----: | :------: | :------: | :------: | :-----: |
| **LeNet5** | None | **AlexNet** | None | **VGG** | [VGG-11](https://download.openmmlab.com/mmclassification/v0/vgg/vgg11_batch256_imagenet_20210208-4271cd6c.pth)<br/>[VGG-13](https://download.openmmlab.com/mmclassification/v0/vgg/vgg13_batch256_imagenet_20210208-4d1d6080.pth)<br/>[VGG-16](https://download.openmmlab.com/mmclassification/v0/vgg/vgg16_batch256_imagenet_20210208-db26f1a5.pth)<br/>[VGG-19](https://download.openmmlab.com/mmclassification/v0/vgg/vgg19_batch256_imagenet_20210208-e6920e4a.pth)<br/>[VGG-11-BN](https://download.openmmlab.com/mmclassification/v0/vgg/vgg11_bn_batch256_imagenet_20210207-f244902c.pth)<br/>[VGG-13-BN](https://download.openmmlab.com/mmclassification/v0/vgg/vgg13_bn_batch256_imagenet_20210207-1a8b7864.pth)<br/>[VGG-16-BN](https://download.openmmlab.com/mmclassification/v0/vgg/vgg16_bn_batch256_imagenet_20210208-7e55cd29.pth)<br/>[VGG-19-BN](https://download.openmmlab.com/mmclassification/v0/vgg/vgg19_bn_batch256_imagenet_20210208-da620c4f.pth)|
| **ResNet** |[ResNet-18](https://download.openmmlab.com/mmclassification/v0/resnet/resnet18_8xb32_in1k_20210831-fbbb1da6.pth)<br/>[ResNet-34](https://download.openmmlab.com/mmclassification/v0/resnet/resnet34_8xb32_in1k_20210831-f257d4e6.pth)<br/>[ResNet-50](https://download.openmmlab.com/mmclassification/v0/resnet/resnet50_8xb32_in1k_20210831-ea4938fc.pth)<br/>[ResNet-101](https://download.openmmlab.com/mmclassification/v0/resnet/resnet101_8xb32_in1k_20210831-539c63f8.pth)<br/>[ResNet-152](https://download.openmmlab.com/mmclassification/v0/resnet/resnet152_8xb32_in1k_20210901-4d7582fa.pth) | **ResNetV1C** | [ResNetV1C-50](https://download.openmmlab.com/mmclassification/v0/resnet/resnetv1c50_8xb32_in1k_20220214-3343eccd.pth)<br/>[ResNetV1C-101](https://download.openmmlab.com/mmclassification/v0/resnet/resnetv1c101_8xb32_in1k_20220214-434fe45f.pth)<br/>[ResNetV1C-152](https://download.openmmlab.com/mmclassification/v0/resnet/resnetv1c152_8xb32_in1k_20220214-c013291f.pth) |**ResNetV1D** | [ResNetV1D-50](https://download.openmmlab.com/mmclassification/v0/resnet/resnetv1d50_b32x8_imagenet_20210531-db14775a.pth)<br/>[ResNetV1D-101](https://download.openmmlab.com/mmclassification/v0/resnet/resnetv1d101_b32x8_imagenet_20210531-6e13bcd3.pth)<br/>[ResNetV1D-152](https://download.openmmlab.com/mmclassification/v0/resnet/resnetv1d152_b32x8_imagenet_20210531-278cf22a.pth) |
| **ResNeXt** | [ResNeXt-50](https://download.openmmlab.com/mmclassification/v0/resnext/resnext50_32x4d_b32x8_imagenet_20210429-56066e27.pth)<br/>[ResNeXt-101](https://download.openmmlab.com/mmclassification/v0/resnext/resnext101_32x4d_b32x8_imagenet_20210506-e0fa3dd5.pth)<br/>[ResNeXt-152](https://download.openmmlab.com/mmclassification/v0/resnext/resnext152_32x4d_b32x8_imagenet_20210524-927787be.pth) | **SEResNet** | [SEResNet-50](https://download.openmmlab.com/mmclassification/v0/se-resnet/se-resnet50_batch256_imagenet_20200804-ae206104.pth)<br/>[SEResNet-101](https://download.openmmlab.com/mmclassification/v0/se-resnet/se-resnet101_batch256_imagenet_20200804-ba5b51d4.pth)| **SEResNeXt**| None|
| **RegNet** |[RegNetX-400MF](https://download.openmmlab.com/mmclassification/v0/regnet/regnetx-400mf_8xb128_in1k_20211213-89bfc226.pth)<br/>[RegNetX-800MF](https://download.openmmlab.com/mmclassification/v0/regnet/regnetx-800mf_8xb128_in1k_20211213-222b0f11.pth)<br/>[RegNetX-1.6GF](https://download.openmmlab.com/mmclassification/v0/regnet/regnetx-1.6gf_8xb128_in1k_20211213-d1b89758.pth)<br/>[RegNetX-3.2GF](https://download.openmmlab.com/mmclassification/v0/regnet/regnetx-3.2gf_8xb64_in1k_20211213-1fdd82ae.pth)<br/>[RegNetX-4.0GF](https://download.openmmlab.com/mmclassification/v0/regnet/regnetx-4.0gf_8xb64_in1k_20211213-efed675c.pth)<br/>[RegNetX-6.4GF](https://download.openmmlab.com/mmclassification/v0/regnet/regnetx-6.4gf_8xb64_in1k_20211215-5c6089da.pth)<br/>[RegNetX-8.0GF](https://download.openmmlab.com/mmclassification/v0/regnet/regnetx-8.0gf_8xb64_in1k_20211213-9a9fcc76.pth)<br/>[RegNetX-12GF](https://download.openmmlab.com/mmclassification/v0/regnet/regnetx-12gf_8xb64_in1k_20211213-5df8c2f8.pth) | **MobileNetV2** | [MobileNetV2](https://download.openmmlab.com/mmclassification/v0/mobilenet_v2/mobilenet_v2_batch256_imagenet_20200708-3b2dc3af.pth) |**MobileNetV3** | [MobileNetV3-Small](https://download.openmmlab.com/mmclassification/v0/mobilenet_v3/convert/mobilenet_v3_small-8427ecf0.pth)<br/>[MobileNetV3-Large](https://download.openmmlab.com/mmclassification/v0/mobilenet_v3/convert/mobilenet_v3_large-3ea3c186.pth) |
| **ShuffleNetV1** |[ShuffleNetV1](https://download.openmmlab.com/mmclassification/v0/shufflenet_v1/shufflenet_v1_batch1024_imagenet_20200804-5d6cec73.pth) | **ShuffleNetV2** | [ShuffleNetV2](https://download.openmmlab.com/mmclassification/v0/shufflenet_v2/shufflenet_v2_batch1024_imagenet_20200812-5bf4721e.pth) |**EfficientNet** | [EfficientNet-B0](https://download.openmmlab.com/mmclassification/v0/efficientnet/efficientnet-b0_3rdparty_8xb32_in1k_20220119-a7e2a0b1.pth)<br/>[EfficientNet-B1](https://download.openmmlab.com/mmclassification/v0/efficientnet/efficientnet-b1_3rdparty_8xb32_in1k_20220119-002556d9.pth)<br/>[EfficientNet-B2](https://download.openmmlab.com/mmclassification/v0/efficientnet/efficientnet-b2_3rdparty_8xb32_in1k_20220119-ea374a30.pth)<br/>[EfficientNet-B3](https://download.openmmlab.com/mmclassification/v0/efficientnet/efficientnet-b3_3rdparty_8xb32_in1k_20220119-4b4d7487.pth)<br/>[EfficientNet-B4](https://download.openmmlab.com/mmclassification/v0/efficientnet/efficientnet-b4_3rdparty_8xb32_in1k_20220119-81fd4077.pth)<br/>[EfficientNet-B5](https://download.openmmlab.com/mmclassification/v0/efficientnet/efficientnet-b5_3rdparty_8xb32_in1k_20220119-e9814430.pth)<br/>[EfficientNet-B6](https://download.openmmlab.com/mmclassification/v0/efficientnet/efficientnet-b6_3rdparty_8xb32-aa_in1k_20220119-45b03310.pth)<br/>[EfficientNet-B7](https://download.openmmlab.com/mmclassification/v0/efficientnet/efficientnet-b7_3rdparty_8xb32-aa_in1k_20220119-bf03951c.pth)<br/>[EfficientNet-B8](https://download.openmmlab.com/mmclassification/v0/efficientnet/efficientnet-b8_3rdparty_8xb32-aa-advprop_in1k_20220119-297ce1b7.pth) |
| **RepVGG** |[RepVGG-A0](https://download.openmmlab.com/mmclassification/v0/repvgg/repvgg-A0_3rdparty_4xb64-coslr-120e_in1k_20210909-883ab98c.pth)<br/>[RepVGG-A1](https://download.openmmlab.com/mmclassification/v0/repvgg/repvgg-A1_3rdparty_4xb64-coslr-120e_in1k_20210909-24003a24.pth) <br/>[RepVGG-A2](https://download.openmmlab.com/mmclassification/v0/repvgg/repvgg-A2_3rdparty_4xb64-coslr-120e_in1k_20210909-97d7695a.pth)<br/>[RepVGG-B0](https://download.openmmlab.com/mmclassification/v0/repvgg/repvgg-B0_3rdparty_4xb64-coslr-120e_in1k_20210909-446375f4.pth)<br/>[RepVGG-B1](https://download.openmmlab.com/mmclassification/v0/repvgg/repvgg-B1_3rdparty_4xb64-coslr-120e_in1k_20210909-750cdf67.pth)<br/>[RepVGG-A1](https://download.openmmlab.com/mmclassification/v0/repvgg/repvgg-A1_3rdparty_4xb64-coslr-120e_in1k_20210909-24003a24.pth)<br/>[RepVGG-B1g2](https://download.openmmlab.com/mmclassification/v0/repvgg/repvgg-B1g2_3rdparty_4xb64-coslr-120e_in1k_20210909-344f6422.pth)<br/>[RepVGG-B1g4](https://download.openmmlab.com/mmclassification/v0/repvgg/repvgg-B1g4_3rdparty_4xb64-coslr-120e_in1k_20210909-d4c1a642.pth)<br/>[RepVGG-B2](https://download.openmmlab.com/mmclassification/v0/repvgg/repvgg-B2_3rdparty_4xb64-coslr-120e_in1k_20210909-bd6b937c.pth)<br/>[RepVGG-B2g4](https://download.openmmlab.com/mmclassification/v0/repvgg/repvgg-B2g4_3rdparty_4xb64-autoaug-lbs-mixup-coslr-200e_in1k_20210909-7b7955f0.pth)<br/>[RepVGG-B2g4](https://download.openmmlab.com/mmclassification/v0/repvgg/repvgg-B2g4_3rdparty_4xb64-autoaug-lbs-mixup-coslr-200e_in1k_20210909-7b7955f0.pth)<br/>[RepVGG-B3](https://download.openmmlab.com/mmclassification/v0/repvgg/repvgg-B3_3rdparty_4xb64-autoaug-lbs-mixup-coslr-200e_in1k_20210909-dda968bf.pth)<br/>[RepVGG-B3g4](https://download.openmmlab.com/mmclassification/v0/repvgg/repvgg-B3g4_3rdparty_4xb64-autoaug-lbs-mixup-coslr-200e_in1k_20210909-4e54846a.pth)<br/>[RepVGG-D2se](https://download.openmmlab.com/mmclassification/v0/repvgg/repvgg-D2se_3rdparty_4xb64-autoaug-lbs-mixup-coslr-200e_in1k_20210909-cf3139b7.pth)| **Res2Net** | [Res2Net-50-14w-8s](https://download.openmmlab.com/mmclassification/v0/res2net/res2net50-w14-s8_3rdparty_8xb32_in1k_20210927-bc967bf1.pth)<br/>[Res2Net-50-26w-8s](https://download.openmmlab.com/mmclassification/v0/res2net/res2net50-w26-s8_3rdparty_8xb32_in1k_20210927-f547a94b.pth)<br/>[Res2Net-101-26w-4s](https://download.openmmlab.com/mmclassification/v0/res2net/res2net101-w26-s4_3rdparty_8xb32_in1k_20210927-870b6c36.pth)<br/> |**ConvNeXt** | [ConvNeXt-Tiny](https://download.openmmlab.com/mmclassification/v0/convnext/convnext-tiny_3rdparty_32xb128_in1k_20220124-18abde00.pth)<br/>[ConvNeXt-Small](https://download.openmmlab.com/mmclassification/v0/convnext/convnext-small_3rdparty_32xb128_in1k_20220124-d39b5192.pth)<br/>[ConvNeXt-Base](https://download.openmmlab.com/mmclassification/v0/convnext/convnext-base_in21k-pre-3rdparty_32xb128_in1k_20220124-eb2d6ada.pth)<br/>[ConvNeXt-Large](https://download.openmmlab.com/mmclassification/v0/convnext/convnext-large_in21k-pre-3rdparty_64xb64_in1k_20220124-2412403d.pth)<br/>[ConvNeXt-XLarge](https://download.openmmlab.com/mmclassification/v0/convnext/convnext-xlarge_in21k-pre-3rdparty_64xb64_in1k_20220124-76b6863d.pth) |
| **HRNet** |[HRNet-W18](https://download.openmmlab.com/mmclassification/v0/hrnet/hrnet-w18_3rdparty_8xb32_in1k_20220120-0c10b180.pth)<br/>[HRNet-W30](https://download.openmmlab.com/mmclassification/v0/hrnet/hrnet-w30_3rdparty_8xb32_in1k_20220120-8aa3832f.pth) <br/>[HRNet-W32](https://download.openmmlab.com/mmclassification/v0/hrnet/hrnet-w32_3rdparty_8xb32_in1k_20220120-c394f1ab.pth)<br/>[HRNet-W40](https://download.openmmlab.com/mmclassification/v0/hrnet/hrnet-w40_3rdparty_8xb32_in1k_20220120-9a2dbfc5.pth)<br/>[HRNet-W44](https://download.openmmlab.com/mmclassification/v0/hrnet/hrnet-w44_3rdparty_8xb32_in1k_20220120-35d07f73.pth)<br/>[HRNet-W48](https://download.openmmlab.com/mmclassification/v0/hrnet/hrnet-w48_3rdparty_8xb32_in1k_20220120-e555ef50.pth)<br/>[HRNet-W64](https://download.openmmlab.com/mmclassification/v0/hrnet/hrnet-w64_3rdparty_8xb32_in1k_20220120-19126642.pth) | **ConvMixer** | [ConvMixer-768/32](https://download.openmmlab.com/mmclassification/v0/convmixer/convmixer-768-32_3rdparty_10xb64_in1k_20220323-bca1f7b8.pth)<br/>[ConvMixer-1024/20](https://download.openmmlab.com/mmclassification/v0/convmixer/convmixer-1024-20_3rdparty_10xb64_in1k_20220323-48f8aeba.pth)<br/>[ConvMixer-1536/20](https://download.openmmlab.com/mmclassification/v0/convmixer/convmixer-1536_20_3rdparty_10xb64_in1k_20220323-ea5786f3.pth) |**CSPNet** | [CSPDarkNet50](https://download.openmmlab.com/mmclassification/v0/cspnet/cspdarknet50_3rdparty_8xb32_in1k_20220329-bd275287.pth)<br/>[CSPResNet50](https://download.openmmlab.com/mmclassification/v0/cspnet/cspresnet50_3rdparty_8xb32_in1k_20220329-dd6dddfb.pth)<br/>[CSPResNeXt50](https://download.openmmlab.com/mmclassification/v0/cspnet/cspresnext50_3rdparty_8xb32_in1k_20220329-2cc84d21.pth) |
|**Swin Transformer**|[tiny-224](https://download.openmmlab.com/mmclassification/v0/swin-transformer/swin_tiny_224_b16x64_300e_imagenet_20210616_090925-66df6be6.pth)<br/>[small-224](https://download.openmmlab.com/mmclassification/v0/swin-transformer/swin_small_224_b16x64_300e_imagenet_20210615_110219-7f9d988b.pth)<br/>[base-224](https://download.openmmlab.com/mmclassification/v0/swin-transformer/swin_base_224_b16x64_300e_imagenet_20210616_190742-93230b0d.pth)<br/>[large-224](https://download.openmmlab.com/mmclassification/v0/swin-transformer/convert/swin_large_patch4_window7_224_22kto1k-5f0996db.pth)<br/>[base-384](https://download.openmmlab.com/mmclassification/v0/swin-transformer/convert/swin_base_patch4_window12_384_22kto1k-d59b0d1d.pth)<br/>[large-384](https://download.openmmlab.com/mmclassification/v0/swin-transformer/convert/swin_large_patch4_window12_384_22kto1k-0a40944b.pth)|**Vision Transformer**|[vit_base_p16_224](https://download.openmmlab.com/mmclassification/v0/vit/pretrain/vit-base-p16_3rdparty_pt-64xb64_in1k-224_20210928-02284250.pth)<br/>[vit_base_p32_224](https://download.openmmlab.com/mmclassification/v0/vit/pretrain/vit-base-p32_3rdparty_pt-64xb64_in1k-224_20210928-eee25dd4.pth)<br/>[vit_large_p16_224](https://download.openmmlab.com/mmclassification/v0/vit/pretrain/vit-large-p16_3rdparty_pt-64xb64_in1k-224_20210928-0001f9a1.pth)<br/>[vit_base_p16_384](https://download.openmmlab.com/mmclassification/v0/vit/finetune/vit-base-p16_in21k-pre-3rdparty_ft-64xb64_in1k-384_20210928-98e8652b.pth)<br/>[vit_base_p32_384](https://download.openmmlab.com/mmclassification/v0/vit/finetune/vit-base-p32_in21k-pre-3rdparty_ft-64xb64_in1k-384_20210928-9cea8599.pth)<br/>[vit_large_p16_384](https://download.openmmlab.com/mmclassification/v0/vit/finetune/vit-large-p16_in21k-pre-3rdparty_ft-64xb64_in1k-384_20210928-b20ba619.pth)|**Transformer in Transformer**|[TNT-small](https://download.openmmlab.com/mmclassification/v0/tnt/tnt-small-p16_3rdparty_in1k_20210903-c56ee7df.pth)|
|**MLP Mixer**|[base_p16](https://download.openmmlab.com/mmclassification/v0/mlp-mixer/mixer-base-p16_3rdparty_64xb64_in1k_20211124-1377e3e0.pth)<br/>[large_p16](https://download.openmmlab.com/mmclassification/v0/mlp-mixer/mixer-large-p16_3rdparty_64xb64_in1k_20211124-5a2519d2.pth)|**Deit**|[DeiT-tiny](https://download.openmmlab.com/mmclassification/v0/deit/deit-tiny_pt-4xb256_in1k_20220218-13b382a0.pth)<br/>[DeiT-tiny distilled](https://download.openmmlab.com/mmclassification/v0/deit/deit-tiny-distilled_3rdparty_pt-4xb256_in1k_20211216-c429839a.pth)<br/>[DeiT-small](https://download.openmmlab.com/mmclassification/v0/deit/deit-small_pt-4xb256_in1k_20220218-9425b9bb.pth)<br/>[DeiT-small distilled](https://download.openmmlab.com/mmclassification/v0/deit/deit-small-distilled_3rdparty_pt-4xb256_in1k_20211216-4de1d725.pth)<br/>[DeiT-base](https://download.openmmlab.com/mmclassification/v0/deit/deit-base_pt-16xb64_in1k_20220216-db63c16c.pth)<br/>[DeiT-base distilled](https://download.openmmlab.com/mmclassification/v0/deit/deit-base-distilled_3rdparty_pt-16xb64_in1k_20211216-42891296.pth)<br/>[DeiT-base 384px](https://download.openmmlab.com/mmclassification/v0/deit/deit-base_3rdparty_ft-16xb32_in1k-384px_20211124-822d02f2.pth)<br/>[DeiT-base distilled 384px](https://download.openmmlab.com/mmclassification/v0/deit/deit-base-distilled_3rdparty_ft-16xb32_in1k-384px_20211216-e48d6000.pth)|**Conformer**|[Conformer-tiny-p16](https://download.openmmlab.com/mmclassification/v0/conformer/conformer-tiny-p16_3rdparty_8xb128_in1k_20211206-f6860372.pth)<br/>[Conformer-small-p32](https://download.openmmlab.com/mmclassification/v0/conformer/conformer-small-p32_8xb128_in1k_20211206-947a0816.pth)<br/>[Conformer-small-p16](https://download.openmmlab.com/mmclassification/v0/conformer/conformer-small-p16_3rdparty_8xb128_in1k_20211206-3065dcf5.pth)<br/>[Conformer-base-p16](https://download.openmmlab.com/mmclassification/v0/conformer/conformer-base-p16_3rdparty_8xb128_in1k_20211206-bfdf8637.pth)|
|**T2T-ViT**|[T2T-ViT_t-14](https://download.openmmlab.com/mmclassification/v0/t2t-vit/t2t-vit-t-14_8xb64_in1k_20211220-f7378dd5.pth)<br/>[T2T-ViT_t-19](https://download.openmmlab.com/mmclassification/v0/t2t-vit/t2t-vit-t-19_8xb64_in1k_20211214-7f5e3aaf.pth)<br/>[T2T-ViT_t-24](https://download.openmmlab.com/mmclassification/v0/t2t-vit/t2t-vit-t-24_8xb64_in1k_20211214-b2a68ae3.pth)|**Twins**|[PCPVT-small](https://download.openmmlab.com/mmclassification/v0/twins/twins-pcpvt-small_3rdparty_8xb128_in1k_20220126-ef23c132.pth)<br/>[PCPVT-base](https://download.openmmlab.com/mmclassification/v0/twins/twins-pcpvt-base_3rdparty_8xb128_in1k_20220126-f8c4b0d5.pth)<br/>[PCPVT-large](https://download.openmmlab.com/mmclassification/v0/twins/twins-pcpvt-large_3rdparty_16xb64_in1k_20220126-c1ef8d80.pth)<br/>[SVT-small](https://download.openmmlab.com/mmclassification/v0/twins/twins-svt-small_3rdparty_8xb128_in1k_20220126-8fe5205b.pth)<br/>[SVT-base](https://download.openmmlab.com/mmclassification/v0/twins/twins-svt-base_3rdparty_8xb128_in1k_20220126-e31cc8e9.pth)<br/>[SVT-large](https://download.openmmlab.com/mmclassification/v0/twins/twins-svt-large_3rdparty_16xb64_in1k_20220126-4817645f.pth)|**PoolFormer**|[PoolFormer-S12](https://download.openmmlab.com/mmclassification/v0/poolformer/poolformer-s12_3rdparty_32xb128_in1k_20220414-f8d83051.pth)<br/>[PoolFormer-S24](https://download.openmmlab.com/mmclassification/v0/poolformer/poolformer-s24_3rdparty_32xb128_in1k_20220414-d7055904.pth)<br/>[PoolFormer-S36](https://download.openmmlab.com/mmclassification/v0/poolformer/poolformer-s36_3rdparty_32xb128_in1k_20220414-d78ff3e8.pth)<br/>[PoolFormer-M36](https://download.openmmlab.com/mmclassification/v0/poolformer/poolformer-m36_3rdparty_32xb128_in1k_20220414-c55e0949.pth)<br/>[PoolFormer-M48](https://download.openmmlab.com/mmclassification/v0/poolformer/poolformer-m48_3rdparty_32xb128_in1k_20220414-9378f3eb.pth)|
|**DenseNet**|[DenseNet121](https://download.openmmlab.com/mmclassification/v0/densenet/densenet121_4xb256_in1k_20220426-07450f99.pth)<br/>[DenseNet161](https://download.openmmlab.com/mmclassification/v0/densenet/densenet161_4xb256_in1k_20220426-ee6a80a9.pth)<br/>[DenseNet169](https://download.openmmlab.com/mmclassification/v0/densenet/densenet169_4xb256_in1k_20220426-a2889902.pth)<br/>[DenseNet201](https://download.openmmlab.com/mmclassification/v0/densenet/densenet201_4xb256_in1k_20220426-05cae4ef.pth)|**Visual Attention Network(VAN)**|[VAN-Tiny](https://download.openmmlab.com/mmclassification/v0/van/van-tiny_8xb128_in1k_20220501-385941af.pth)<br/>[VAN-Small](https://download.openmmlab.com/mmclassification/v0/van/van-small_8xb128_in1k_20220501-17bc91aa.pth)<br/>[VAN-Base](https://download.openmmlab.com/mmclassification/v0/van/van-base_8xb128_in1k_20220501-6a4cc31b.pth)<br/>[VAN-Large](https://download.openmmlab.com/mmclassification/v0/van/van-large_8xb128_in1k_20220501-f212ba21.pth)|**Wide-ResNet**|[WRN-50](https://download.openmmlab.com/mmclassification/v0/wrn/wide-resnet50_3rdparty-timm_8xb32_in1k_20220304-83ae4399.pth)<br/>[WRN-101](https://download.openmmlab.com/mmclassification/v0/wrn/wide-resnet101_3rdparty_8xb32_in1k_20220304-8d5f9d61.pth)|
|**HorNet**|[HorNet-Tiny](https://download.openmmlab.com/mmclassification/v0/hornet/hornet-tiny_3rdparty_in1k_20220915-0e8eedff.pth)<br/>[HorNet-Tiny-GF](https://download.openmmlab.com/mmclassification/v0/hornet/hornet-tiny-gf_3rdparty_in1k_20220915-4c35a66b.pth)<br/>[HorNet-Small](https://download.openmmlab.com/mmclassification/v0/hornet/hornet-small_3rdparty_in1k_20220915-5935f60f.pth)<br/>[HorNet-Small-GF](https://download.openmmlab.com/mmclassification/v0/hornet/hornet-small-gf_3rdparty_in1k_20220915-649ca492.pth)<br/>[HorNet-Base](https://download.openmmlab.com/mmclassification/v0/hornet/hornet-base_3rdparty_in1k_20220915-a06176bb.pth)<br/>[HorNet-Base-GF](https://download.openmmlab.com/mmclassification/v0/hornet/hornet-base-gf_3rdparty_in1k_20220915-82c06fa7.pth)<br/>[HorNet-Large](https://download.openmmlab.com/mmclassification/v0/hornet/hornet-large_3rdparty_in21k_20220909-9ccef421.pth)<br/>[HorNet-Large-GF](https://download.openmmlab.com/mmclassification/v0/hornet/hornet-large-gf_3rdparty_in21k_20220909-3aea3b61.pth)<br/>[HorNet-Large-GF384](https://download.openmmlab.com/mmclassification/v0/hornet/hornet-base-gf_3rdparty_in1k_20220915-82c06fa7.pth)|**EfficientFormer**|[efficientformer-l1](https://download.openmmlab.com/mmclassification/v0/efficientformer/efficientformer-l1_3rdparty_in1k_20220803-d66e61df.pth)<br/>[efficientformer-l3](https://download.openmmlab.com/mmclassification/v0/efficientformer/efficientformer-l3_3rdparty_in1k_20220803-dde1c8c5.pth)<br/>[efficientformer-l7](https://download.openmmlab.com/mmclassification/v0/efficientformer/efficientformer-l7_3rdparty_in1k_20220803-41a552bb.pth)|**Swin Transformer v2**|[tiny-256 window 8](https://download.openmmlab.com/mmclassification/v0/swin-v2/swinv2-tiny-w8_3rdparty_in1k-256px_20220803-e318968f.pth)<br/>[tiny-256 window 16](https://download.openmmlab.com/mmclassification/v0/swin-v2/swinv2-tiny-w16_3rdparty_in1k-256px_20220803-9651cdd7.pth)<br/>[small-256 window 8](https://download.openmmlab.com/mmclassification/v0/swin-v2/swinv2-small-w8_3rdparty_in1k-256px_20220803-b01a4332.pth)<br/>[small-256 window 16](https://download.openmmlab.com/mmclassification/v0/swin-v2/swinv2-small-w16_3rdparty_in1k-256px_20220803-b707d206.pth)<br/>[base-256 window 8](https://download.openmmlab.com/mmclassification/v0/swin-v2/swinv2-base-w8_3rdparty_in1k-256px_20220803-8ff28f2b.pth)<br/>[base-256 window 16](https://download.openmmlab.com/mmclassification/v0/swin-v2/swinv2-base-w16_3rdparty_in1k-256px_20220803-5a1886b7.pth)<br/>[large-256 window 16](https://download.openmmlab.com/mmclassification/v0/swin-v2/swinv2-large-w16_in21k-pre_3rdparty_in1k-256px_20220803-c40cbed7.pth)<br/>[large-384 window 24](https://download.openmmlab.com/mmclassification/v0/swin-v2/swinv2-large-w24_in21k-pre_3rdparty_in1k-384px_20220803-3b36c165.pth)|
|**HorNet**|[MViTv2-Tiny](https://download.openmmlab.com/mmclassification/v0/mvit/mvitv2-tiny_3rdparty_in1k_20220722-db7beeef.pth)<br/>[MViTv2-Small](https://download.openmmlab.com/mmclassification/v0/mvit/mvitv2-small_3rdparty_in1k_20220722-986bd741.pth)<br/>[MViTv2-Base](https://download.openmmlab.com/mmclassification/v0/mvit/mvitv2-base_3rdparty_in1k_20220722-9c4f0a17.pth)<br/>[MViTv2-Large](https://download.openmmlab.com/mmclassification/v0/mvit/mvitv2-large_3rdparty_in1k_20220722-2b57b983.pth)|

## 参考
```
@repo{2020mmclassification,
    title={OpenMMLab's Image Classification Toolbox and Benchmark},
    author={MMClassification Contributors},
    howpublished = {\url{https://github.com/open-mmlab/mmclassification}},
    year={2020}
}
```
