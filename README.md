# 语音转换展示应用

## 简介

应用的架构如下：

+ 网页页面：
  
  + 用户在页面中选择发音人，目前有两个可选项；
  + 用户在页面中决定开始和结束时刻；
  
+ 蓝牙设备：
  
  + 录制音频和播放音频一体音频设备。
  + 当用户点击「开始」时，设备开始录制音频；
  + 当用户点击「结束」时，设备结束录制；同时，在 1s 后，设备将播放转化后的音频。

+ 推理部分：
  
  + 当用户点击「开始」时， 录制音频流开始工作，并储存相关的音频信息；
  + 当用户点击「结束」时，停止储存音频信息，并将存储的数据传给推理函数进行音频转化。

应用的加载时间：

+ 初始化应用（重启）：8s 左右。
+ 推理：
  + 初次推理：1s - 2s；
  + 复用推理：1s 以内。
+ 点击「开始」到程序启动的延迟： 1s - 5s 之间。

## 使用说明

1. 设置好蓝牙设备；
2. 在桌面选中「运行语音转化.sh」；
3. 双击即可执行。

注1：如按此法无法打开该文件，执行一下步骤：

  1. 选中·运行语音转化.sh」并右键；
  2. 鼠标移动至「打开方式(H)」，单击「Git for Windows」；
  3. 程序即可运行。

注2：蓝牙设备使用说明：

  1. 将 3.55mm 接口与接收器组装；
  2. 启动接收器与麦克风，待接收器与麦克风的指示灯常亮为蓝色后（配对成功）进行下一步，否则重复该步骤；
  3. 将组装好的接口插入电脑的「麦克风」接口，机箱上方接口或机箱背后的音响线内侧接口。
  4. 使用结束后，将设备取下并放入盒中进行充电。
  