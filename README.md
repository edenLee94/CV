### Computer Vision

컴퓨터 비전 관련된 논문 리뷰 및 코드 구현
* 최신 논문 위주로, 많은 인기를 끌고 있는 다양한 딥러닝 논문을 소개합니다.

#### CV 분야 논문
* Histograms of Oriented Gradients for Human Detection(HOG)
    * [Original Paper Link](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=1467360&tag=1) / Contents / Code Practice
* GradientBased Learning Applied to Document Recognition(LeNet)
    * [Original Paper Link](http://vision.stanford.edu/cs598_spring07/papers/Lecun98.pdf) / Contents /[Code Practice](https://github.com/edenLee94/CV/blob/main/Paper/LeNet/LeNet.ipynb)
* ImageNet Classification with Deep Convolutional Neural Networks(AlexNet)
    * [Original Paper Link](https://proceedings.neurips.cc/paper/2012/file/c399862d3b9d6b76c8436e924a68c45b-Paper.pdf) / [Contents](https://github.com/edenLee94/CV/blob/main/Paper/AlexNet/Readme.md) / [Code Practice](https://github.com/edenLee94/CV/blob/main/Paper/AlexNet/AlexNet_pr.ipynb)
* Very Deep Convolution Networks for Large-scale image recognition(VGG)
    * [Original Paper Link](https://arxiv.org/pdf/1409.1556.pdf%20http://arxiv.org/abs/1409.1556.pdf) / [Contents](https://github.com/edenLee94/CV/blob/main/Paper/VGG/Readme.md) / [Code Practice](https://github.com/edenLee94/CV/blob/main/Paper/VGG/vgg.py)
* Going deeper with convolutions(GoogLeNet)
    * [Original Paper Link](https://arxiv.org/pdf/1409.4842.pdf) / [contents](https://github.com/edenLee94/CV/blob/main/Paper/GoogLeNet/Readme.md) / [Code Practice](https://github.com/edenLee94/CV/blob/main/Paper/GoogLeNet/_GoogLeNet_pr.ipynb)
* Deep Residual Learning for Image Recognition(ResNet)
    * [Original Paper Link](https://arxiv.org/pdf/1512.03385.pdf) / [contents](https://github.com/edenLee94/CV/blob/main/Paper/ResNet/Readme.md) / [Code Practice](https://github.com/edenLee94/CV/blob/main/Paper/ResNet/ResNet_50.ipynb) / [cat vs dog dataset:resnet50 클래스 분류하기 및 cv2에 대한 내용](https://github.com/edenLee94/CV/blob/main/resnet_classfication_catvsdog.ipynb)
* Squeeze-and-Excitation Networks(SENet)
    * [Original Paper Link](https://arxiv.org/pdf/1709.01507v4.pdf) / [contents](https://github.com/edenLee94/CV/blob/main/Paper/SENet/Readme.md) / [Code Practice](https://github.com/edenLee94/CV/blob/main/Paper/SENet/add_SE_module.py)
* EfficientNet, Rethinking Model Scaling for Convolutional Neural Networks(EfficientNet)
    * [Original Paper Link](https://arxiv.org/pdf/1905.11946.pdf) / [contents](https://github.com/edenLee94/CV/blob/main/Paper/EfficientNet/Readme.md) / Code Practice
    
#### object detection
* R-CNN / Fast R-CNN / Faster R-CNN
    * [Original Paper Link-basic model: R-CNN](https://arxiv.org/pdf/1311.2524.pdf) / [contents](https://github.com/edenLee94/CV/blob/main/Paper/R%20CNN/read.md)
- YOLO

#### GAN에서 발전한 논문
* Generative Adversarial Networks(GAN)
    * [Original Paper Link](https://arxiv.org/pdf/1406.2661.pdf) / [contents] / [Code Practice](https://github.com/edenLee94/CV/blob/main/GAN.ipynb)
* Interpretable Representation Learning by Information Maximizing Generative Adversarial Nets(InfoGAN)
    * [Original Paper Link](https://arxiv.org/pdf/1606.03657.pdf) / [contents] / [Code Practice]
* Unpaired Image-to-Image Translation using Cycle-Consistent Adversarial Networks(CycleGAN)
    * [Original Paper Link](https://arxiv.org/pdf/1606.03657.pdf) / [contents] / [Code Practice]
* PROGRESSIVE GROWING OF GANS FOR IMPROVED QUALITY, STABILITY, AND VARIATION(Progressive Growing of GANS(PGGAN))
    * [Original Paper Link](https://arxiv.org/pdf/1710.10196.pdf) / [contents] / [Code Practice]
- VAE
- MobileNet-v1.v2.v3

#### Image Recognition (이미지 인식)
* 이미지와 질문이 주어졌을 때 답을 맞추는 Visual QnA
    * Original Paper Link / contents / Code Practice
* 이미지를 설명하는 문장을 만들어내는 Image Captioning
    * [Original Paper Link](https://arxiv.org/pdf/1411.4555v2.pdf) / contents / Code Practice
* Neural Image Caption Generation with visual Attention
    * Original Paper Link / contents / Code Practice
* Image Captioning with Semantic Attention
    * [Original Paper Link](https://www.cv-foundation.org/openaccess/content_cvpr_2016/papers/You_Image_Captioning_With_CVPR_2016_paper.pdf) / contents / Code Practice  
 
-----
ImageNet(large-scale), MNIST, CIFAR dataset
MNIST나 CIFAR는 idea에 대한 검증 목적으로 사용
- MNIST: 0부터 9까지의 '28 x 28 손글씨 사진'을 모은 데이터셋 (학습용: 60,000개 / 테스트용: 10,000)
- CIFAR-10: 10개의 클래스로 구분된 '32 x 32 사물 사진'을 모은 데이터셋 (학습용: 50,000개 / 테스트용: 10,000개)
- ImageNet : (Amazon Mechanical Turk) 서비스를 이용하여 일일이 사람이 분류한 데이터셋


### 파일 설명
#### > overfitting을 극복하는 방법
overfitting을 극복하는 방법으로는 data augmentation, batch normalization, drop out이 있다. 이를 통해서 얼마나 고쳐지는지 확인한다. [code](https://github.com/edenLee94/CV/blob/main/Solution_overfitting.ipynb)

#### > CNN_cifar10.ipynb
https://tutorials.pytorch.kr/beginner/basics/optimization_tutorial.html

pytorch에서 제공한 tutorials에서 제공하는 설정을 이용해서 신경망 설계 및 최적화 코드를 반복하여 수행하는 train와 테스트 데이터로 모델의 성능을 측정하는 evaluate를 정의!
GPU 설정을 '펭귄브로의 3분 딥러닝, 파이토치맛' 책의 내용을 학습해서 진행하였다.
