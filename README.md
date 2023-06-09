# learn-dl-with-pytorch

### FCN语义分割模型（Fully Convolutional Networks for Semantic Segmentation)
- 语义分割是基于像素级别的处理图像方式，自动从图像中识别对象区域与对象区域的类别。
- 论文：https://arxiv.org/pdf/1411.4038.pdf
- FCN提出所追求的是，输入是一张图片，输出也是一张图片，学习像素到像素的映射。
- FCN对图像FCN则是从抽象的特征中恢复出每个像素所属的类别。即从图像级别的分类进一步延伸到像素级别的分类。FCN对图像进行像素级别的分类，从而解决了语义级别的图像分割(Semantic segmentation)问题。
- FCN可以接受任意尺寸的输入图像，采用反卷积层对最后一个卷积层的Feature map进行上采样，使得它恢复到输入图像相同的尺寸。
