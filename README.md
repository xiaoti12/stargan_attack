# 关键py代码

## main.py

包括了所有命令行参数及其默认值

## dataloader.py

数据集图片的读取、排序、预处理

## solver.py（重要）

`test_attack`方法里是整个加噪音的过程，包括读取预训练模型、遍历数据集图片及属性、添加噪音并篡改、保存图片、计算`L1_ERROR`和`L2_ERROR`值等步骤

# 其他重要结构

## data文件夹

数据集，其中`list_attr_celeba`文件用于存放数据集图片的属性及其赋值，用1或-1表示

## stargan_celeba_256文件夹

`models`文件夹用于存放预训练模型（只提供了5个可保护属性），`results`文件夹用于存放生成的图片

# P.S.

我的代码是根据项目调整过的，建议先跑原始的代码，然后自己再研究代码功能

