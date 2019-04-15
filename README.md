# openCamera
## Mac OS 安装 OpenCV
> Python 环境为 python3

终端执行如下指令：
```
# 安装opencv及其依赖包
brew install opencv3
```
brew install opencv3 用来指明安装python3版本的opencv。
```
# 链接opencv
brew link --force opencv3
```
这个指令执行后，报错后面执行程序也不会出现太大的问题的。
## 安装后测试
终端执行如下指令：
```
# 进入python3交互模式
python3

# 导入cv2模块
import cv2
```
若是没有报错，那么你便安装成功了。
## python3脚本打开摄像头
终端进入脚本目录后执行如下指令：
```
# 运行脚本
python3 open_camera.py
```
mac 此时会提示你允许terminal访问摄像头，同意。
若第一次提示失败的话，是因为授权问题，再来一次就ok了。
## 脚本代码解释
```
# openCV自带函数创建摄像头对象，0表示第一个摄像头
cap = cv2.VideoCapture(0)
```
## 参考
- https://blog.csdn.net/willduan1/article/details/53898440
- https://blog.csdn.net/huanglu_thu13/article/details/52337013