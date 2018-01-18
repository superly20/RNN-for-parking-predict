# RNN-for-parking-predict

把数据分为训练数据和测试数据

75%为训练数据 and 25%为测试数据


参数定义

lstm_size：在一个LSTM训练里的输入输出的个数

num_layers：一个输入输出中间包含cell的个数

keep_prob：用于dropout.每批数据输入时神经网络中的每个单元会以1-keep_prob的概率不工作，可以防止过拟合

init_learning_rate：学习速率,在循环次数超过init_epoch以后会逐渐降低

learning_rate_decay：学习速率衰减（epoch>init_epoch时,decay逐渐减小）

max_epoch：整个数据集循环次数（当一个完整的数据集通过了神经网络一次并且返回了一次，这个过程称为一个epoch）随着epoch数量增加，神经网络中的权重的更新次数也增加，曲线从欠拟合变得过拟合。

init_epoch：设定一个临界值，epoch<init_epoch时，decay值=1,epoch>init_epoch时，decay逐渐减小

batch_size：每批数据的规模，有多少数据（调整是为了在内存效率和内存容量之间寻找最佳平衡，适当的增加会使梯度下降方向准确度增加，训练震动的幅度减小）

input_size：每个窗口里面包含几个数据

num_steps：使用几个窗口去预测下一个窗口

