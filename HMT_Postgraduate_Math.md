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


