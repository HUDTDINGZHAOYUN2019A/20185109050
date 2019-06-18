
# 高晋超组作业
网络图片的文本识别的代码实现

## 实验目的
本文将具体介绍如何利用Python的图像处理模块pillow和OCR模块pytesseract来识别上述验证码（数字加字母）。

## 实验步骤
我们识别上述验证码的算法过程如下：
1.首先我们先将原图像进行灰度处理，就是我们所选择的验证码图片转化为灰度图像；
2.然后获取图片中像素点数量最多的像素（此为图片背景），以此图片像素设置阈值，采用扫描的方法消除图像中差值小于阈值的颜色，对此图像进行二值化处理，将灰度图像转化为黑白图像（用来提高识别的准确率）；
3.利用pytesseract模块识别，去掉识别结果中的特殊字符，获得识别结果。







