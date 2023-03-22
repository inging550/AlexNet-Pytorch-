# AlexNet-Pytorch
使用的Pytorch版本为1.7.1,经过测试1.11.0也可以正常运行，对应的博客地址为：https://blog.csdn.net/ing100/article/details/129519614 

此代码对应的Libtorch（C++）版本的博客地址为：\
https://blog.csdn.net/ing100/article/details/129621206 

以及Libtorch实现的代码地址为：\
https://github.com/inging550/AlexNet-Libtorch-
    
博客中的0~9手写数据集下载地址：\
链接：https://pan.baidu.com/s/1-THA3tu7NHzyoS5ZIFv0Tw\
提取码：1234

## 训练方法: (修改train.py)
1、准备好数据集（可以在上面下载，或者使用自己的数据集），数据集的摆放方式请参考博客 \
2、根据数据集的位置更改dataset的路径 ，对应代码27，28行 \
3、在定义网络结构处更改NUM_CLASS的值(数据集所含类别总数)，在第35行 \
4、运行train.py \
5、 训练完成后结果保存为AlexNet.pth文件，对应代码最后一行

## 预测方法:（修改predict.py）
1、修改img_root（带预测的图片路径），在第9行 \
2、修改 NUM_CLASS（数据集类别总数），第10行 \
3、修改列表labels_name，在第15行 \
4、 运行predict.py \
在此文件中我还附上了绘制混淆矩阵的方法，只需要将代码83行之后的注释全部清除即可（运行会花费一定时间）
