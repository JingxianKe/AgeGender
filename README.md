# 年龄性别分类器

年龄性别分类

使用[OUI-Adience dataset](https://talhassner.github.io/home/projects/Adience/Adience-data.html)，预训练的Resnet50和MobilenetV3模型

最终精度：性别96.94%，年龄78.79% (resnet50)；性别96.12%，年龄82.12% (mobilenet_v3)

MobilenetV3实现源自[pytorch-image-models](https://github.com/rwightman/pytorch-image-models)


预训练模型：
* resnet50: to-be-published
* mobilenetv3: [link](https://yadi.sk/d/zUYVP-y8aQ14Hw) 

模型输入图像大小224x224，输出age_logits (bs x 8), gender_logits (bs x 3)
age logits——0-2, 3-6, 8-13, 15-20, 22-32, 34-43, 45-53, 55-100的8组中每组的图像概率
