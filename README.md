# StrokeBasedRNN
Codes for paper : "A Stroke-based RNN for Writer-Independent Online Signature Verification" 

# 运行指南
- mobisig.7z为初始数据集的压缩包   
- 制作数据集
``` python
 python dataset/processor_mobisig.py

```
上面两个脚本需要关注的主要有数据集的原始路径和输出路径.我这里给出的mobisig文件夹是原始的数据集，后缀带有_processed的文件夹是处理之后的数据集（mobisig_processed.7z为压缩后的数据集）

- 运行训练文件
``` python
tar zxvf no_encoder.tar.gz
python run_run.py 
```
如果需要用预训练的权重，解压 no_encoder.tar.gz，训练中需要关注dataset/params.json这个文件，里面包含里训练相关的配置