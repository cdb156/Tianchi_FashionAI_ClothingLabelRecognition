# attribute recognition
这个比赛当时和杭电的陶星一起组队的。一段很棒的经历，水平提升不少。最终排名：7/2950

比赛总结：https://blog.csdn.net/hzh_0000/article/details/81149268

最近在找工作，可能代码有些多余的东西也没有时间删除，pytorch来训练模型的话，最关键的几部分代码就是，创建model（在getmodel里面），然后构建数据加载器（dataloader里面），然后就是train.py里面训练就行了。
#### 环境
`pytorch`, #版本0.3.0or0.3.1

`tensorboard_logger`, #log信息

`pretrainedmodels`, #预训练模型库

`argparse`,
`PIL`

#### 1.目录
文件目录：
```

```
#### 2.准备数据
将`训练集`，`测试集`，`热身数据`分别放入`base`,`rank`,`web`

运行prepare_data.py进行数据划分
#### 3.训练
`main.py` #`--arch`为模型名称，不同预训练模型在最后一层不一样，需要调试修改

`train.sh` #训练脚本
#### 4.生成csv
`evaluate.py` #`arc_lists`为待测试模型
#### 5.结果平均
`average.ipynb`
