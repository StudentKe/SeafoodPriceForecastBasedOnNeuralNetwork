# TensorFlow - SeafoodPriceForecastBasedOnNeuralNetwork

## 用神经网络实现的海鲜价格预测

### 因为没有合适的数据集 故伪造了数据集
- 价格随月份波动
- 价格随运送距离波动
- 价格随产品的鲜活度波动
- 价格随人口密度波动
- 价格随城市消费水平波动
- ..

### 文件结构
- `forward.py `
   - 搭建网络向前传播的过程
   - 定义网络结构
     - 输入层 5 
     - 隐藏层1 5
     - 隐藏层2 5
     - 输出层 1
- `backwar.py`
  - 搭建网络向后传播过程
  - 指定优化参数
    - 正则化参数
    - 滑动平均
    - 学习率
    - 损失函数
  - 执行训练过程并计算模型损失
- `test.py`
  - 测试模型准确度
- `input_data.py`
  - 读取数据
  - 返回数据对象

- [x] 使用神经网络实现预测
- [x] 重构`input_data.py`
- [x] 选取另一种算法对比效果
- [x] 图表展示
- [x] 留出接口，对接主程序
