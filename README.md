# BitWar
# 编译原理课程项目（比特大战）
## 介绍
在设计好一种程序语言的基础上，使用该语言进行比特大战的程序设计。

比特大战，最主要的是编写出可供用户选择的5种策略，并根据每一回合A、B双方选定的策略来进行判断各方的得分情况，得分高的玩家获胜。

各方根据自己做出的选择获得相应分数

其中，有5种可供用户选择的策略，具体描述如下：
* （T1）永远合作，每次都选择1；
* （T2）随机，每次以某个概率随机选择1，否则选择0；
* （T3）针锋相对，先选择1，以后每次都选择对方的上一次选择；
* （T4）老实人探测器，基本和“针锋相对”一样，只是会随机的选择一次0；
* （T5）永不原谅，一直选择1，一旦对方选择0，则一直选择0。

## 设计语言
   策略Strategy和比赛Competition可以看成是不同的对象。比赛可以看成是一个事件源，比如10回合的比赛就会产生10个事件的事件流。策略是一组响应式的操作符，可以对比赛的事件作出响应。
   设计的语言非常简单，没有数据类型的概念，只有数值变量、数值、算数运算符、逻辑运算符等。
