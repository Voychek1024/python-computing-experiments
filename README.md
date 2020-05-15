# 实验三 Python函数定义与面向对象程序设计

## 导航

[返回](https://github.com/ZKLlab/python-computing-experiments)

## 实验要求

1. 函数和数据结构复习
   1. 编写Ackermann函数的递归实现Ack(m, n)；

      ![Ackermann函数](https://render.githubusercontent.com/render/math?math=A%5Cleft%28m%2Cn%5Cright%29%3D%5Cleft%5C%7B%5Cbegin%7Barray%7D%7Bll%7Dn%2B1%26%5Crm%7Bif%7D%5C%3Bm%3D0%5C%5CA%5Cleft%28m-1%2C1%5Cright%29%26%5Crm%7Bif%7D%5C%3Bm%5Cgt0%5C%3B%5Crm%7Band%7D%5C%3Bn%3D0%5C%5CA%5Cleft%28m-1%2CA%5Cleft%28m%2Cn-1%5Cright%29%5Cright%29%26%5Crm%7Bif%7D%5C%3Bm%5Cgt0%5C%3B%5Crm%7Band%7D%5C%3Bn%5Cgt0.%5Cend%7Barray%7D%5Cright.)

      测试Ack(3, 4)的值，阅读[https://en.wikipedia.org/wiki/Ackermann_function](https://en.wikipedia.org/wiki/Ackermann_function)，分析m和n取值对函数值计算的影响，深入理解递归；

   2. 编写一个函数，实现从序列中移除重复项，且保持元素间顺序不变。生成随机的列表和字典，验证所实现函数的功能。

2. 编写拥有 a) 对象成员hour、minute和second的时间类Time； b) 重载\_\_str\_\_和\_\_add\_\_方法； c) 方法time2int：把时间对象转换为秒数； d) 方法printtime：输出时间； e) 方法isafter：判断两个时间对象的先后； f) 方法increment：计算对象经过n>0秒后时间； g) 方法isvalid：判断时间对象合法性。在主函数设计代码验证Time各个方法的正确性。

3. 马尔可夫文本分析和应用

   1. 马尔可夫文本分析计算文本中单词组合和其后续单词（含标点符号）的映射，这个单词组合被称为马尔可夫分析的前缀，前缀中单词的个数被称为马尔可夫分析的“阶数”。编写Python代码实现某个文本的n阶马尔可夫文本分析，并且将分析结果记录在字典中；

   2. 采用 i. 所实现的马尔可夫分析模块，对“emma.txt”或“whitefang.txt”进行马尔可夫分析，运用n阶马尔可夫分析的结果生成由m个句子（注意首字母大写和结尾标点符号）组成的随机文本。分析所生成文本的语义自然性和阶数n的关系；

   3. 尝试采用Python不同的序列数据结构表示前缀，比较运行效率的差异。

4. 模拟快餐订餐场景

   1. 定义4个类：Customer顾客类，Employee商户类，Food食物类以及Lunch订餐管理；

   2. Lunch类包含Customer和Employee实例，具有下单order方法，该方法要求Customer实例调用自身的placeOrder向Employee对象要求下单，并且获得Employee对象调用takeOrder生成和返回一个Food对象，Food对象应当包含了食物名字符串。调用关系如下：

      Lunch.order → Customer.placeOrder → Employee.takeOrder → Food；

   3. Lunch类包含result方法，要求Customer打印所收到的食物订单；

   4. 编写交互式界面验证所设计的订餐系统。

