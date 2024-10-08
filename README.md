# 基于PYQT5和图像处理算法的智能美颜相机

## 1、简介：

本项目是一款基于PYQT5和图形图像处理算法的智能美颜相机，利用图像处理等技术，实现了美颜、滤镜、增强等功能，能够给用户提供更好的使用体验。

## 2、具体功能：

- 首先利用人脸识别模型检测输入图像中的人脸位置。借助dlib人脸关键特征点，应用程序能够准确地定位人脸的关键部位，如眼睛、嘴巴等。
- 滤镜功能使用户能够通过应用各种滤镜效果改变图像的外观。用户可以选择不同的滤镜样式，如怀旧、铅笔画、哈哈镜等，以实现不同的艺术效果。
- 增强功能提供了调整图像属性的选项。用户可以增加亮度、对比度、饱和度等，以改善图像的质量和视觉效果。
- 美颜功能是该应用程序的亮点之一。通过应用各种图像处理技术，如美白、磨皮、瘦脸和大眼。
- 涂鸦功能为用户提供了自由绘制的能力。他们可以在图像上绘制椭圆、矩形等，为照片增添创意和个性。
- 贴纸功能允许用户添加各种贴纸或装饰物到图像上。用户可以选择喜欢的贴纸，如比心、飞机等，以增加图像的趣味性和个性化。
- 文字功能允许用户在图像上添加自定义文本。他们可以添加标题、标签、注释或个性化的文字消息，以传达特定的信息或增强照片的表达力。
- 马赛克功能可以用于模糊图像。用户可以选择马赛克效果来隐藏敏感信息或保护隐私。 

此外，美颜相机还支持摄像头拍照功能，这提供了便捷的方式来捕捉美丽的瞬间，为后面的美颜操作提供便利。同时，美颜相机提供了图片缩放、撤销还原等实用功能，使用户能够调整图像的大小和恢复到之前的状态。核心功能如图所示。

<img width="880" alt="1" src="https://github.com/user-attachments/assets/243e7dfa-b935-453b-9ad5-ad073353f06f">

## 3、环境

cmake               3.26.3
colorama            0.4.6
contourpy           1.0.7
cycler              0.11.0
dlib                19.24.1
imageio             2.28.1
importlib-resources 5.12.0
mdurl               0.1.2
mmengine            0.7.3
mpmath              1.3.0
PyQt5               5.15.9
pyqt5-plugins       5.15.9.2.3
PyQt5-Qt5           5.15.2
PyQt5-sip           12.12.1
pyqt5-tools         5.15.9.3.3
PyQt5Designer       5.14.1
python-dateutil     2.8.2
python-dotenv       1.0.0
qt5-applications    5.15.2.2.3
qt5-tools           5.15.2.1.3

具体见requirements.txt

## 4、QT Designer

QT Designer 是一个可视化的界面设计工具，能够以图形化方式创建和编辑QT应用程序的用户界面。通过使用QT Designer，我们可以以可视化的方式设计和编辑界面，减少了手动编写界面代码的工作量，并提供了一个直观和易于使用的界面设计体验。因此，在美颜相机的开发中我们采用了QT Designer进行界面的设计与美化。QT Designer设计界面和最终的效果图如图所示。

<img width="1001" alt="2" src="https://github.com/user-attachments/assets/9fef92d2-0501-4d30-93cc-ac01da9c9c12">

<img width="723" alt="3" src="https://github.com/user-attachments/assets/428a203a-5dca-4dbc-abd0-7fba16a490ce">

## 5、Dlib人脸关键特征点检测

人脸关键点定位技术是对人脸中眉毛、眼睛、鼻子、嘴巴以及脸部的轮廓进行定位。包括基于特征点检测（支持向量机、随机森林）、基于模型拟合（ASM-主动形状模型、AAM-主动外观模型）和基于深度学习的方法等等。目前最通用的方案是68点标注，即opencv中的Dlib库所采用的方案，它将人脸关键点分为内部关键点和轮廓关键点，内部关键点包含51个关键点，轮廓关键点包含17个关键点，如图所示。

<img width="583" alt="5" src="https://github.com/user-attachments/assets/c1c2ce77-ddae-45a2-a681-e3b3efd0adb7">

注：dlib人脸68点特征点检测模型官网下载地址：http://dlib.net/files/shape_predictor_68_face_landmarks.dat.bz2

## 6、例图

<img width="472" alt="6" src="https://github.com/user-attachments/assets/712fdf22-38aa-4566-8346-5ae710bd46b5">

<img width="474" alt="7" src="https://github.com/user-attachments/assets/2eaca40f-cc65-481d-809d-b2f36e1325e8">

<img width="470" alt="8" src="https://github.com/user-attachments/assets/e3686578-4f47-4f64-8ad8-69760d602257">

<img width="472" alt="9" src="https://github.com/user-attachments/assets/3e618151-4088-4268-ac77-a47403fbb6b9">

<img width="475" alt="10" src="https://github.com/user-attachments/assets/0ae1a08e-12ac-4ee8-88cb-ebafa6ccc39b">
