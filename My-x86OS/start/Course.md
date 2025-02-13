# 课程笔记

## 四、引导程序：接管控制权

### 计算机启动流程简介

![01 boot](img\4_boot\01 boot.png)

### 接管运行控制权

![02 Mechanical hard drive](img\4_boot\02 Mechanical hard drive.png)

![03 Hard disk](img\4_boot\03 Hard disk.png)

![04 Solid State Disk](img\4_boot\04 Solid State Disk.png)

![05 boot 0x7c00](img\4_boot\05 boot 0x7c00.png)

BIOS会检查第0个扇区最后两个字节（1FE和1FF）是否为0x55和0xAA，否则则判定为不可引导的磁盘。此时只考虑硬盘只有一个分区的情况，若有多个分区则需要使用主引导记录（MBR）。

### 创建可引导的启动程序

![06 Project Structure](img\4_boot\06 Project Structure.png)

![07 Development workflow](img\4_boot\07 Development workflow.png)

### 初始化引导程序

![08 boot program](img\4_boot\08 boot program.png)

![09 boot 0x7c00 0x55 0xaa](img\4_boot\09 boot 0x7c00 0x55 0xaa.png)

![10 boot and loader](img\4_boot\10 boot and loader.png)

![11 x86 Real mode](img\4_boot\11 x86 Real mode.png)

![12 Kernel register](img\4_boot\12 Kernel register.png)

![13 Segment Registers](img\4_boot\13 Segment Registers.png)

![14 memory-mapped](img\4_boot\14 memory-mapped.png)
