# 课程笔记

## 四、引导程序：接管控制权

### 4.1 计算机启动流程简介

![4.1 boot](img\4.1 boot.png)

### 4.2 接管运行控制权

![Mechanical hard drive](img\4.2 Mechanical hard drive.png)

![Hard disk](img\4.2 Hard disk.png)

![Solid State Disk](img\4.2 Solid State Disk.png)

![4.2 boot 0x7c00](img\4.2 boot 0x7c00.png)

BIOS会检查第0个扇区最后两个字节（1FE和1FF）是否为0x55和0xAA，否则则判定为不可引导的磁盘。此时只考虑硬盘只有一个分区的情况，若有多个分区则需要使用主引导记录（MBR）。

### 4.3 创建可引导的启动程序

![4.3 Project Structure](img\4.3 Project Structure.png)

![4.3 Development workflow](img\4.3 Development workflow.png)
