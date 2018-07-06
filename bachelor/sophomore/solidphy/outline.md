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

一维单原子链情况下，每个 $q$ 值对应一个 $\omega$，
一组 $(\omega,q)$ 对应一个格波，$N$ 个原子有 $N$ 个格波。
格波频率与波矢的关系是一条色散曲线，
$N$ 个格波构成一支格波，
波矢 $q$ 取值数 = $N$（初基元胞数），
一维单原子链只有一支格波（一个初基元胞中原子自由度）。

##### 通解

每一个原子（确定的 $n$）参与了 $N$ 个独立的简谐振动
$$
U_n(t) = \sum_q^N{A_q\mathrm{e}^{i(qna-\omega{}t)}}
$$

### 一维双原子链的晶格振动
#### 模型与💊色散关系
有两支 $\omega \sim q$ 关系。

当取“$-$”号时，$\omega$ 记为 $\omega_A$，
称为声学支（Acoustic branch）格波；
取“$+$”号时，$\omega$ 记为 $\omega_O$，
称为光学支（Optical branch）格波。
分别描述了原子不同的运动状态。

![一维复式格子晶体中可以存在两种独立的格波](https://abreto.github.io/final-exam/bachelor/sophomore/solidphy/oanda.png)

当 $q=0$ 时，$\omega_A = 0$，$\omega_O \ne 0$.

#### 关于声学波与光学波的讨论
##### 格波数
为保证每支格波中 $\omega$ 与 $q$ 之间的一一对应关系，
限制 $q$ 的取值范围为第一布里渊区
$$ -\frac{\pi}{a} < q \le \frac{\pi}{a} $$
利用周期性条件得到
$$ q = \frac{2\pi{}m}{Na} \qquad m \in \mathbb{Z} $$
在第一布里渊区内，可取的 $q$ 点数为
$$ \frac{2\pi/a}{2\pi/(Na)} = N $$
这里 $N$ 为一维晶格的初基原胞数。
每个 $q$ 对应两个频率，共有 $2N$ 组 $(\omega,q)$，
有 $2N$（原子数目） 个格波。
晶体中任何一原子的运动均为这 $2N$ 个格波所确定的谐振动的现行叠加。
晶体的总自由度数也为 $2N$.

> 允许的波矢($q$)数 = 晶体的初基原胞数
> 
> 格波总数 = 晶体振动的总自由度数

##### 长波极限

当 $|q| \to 0$、$\lambda \to \infty$ 时，
相邻原胞间的振动相位差 $qa \to 0$.

声学支格波具有声波的线性色散关系：
$\omega_A = \upsilon_0q$，
且其频率很低（可以用超声波来激发，故此得名）。
完全相同原子所组成的布喇菲格子只有声学波。

光学支格波在 $q = 0$ 附近 $\omega_O$ 几乎与 $q$ 无关，
在 $q=0$ 处有极大值（可以和电磁波作用，故此得名）。

对于两种原子的振幅比：
- 声学支： $A_2/A_1 > 0$
- 光学支： $A_2/A_1 < 0$

在长波极限下，声学支格波描述原胞内原子的同相运动，
光学支格波描述原胞内原子的反相运动。
![在长波极限下声学支格波和光学支格波相应原子的运动](https://abreto.github.io/final-exam/bachelor/sophomore/solidphy/avso.jpg)

##### 短波极限（$q$ 趋近第一布里渊区边界）

当 $a \to \pi/a$ 时，
在第一布里渊区边界上，存在格波频率“间隙”：
$$ \Delta\omega = \omega_O - \omega_A $$
$\omega$ 值处于间隙和 $\omega > \omega_O$ 的波
不能在晶体中传播，
一维双原子链晶体对格波的作用就是一个带通滤波器。

相邻原胞的相位差 $qa \to \pm\pi$.
声学支格波仍描述原胞内原子的同相整体运动，
光学支格波仍描述原胞内原子的反相运动。

##### 振动特点

声学支在 $q=0$ 时，$\omega=0$。随着 $q$ 增加，曲线开始线性上升，表明在 $q \to 0$ 时，晶格可以看成弹性连续介质，格波类似于声波，曲线的斜率 $\omega/q=v_p=\text{常数}$，相当于声速。随着 $q$ 增加，曲线逐渐偏离直线向下弯曲，最后在 $q=\pm\pi/2a$ 时， $\omega$ 达到极大值。这是因为 $q$ 增大，波长减小，来自原子的散射加强，晶格不能再被看成连续介质。

光学支在 $q=0$ 时，有极限频率。$q$ 增大，曲线缓慢下降，$q=\pm\pi/2a$ 时, $\omega$ 达到极小值，在 $q$ 的整个变化范围内 $\omega$ 的变化不大，经常把 $\omega$ 看成常数，尤其是两个原子质量相差很大时。

#### 三维晶格振动

设实际三维晶体沿基矢
$\boldsymbol{a}_1, \boldsymbol{a}_2, \boldsymbol{a}_3$
方向的初基原胞数分别为 $N_1, N_2, N_3$，
晶体由 $N=N_1\cdot N_2\cdot N_3$ 个初基原胞组成，
每个初基原胞内含 $S$ 个原子。

###### 原子振动方向

一维：波矢 $q$ 和原子振动方向相同，只有纵波。

三维：波矢 $\boldsymbol{q}$ 和原子的振动方向可能不同，
原子的三维振动分解为与波矢 $\boldsymbol{q}$ 平行和垂直的
$3$ 个分量。
三维晶体的格波有振动方向与波矢 $\boldsymbol{q}$ 平行的
一种**纵波**（L）
和与波矢垂直的两种**横波**（T）。

##### 格波支数
> 每只格波都描述了晶格中原子振动的一类运动形式。
> 初级原胞有多少个自由度，
> 晶格原子振动就有多少种可能的运动形式，
> 就需要多少支格波来描述。

一维单原子链：自由度 $1$，原子的运动就是原胞质心的运动，仅存在一支格波，声学支格波。

一维双原子链：自由度 $2$，两支格波，一声一光。初基原胞质心的运动主要由声学支格波代表，初基原胞内两原子的相对运动主要由光学支格波代表。

一维 $S$ 原子链：自由度 $S$，$S$ 支格波，$1$ 支声学波，
$S-1$ 支光学波（假设确定了某个原子与其他$S-1$个原子的相对运动，则任意两个原子间的相对运动可以通过以该原子为参考系合成得到，故只有 $S-1$ 支光学格波）

三维晶体：晶体由 $N$ 个初基原胞组成，每个初基原胞内有 $S$ 个原子，每个原子有 $3$ 个自由度，初基原胞的总自由度数为 $3S$，晶体中原子的振动用 $3S$ 支格波来描述。
定性地描述原胞质心运动的声学支格波有 $3$ 支，剩下 $3(S-1)$ 支为光学支格波。

> 格波色散曲线也成为声子谱。

![](https://abreto.github.io/final-exam/bachelor/sophomore/solidphy/gebozhishu.png)

> 由于晶体晶格的对称性，两支 TA 重合，两支 TO 重合的现象称为简并。

##### 格波数

一维 $S$ 原子链存在 $S$ 支格波，一个 $q$ 对应 $S$ 个格波，$q$ 的取值数为初基原胞数 $N$，晶体中总共有 $NS$ 个格波，运动方程组共有 $NS$ 个方程，可有 $NS$ 个解，晶体的总自由度数 $NS$.

三维晶格中 $3S$ 支格波，一个 $\boldsymbol{q}$ 对应 $3S$ 个 $\omega$ 值，对应 $3S$ 个格波。$\boldsymbol{q}$ 取值数仍为初基原胞数 $N$，共有 $3NS$ 个 $(\omega_i,\boldsymbol{q})$ 数组，晶体中有 $3NS$ 个格波。
> 晶体中格波数 = 晶格的总自由度数

##### 波矢取值
三维原子的位移：
$$ U_{na_i} = A_i\mathrm{e}^{i(\boldsymbol{q}\cdot\boldsymbol{R}_{na_i}-\omega{}t)} \qquad i = 1,2,3 $$
三维玻恩卡曼条件：
$$ U_{na_i} = U_{(n+N_i)a_i} $$
得
$$ \mathrm{e}^{i\boldsymbol{q}\cdot{}N_i\cdot{}\boldsymbol{a}_i} = 1 \qquad i = 1,2,3 $$
由倒格子基矢的定义 $\boldsymbol{a}_i \cdot \boldsymbol{b}_j = 2\pi\delta_{ij}$，可知同时满足 $3$ 个式子的波矢为
$$ \boldsymbol{q} = \frac{L_1}{N_1}\boldsymbol{b}_1 + \frac{L_2}{N_2}\boldsymbol{b}_2 + \frac{L_3}{N_3}\boldsymbol{b}_3 $$
其中 $L_i \in \mathbb{Z}$；$\boldsymbol{b}_1, \boldsymbol{b}_2, \boldsymbol{b}_3$ 是倒格子基矢；$N_1, N_2, N_3$ 是基矢三个方向的初基原胞数。每组 $(L_1,L_2,L_3)$ 对应一个波矢。
这些波矢在到空间逐点表示出来，在任一方向上是均匀分布的。
每个 $\boldsymbol{q}$ 点所占体积为
$$
\frac{\boldsymbol{b}_1}{N_1}\cdot
\left(
  \frac{\boldsymbol{b}_2}{N_2} \times \frac{\boldsymbol{b}_3}{N_3}
\right)
=
\frac{\Omega^*}{N}
=
\frac{(2\pi)^3}{V}
$$
其中 $V = N\Omega$ 是晶体体积。$\boldsymbol{q}$ 的取值范围在第一布里渊区内，
可取值数目为：
$$ \frac{\Omega^*}{\Omega^*/N} = N $$
密度为
$$ \frac{N}{\Omega^*} = \frac{V}{(2\pi)^3} \qquad \text{三维} $$
$$ \frac{S}{(2\pi)^2} \qquad \text{二维，总面积} $$
$$ \frac{L}{2\pi} \qquad \text{一维，总长度} $$

#### 格波态密度函数

> 格波态密度函数 $g(\omega)$（模式密度数）：
> 确定体积 $V$ 的晶体，在 $\omega$ 附近单位频率间隔内的格波总数。

$$ g(\omega) = \frac{\omega\sim\omega+\mathrm{d}\omega\text{频率间的格波数}}{\mathrm{d}\omega} $$

> 格波数：$q$ 点密度 $\times$ $\omega\sim\omega+\mathrm{d}\omega$ "体积"

$$g(\omega) =
\sum_{i=1}^{3S}
{
  \frac{V}{(2\pi)^3}
  \int_\omega{\frac{\mathrm{d}S_\omega}{\left|\nabla_q\omega_i(q)\right|}}
}
$$

如果 $\omega(\boldsymbol{q})=\omega(q)$，有每一支格波
$$ g_i(\omega)\mathrm{d}\omega = {
  \left\{
    \begin{array}{lc}
    \text{一维} & \displaystyle \frac{L}{2\pi} \\ \\
    \text{二维} & \displaystyle \frac{S}{(2\pi)^2} \\ \\
    \text{三维} & \displaystyle \frac{V}{(2\pi)^3} \\
    \end{array}
  \right\}
}\mathrm{d}\vec{q} $$
其中
$$
\newcommand\d{\mathrm{d}}
\mathrm{d}\vec{q} = 
\left\{
  \begin{array}{cl}
  \displaystyle \d(2q) = 2\d{q} & \text{一维} \\ \\
  \displaystyle \d(\pi{}q^2) = 2\pi{q}\d{q} & \text{二维} \\ \\
  \displaystyle \d(\frac{4}{3}\pi{q^3}) = 4\pi{q^2}\d{q} & \text{三维}
  \end{array}
\right.
$$

### 晶格振动的量子化与声子

> 在简谐近似下，晶体中存在 $3NS$ 个独立的简谐格波，
> 晶体中任一原子的实际振动状态由这 $3NS$ 个简谐格波共同决定。

#### 晶格振动与谐振子

在经典力学的框架内，引入简正坐标，可得到如下结论：
由 $N$ 个原子组成的一维晶体，其晶格振动能量可看成 $N$ 个谐振子的能量之和。

#### 能量量子和声子

频率为 $\omega$ 的谐振子，一个频率为 $\omega$ 的格波，能量为
$$ E_n = \left(\frac{1}{2} + n\right)\hbar\omega \qquad n = 0,1,2,\cdots $$
当 $n = 0$ 时，处于基态，零点振动能 $E = \hbar\omega/2$。
相邻状态的能量差为 $\hbar\omega$，是谐振子的能量量子，称为声子。

系统总能量
$$ E = \sum_{i=1}^{3NS}{\left(\frac{1}{2}+n_i\right)\hbar\omega_i} $$
三维晶体中 $3NS$ 个格波与 $3NS$ 个量子谐振子一一对应。
频率为 $\omega_i(\boldsymbol{q})$ 的格波被激发的程度，
用该格波所具有的能量为 $\hbar\omega_i(\boldsymbol{q})$ 的声子数 $n$ 的多少来表征。

引入声子概念后，对于具有强相互作用的原子的集体运动状态——晶格振动的每一个格波，便可以看成是由数目为 $n$ 能量为 $\hbar\omega_i$ 的理想声子组成的，而整个系统则是由众多声子组成的声子气体。

晶格振动时产生了声子，声子的能量为 $\hbar\omega_i(\boldsymbol{q})$。
三维晶体的
* $3$ 支声学支格波 $\longmapsto$ $3$ 支声学声子
* $3(S-1)$ 支光学支格波 $\longmapsto$ $3(S-1)$ 支光学声子
* $3NS$ 个格波 $\longmapsto$ $3NS$ 种声子

简谐近似下，系统是无相互作用的声子气系统；考虑非简谐效应：声子和声子间存在相互作用。

声子的特性：
1. 声子是玻色子。一个模式可以被多个相同的声子占据。
2. 声子是非定域的。对等温平衡态，声子属于整个等温平衡的晶体。
3. 声子是一种准粒子，粒子数不守恒。温度升高，声子频率和声子数增加。
4. 遵守能量守恒和准动量选择定则。
声子的准动量 $\hbar\boldsymbol{q}$。声子与声子，声子与其他粒子、准粒子的相互作用满足能量守恒。

准动量选择定则：准动量的确定只能准确到可以附加任何一个倒格矢 $\boldsymbol{G}_h$：
$$ \omega(\boldsymbol{q}) = \omega(\boldsymbol{q} + \boldsymbol{G}_h) $$

声子的扩散同时伴随着热量的传导。

#### 平均声子数

频率为 $\omega$ 的格波在温度为 $T$ 时的平均声子数
$$ \bar{n}(\omega, T) = {{1} \over {\exp\left(\displaystyle\frac{\hbar\omega}{k_BT}\right)-1}} $$
定量地表示出一个格波被激发的程度。

定性地，$\bar{n}(\omega,T) \ge 0.6$ 的格波已被激发，
即温度为 $T$ 时，只有 $\hbar\omega \le k_BT$ 的格波才能被激发。

### 💊晶体的热容
