# Signal-preprocessing

把BJUT、CWRU、IMS三个数据集划分成2048长度的样本，和（2048，256）的CWT矩阵

2048信号 reshape to (2048,1), （64，64）矩阵的压缩为：（64，64），reshape to (64*64,1)=（4096，1）

拼接成：（2048+4096，1），并保存为csv文件

BJUT:20kHz @ 18_mN、18_0N、15_mN、15_0N @ NC、OF1、IF1、RF1、OF2、IF2、RF2

CWRU:12kHz @ 0HP、1HP、2HP、3HP @ NC、OF1、IF1、RF1、OF2、IF2、RF2、OF3、IF3、RF3

IMS: 20kHz @ 2000RPM+26.6kN @ NC、OF1、IF1、RF1
