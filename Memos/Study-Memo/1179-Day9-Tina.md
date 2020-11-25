#第九讲总结
2018011179 无85 叶天

##一、python中的数学工具：
###积分：import scipy.integrate as sci
1、数值积分:
	定积分：给定上下限和数学函数下的数值积分
	输入列表或者包含函数值和输入值的ndarray对象作为输入，包括使用梯形法则、辛普森
2、蒙特卡洛模拟积分：通过模拟求取积分

###符号计算-SymPy库 import SymPy as sy
会自动化简多项式
SymPy还可以算积分也可以微分（符号计算）

##二、高性能计算库：
###数值计算：numexpr(单线程、多线程)

```python
import numexpr as ne
b=ne.evaluate("sin(a+i)**2+cos(a+i)**2+a**1.5")
```
###并行计算：multiprocessing库

###编译方案：
```python
import numba as nb
```
用Cython进行静态编译

##三、如何获取α：绝对收益

###Alpha的实操框架：
	金融工程模型分类：股票、ETF/期货、债券/期权策略
###基本逻辑：
1、投资组合的建立：一部分是精选A股市场最好的股票，构建现货投资组合；另一部分是做空股指期货，利用股指期货低成本、高杠杆的特性，对冲系统风险。
2、一个典型的股票型Alpha策略基金案例：超配计算机和传媒
3、典型的股票Alpha策略模型的收益特点：
牛市初期阶段：沪深300平稳，Alpha收益上升
牛市中期：指数涨挺好，但Alpha策略开始回撤，考验风控能力
熊市：指数大幅下降，Alpha策略波动

###商品期货交易策略
商品套利（配对）交易策略
举例1-跨品种套利：如螺纹钢和热卷品种都是钢材，相关性很大
举例2-跨期套利：不同到期日的期货合约价差在一个相对稳定的区间，一旦价差大...
举例3-产品特性跨期

###交易型策略：
多空策略：HANS123
回归策略：三种ETF套利方式



