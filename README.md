由于网络原因，hugging face 的模型是无法下载的，所以要修改 https://github.com/douseful/CheXbert/blob/3ab882dbb14dd365ba0e122cc85b1ce592f20c60/src/models/bert_labeler.py#L22C67-L22C67 中的代码，提前下载好模型与 config.json，修改为下载好的文件所在的**目录（不是文件名）**

同时 修改 torch 版本为较新版本 
```
conda install pytorch==1.7.0 torchvision==0.8.0 torchaudio==0.7.0 cudatoolkit=11.0 -c pytorch
```
