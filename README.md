# 基于TensorFlow Lite实现的Android花卉识别应用
## 一、下载初始代码
1、访问 https://github.com/hoitab/TFLClassify.git 网站，下载初始代码ZIP包，解压到自己的工作目录中（目录下不能有中文字符）
![图片文字描述](图片链接)
2、打开Android Studio，打开该项目，第一次运行会下载相应的Gradle，稍微等待即可（需要手机通过USB连接，这里我未使用手机而是模拟器，则会显示以下图片）

## 二、向应用中添加TensorFlow Lite
1、在"start"模块右键选择File，然后New>Other>TensorFlow Lite Model，选择finish模块中ml文件下的FlowerModel.tflite，点击完成后系统会自动下载依赖至文件中

2、成功导入后，生成摘要信息

## 三、检查代码中的TODO项，添加代码重新运行APP
1、在“start”模块的MainActivity.kt文件的TODO 1中添加初始化训练模型的代码

2、在CameraX的analyze方法内部，将摄像头的输入ImageProxy转化为Bitmap对象，并进一步转化为TensorImage 对象

3、对图像进行处理并生成结果，按照属性score对识别结果按照概率从高到低排序并列出最高k种可能的结果

4、将识别的结果加入数据对象Recognition中

5、将原先用于虚拟显示识别结果的代码注释掉或者删除

## 四、以物理设备重新运行start模块
