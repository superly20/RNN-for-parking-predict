# RNN-for-parking-predict

把数据分为训练数据和测试数据

75%为训练数据 and 25%为测试数据

参数定义

lstm_size：在一个LSTM训练里的cell的个数

num_layers：一个cell里隐藏层的个数

keep_prob：

init_learning_rate：

learning_rate_decay：

max_epoch：总共需要训练几遍（当一个完整的数据集通过了神经网络一次并且返回了一次，这个过程称为一个epoch）随着epoch数量增加，神经网络中的权重的更新次数也增加，曲线从欠拟合变得过拟合。

init_epoch：

batch_size：数据分为几批去训练

input_size：每个窗口里面包含几个数据/一个训练数据点

num_steps：使用几个窗口去预测下一个窗口
