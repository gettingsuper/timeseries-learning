#  时间序列笔记
## 时间序列1
### ARMA MODEL
autoregressive–moving-average(ARMA)模型，根据两个多项式提供（弱）平稳随机过程的简约描述，一个用于自回归（AR），第二个用于移动平均

**AR(P) MODEL**
ARp阶模型

$$ X_t  =  \sum_{(i=1)}^p \phi_i X_{(t-1)} +  \epsilon_t $$
可以算方差，协方差，自相关系数
stats中acf（）函数科画出时间序列数据自相关函数autocorrelation function，ACF的图像
```
acf( x, lag.max = Null,
type = c ("correlation","covariance"，"partial", plot = TURE, na.action = na.fail, demean = TURE,...)
```
x-时间序列数据；lag.max-时间间隔最大值，type-图形类型；"correlation","covariance"，"partial"-自相关函数、自协方差函数、偏自相关函数图

构造AR(1)过程（截距不影响自相关函数，设为0.2）
···

