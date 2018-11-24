## Tensorflow中基于检索的会话模型（Ubuntu 对话语料）

#### Overview

本项目代码采用双LSTM编码器基于Ubuntu对话语料实现了一款智能聊天机器人
[The Ubuntu Dialogue Corpus: A Large Dataset for Research in Unstructured Multi-Turn Dialogue Systems](http://arxiv.org/abs/1506.08909).

#### 环境

代码使用 Python 3 + Tensorflow >= 0.9. 运行本代码需要安装以下 packages:

```
pip install -U pip
pip install numpy scikit-learn pandas jupyter
```

#### 获取数据


下载数据集 train/dev/test data [here](https://drive.google.com/open?id=0B_bZck-ksdkpVEtVc1R6Y01HMWM) and extract the acrhive into `./data`.


#### 训练

```
python udc_train.py
```


#### 验证

```
python udc_test.py --model_dir=...
```


#### 预测

```
python udc_predict.py --model_dir=...
```
