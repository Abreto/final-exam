# 固体物理基础24小时预习大冒险

## 第一章 晶体结构

> 根据**组成粒子空间位置的区别，
> 即物质结构上的差别**，
> 通常将固态材料分为晶体、准晶体和非晶体三大类。

> 晶体的结构特点是组成粒子在空间的排列具有周期性，
> 表现为既有**长程取向有序**，又有**平移对称性**。

### 1 空间点阵学说（布拉菲格子）

#### 七大晶系

|晶系|单胞基失的特性|布拉菲格子|所属点群|
|:---:|:---:|:---:|:---:|
|三斜晶系|$\boldsymbol{a}_1 \ne \boldsymbol{a}_2 \ne \boldsymbol{a}_3$ <br /> 夹角不等 |简单三斜 $P$ | $C_1, C_i$ |
|单斜晶系|$\boldsymbol{a}_1 \ne \boldsymbol{a}_2 \ne \boldsymbol{a}_3$ <br /> $\boldsymbol{a}_2 \perp \boldsymbol{a}_1, \boldsymbol{a}_3$|简单单斜<br />底心单斜|$C_2,C_s,C_{2h}$|

#### 14种布拉菲格子
![14种布拉菲格子](https://abreto.github.io/final-exam/bachelor/sophomore/solidphy/14blf.jpg)

## 第二章 晶体的结合
![晶体结合的基本类型和特点](https://abreto.github.io/final-exam/bachelor/sophomore/solidphy/combine.JPG)

## 第三章 晶格振动

> 在常温下晶体中原子热运动的幅度和原子间距相比是很小的，
> 称晶体原子的这种微振动为**晶格振动**。

> 原子的运动状态会在晶体中以波的形式传播，
> 形成“**格波**”。

### 一维单原子晶格的振动

#### 物理模型与运动方程

第 $n$ 个原子的运动方程为
$$
m\frac{\mathrm{d}^2(na+U_n)}{\mathrm{d}t^2}
=
m{{\mathrm{d}^2U_n} \over {\mathrm{d}t^2}}
=
f_{n-1} + f_{n+1}
=
\beta(U_{n+1}+U_{n-1}-2U_n)
$$
$n$ 总共可取 $N$ 个值，该式实为 $N$ 个方程组成的方程组，
可用 $N$ 个解，晶体的总自由度为 $N$。

当 $a$ 非常小时，一维原子链可看做一个连续长杆，
$$
\left\{
    \begin{array}{c}
        na \to x \\
        a \to \Delta{}x
    \end{array}
\right. \\
U_n(t) = U(na,t) \to U(x,t)
$$

上式可化简为

$$
\frac{\mathrm{d}^2U(x,t)}{\mathrm{d}t^2}
=
\upsilon_0^2\frac{\mathrm{d}^2U(x,t)}{\mathrm{d}x^2}
$$
$\upsilon_0^2 = a^2\beta/m$

试探解：
$$
U_n(t) = A\mathrm{e}^{i(qna-\omega{}t)}
$$
$q = 2\pi/\lambda$ 是波矢。
上式表示了一个简谐运动，
也代表了一种全部原子都以同一频率 $\omega$，
同一振幅 $A$，相邻两原子振动相位差均为 $qa$ 的集体运动模式。
这是一个简谐行波，称他为一个**格波**。

> 一个格波是晶体中全体原子都参与的一种简单的集体运动形式。

格波的相速度 $v_p = \frac{\omega}{q}$.

> 一个格波表示的是所有原子同时做频率为 $\omega$ 的振动。

格波波长 $\lambda = \frac{2\pi}{q}$，波矢 $\vec{q} = \frac{2\pi}{\lambda}\vec{n}$，相位差 $(n'-n)qa$.

格波的取值：
$$
-\frac{\pi}{a} < q \le \frac{\pi}{a} \qquad \text{-- 第一布里渊区}
$$

#### 💊 玻恩—卡曼周期性边界条件

> 晶体的热学特征近似地与边界条件的选择无关

假设在有限晶体之外有无限多个和这个有限晶体完全相同的假想晶体，
它们和实际晶体彼此毫无缝隙地衔接在一起，
组成一个无限的晶体，保证了有限晶体的平移对称性。

边界条件：$U_n = U_{n+N}$，代入试探解得到
$$ qNa = 2\pi{}m \qquad m = 0, \pm 1, \pm2, \dots $$
即
$$ q = \frac{\pi}{a}\frac{2m}{N} $$
格波波矢的特征：
1. 格波的波矢 $q$ 不连续
2. $q$ 点的分布均匀，相邻 $q$ 点的间距为 $2\pi/(Na)$
3. $\lambda=2\pi/q=Na/m$

由 $q$ 的限制条件得 $-\frac{N}{2}\le m < \frac{N}{2}$，
$m$ 只能取 $N$ 个分离的值，
晶体振动的波矢数=晶体的初基原胞数（一维）。

#### 关于格波的讨论

##### 格波
群速（能速）
$$v_g = \frac{\mathrm{d}\omega}{\mathrm{d}q}$$
在无色散的媒质中，波速 $v_0$、相速 $v_p$、群速 $v_g$ 三者相同。

##### 色散关系

> 色散本来是指光在某一媒质中传播的速度与频率有关的现象。

若 $\omega \sim q$ 间为线性关系，则相速为常数，
即各种频率的波在该媒质中传播时不发生色散。
在晶格振动的理论中，把 $\omega \sim q$ 之间的关系称为色散关系。

$$\omega = \omega_m\left|\sin{{qa} \over {2}}\right|$$
其中 $\omega_m=(4\beta/m)^{1/2}$。
式中不出现变量 $n$，
描述的格波是满足运动方程的所有原子都参与的一种集体运动模式。
一维单原子链的色散关系：
![一维单原子链的色散关系](https://abreto.github.io/final-exam/bachelor/sophomore/solidphy/ywdyzldssgx.jpg)

$$
\omega_m = \left(\frac{4\beta}{m}\right)^{1\over{}2}
\qquad
\text{当}\ q = \pm\frac{\pi}{2}\ \text{时}
$$
高于该频率的格波不能在晶格中传播，称为截止频率。
可以将一维单原子晶格看成低通滤波器。

$$v_p = v_0\frac{|\sin{qa/2}|}{qa/2}$$
$v_p$ 是 $q$ 的函数，有色散。

格波频率是波矢的周期函数，
周期为 $2\pi/a$（一维原子链的最短倒格矢），倒格子周期性，
倒格子平移对称性：
$$ \omega(q) = \omega(q+G_h) $$

倒格子反演对称性：
$$\omega(q) = \omega(-q)$$

以上两个对三维晶格适用。✔

若 $q$ 为正，表示沿某方向前进的格波，$q$ 为负则表示沿反方向传播的格波。

###### 极限情况下的波动性质
* 长波近似 <br />
  当 $a \ll \lambda$、$\lambda \to \infty$、$q \to 0$ 时，$\sin(qa/2)\approx{}qa/2$，得
  $$\omega = v_0q$$
  与连续介质中弹性波的色散关系一致，称为无色散。
  在长波极限下，对以一维单原子晶格格波可以看作是弹性波，晶格可以看成是连续介质。相邻两个原子间的相位差 $qa \to 0$，
  一个波长内包含许多原子。
* 短波极限<br />
  当 $q \to \frac{\pi}{a}$，格波波长 $\lambda = 2a$：
  两个相邻原子振动反相。

##### 格波数

一维单原子链：格波数=在第一布里渊区中波矢 $q$ 的取值数。

*在 $q$ 空间*，$q$ 点均匀分布，
相邻 $q$ 点间的“距离”为 $2\pi/(Na)$，
所以允许的 $q$ 值总数为
$$ \frac{2\pi/a}{2\pi/(Na)} = N $$
这里 $N$ 是原子总数，对于单式格子也就是初基原胞的总数。

> 允许的 $q$ 值总数等于组成晶体的初基原胞数（每个初基原胞含有一个基元，也就是基元的总数）。
