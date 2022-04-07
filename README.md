## 软件功能说明

![](https://github.com/liuhao1946/Nordic-app-Log-conversion-tool/blob/master/image/%E8%BD%AF%E4%BB%B6%E6%88%AA%E5%9B%BE.jpg)

该软件用于从Nordic App保存的Log文件中提取由MCU端发送的字符串数据，具有有以下功能：

* 提取原始log文件中由MCU发出的字符内容
* 提取可以选择以txt或者csv格式保存（默认csv格式）
* 可选是否包含原始log中的时间戳信息
* 检查SN，统计掉包信息

## 软件使用说明

* 如果以csv格式保存提取后的文件，要求MCU端发送的数据需要符合csv格式。比如：
  > (序列号，数据，数据)
  
  > 123,70,60
  
  > 124,70,60
  
  > 125,70,60

* 如果以txt格式保存提取后的文件，MCU可以发送任意格式的字符串数据
  
* 检查SN目前只用于csv格式文件

* 勾上**包含时间戳**，软件除了提取原始log外，还会附带由App产生的时间戳，比如勾上时间戳，以csv格式保存提取后的文件
  > （时间戳，序号，数据，数据）


  > 15:01:23.525,123,70,60
