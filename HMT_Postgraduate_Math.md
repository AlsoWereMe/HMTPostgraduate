# 高数

## 极限

### 两个重要极限

$$
\lim_{x\rarr0}{\frac{\sin x}{x}=1} \\\
\lim_{x\rarr\infty}{(1+x)^{\frac{1}{x}}=e} \\\
$$

### 等价无穷小

> x均为变量的整体，而非单个变量x

#### 三角函数类

$$
\sin x \sim x  , \ \arcsin x \sim x \\\
\tan x \sim x , \ \arctan x \sim x \\\
\sec x - 1 = 1 - \cos x \sim \frac{x^2}{2} \\\
$$

#### 指数、对数类

$$
\begin{aligned}
\log_a(1+x) &\sim \frac{x}{\ln a} \\\
a^x-1 &\sim x\ln a \\\
(1+x)^a-1 &\sim ax \\\
\end{aligned}
$$

#### 常用扩展

$$
\begin{aligned}
x-\ln(1+x)&\sim\frac{x^2}{2} \\\
\tan x - \sin x &\sim \frac{x^3}{2} \\\
\arcsin x - x \sim x - \sin x &\sim \frac{x^3}{6} \\\
x-\arctan x \sim \tan x - x &\sim \frac{x^3}{3}
\end{aligned}
$$



### 间断点

#### 第一类间断点

左右极限都存在，又分为：

- 跳跃间断点，左右极限不相等
- 可去间断点，左右极限相等

#### 第二类间断点

除第一类间断点外的任何间断点

## 导数

### 导数四项法则

加减乘除，除为分子导乘分母减分子乘分母导

### 导数基本公式 

#### 三角函数类

$$
\begin{aligned}
\sin x &\rarr \cos x \\\
\cos x &\rarr -\sin x \\\
\tan x &\rarr \sec^2 x \\\
\cot x &\rarr -\csc^2 x \\\
\sec x &\rarr \sec x \tan x \\\
\csc x &\rarr -\csc x \cot x
\end{aligned}
$$

#### 反三角函数类

$$
\begin{aligned}
\arcsin x &\rarr \frac{1}{\sqrt{1-x^2}} \\\
\arccos x &\rarr -\frac{1}{\sqrt{1-x^2}}\\\
\arctan x &\rarr \frac{1}{1+x^2}\\\
\end{aligned}
$$

#### 指数、对数类

$$
\begin{aligned}
\log_ax &\rarr \frac{1}{x\ln a}\\\
a^x&\rarr a^x\ln a
\end{aligned}
$$



### 莱布尼茨公式

$$
(uv)^{(n)}=\sum_{k=0}^n{C^k_nu^{n-k}v^{k}}
$$

 ## 微分

### 实际值与微分的近似

$$
\Delta y \approx\mathrm{d}y=f'(x_0)\Delta x\\\
x_0\text{代表一个简洁的定点，}\Delta x\text{为其增量，上式成立需要}\Delta x\rarr 0 \\\
\text{这个式子的推导式为：}\\\
f(x_0+\Delta x)=f(x_0)+f'(x_0)\Delta x \\\
\text{这代表了一个函数可以如下近似任意点} \ x=x_0+\Delta x \ \text{的值：}\\\
f(x)=f(x_0)+f'(x_0)(x-x_0) \\\
$$

> Tips: 谨记将一个表达式转回微分形式时一定要在后面加上一个常数C

## 洛必达法则

当$x\rarr a$时，如果$f(x),F(x)$同时趋近于$0$或$\infty$，那么:
$$
\lim_{x\rarr a}\frac{f(x)}{F(x)}=\lim_{x\rarr a}\frac{f'(x)}{F'(x)}
$$

## 函数的性质

### 单调性与驻点

特定区间内，一阶导数大于0则单调增，一阶导数小于0则单调减

驻点是一阶导数为0对应的点

### 凹凸性与拐点

凸函数的特殊性质：
$$
\frac{f(x)+f(y)}{2}< f(\frac{x+y}{2})
$$
对应的，凹函数为：
$$
\frac{f(x)+f(y)}{2}> f(\frac{x+y}{2})
$$
形式上，理解为两点连线后，其中点处函数值在连线上方则为凸函数，连线下方则为凹函数

区间内，二阶导数大于0则凹，二阶导数小于0则凸

拐点是二阶导数为0对应的点

### 极值与最值

对于函数$f(x)$，x为极小值点当
$$
f'(x+\epsilon)>0\and f'(x-\epsilon)<0 \\\
或 \\\
f''(x)>0 \and f'(x)=0
$$
x为极大值点当
$$
f'(x+\epsilon)<0\and f'(x-\epsilon)>0 \\\
或 \\\
f''(x)<0\and f'(x)=0
$$
若求区间$[a,b]$内的最值，求出所有驻点$x_0,...,x_n$，并比较
$$
f(a),f(b),f(x_0),...,f(x_n)
$$
即可

### 曲率

曲率K为
$$
K=\frac{|y''|}{(1+y'^2)^{3/2}}
$$
曲率半径为曲率的倒数

## 积分

### 积分基本公式与三角恒等式

$$
\begin{align}
\int \tan xdx&=-ln|\cos x| + C \\\
\int \cot xdx&=ln|\sin x| + C \\\
\int \sec xdx&=ln|\sec x + \tan x| + C\\\
\int \csc xdx&=ln|\csc x - \cot x| + C\\\
\int \frac{dx}{a^2 + x^2}&=\frac{1}{a}\arctan{\frac{x}{a}} + C\\\
\int \frac{dx}{x^2 - a^2}&=\frac{1}{2a}ln{|\frac{x-a}{x+a}|}+C \\\
\int \frac{dx}{\sqrt{a^2 - x^2}}&=\arcsin{\frac{x}{a}} + C\\\
\int \frac{dx}{\sqrt{x^2 \pm a^2}}&=ln(x+\sqrt{x^2 \pm a^2}) + C\\\
\end{align}
$$

$$
sin A cos B = \frac{1}{2}[sin(A+B) + sin(A-B)]\\\
cos A cos B = \frac{1}{2} [cos(A+B) + cos(A-B)]\\\
sin A sin B = \frac{1}{2} [cos(A-B) - cos(A+B)]\\\
$$

### 分部积分法
