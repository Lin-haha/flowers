# 基于TensorFlow Lite实现的Android花卉识别应用
## 一、下载初始代码
1、访问 https://github.com/hoitab/TFLClassify.git 网站，下载初始代码ZIP包，解压到自己的工作目录中（目录下不能有中文字符）

2、打开Android Studio，打开该项目，第一次运行会下载相应的Gradle，稍微等待即可（需要手机通过USB连接，这里我未使用手机而是模拟器，则会显示以下图片）

## 二、向应用中添加TensorFlow Lite
1、在"start"模块右键选择File，然后New>Other>TensorFlow Lite Model，选择finish模块中ml文件下的FlowerModel.tflite，点击完成后系统会自动下载依赖至文件中

2、成功导入后，生成摘要信息

## 三、检查代码中的TODO项
