# 固体物理基础24小时预习大冒险 ✅

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
  \int_{S_\omega}{\frac{\mathrm{d}S_\omega}{\left|\nabla_q\omega_i(q)\right|}}
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
#### 概述
*定容***热容**：单位质量的物质在定容过程中，温度升高 1℃ 时，系统内能的增量：
$$ C_V = \lim_{\Delta T\to 0}{\left(\frac{\Delta{U}}{\Delta{T}}\right)_V}
= \left(\frac{\partial U}{\partial T}\right)_V $$
晶格热容 $C_{Vl}$ $\gg$ 电子热容 $C_{Ve}$，仅讨论晶格热容。

高温，杜隆—珀替定律：对确定的材料，高温下的热容为常数，摩尔热容为 $3R$。

低温，德拜定律：低温下的固体热容与 $T^3$ 成正比。

$$ N_0k_B = R $$

每个谐振子的平均能量为
$$ E(\omega_i, T) = \left(\frac{1}{2} + \bar{n}\right)\hbar\omega_i $$
晶格振动能量为 $3NS$ 个量子谐振子能量之和：
$$
U = \sum_{i=1}^{3NS}\bar{E}_i = \int_0^{\omega_m}{g(\omega)\bar{E}(\omega,T)\mathrm{d}\omega}
$$
其中 $\omega_m$、$$ 为截止频率：
$$ \int_0^{\omega_m}{g(\omega)\mathrm{d}\omega} = 3NS $$
定容热容为
$$
C_V = \left(\frac{\partial U}{\partial T}\right)_V
= \frac{\partial}{\partial T}\int_0^{\omega_m}g(\omega)\bar{E}(\omega,T)\mathrm{d}\omega
$$
联立解得
$$ C_V = \int_0^{\omega_m}{k_B \eta^2 \frac{\exp{\eta}}{(\exp{\eta}-1)^2} g(\omega) \mathrm{d}\omega} $$
其中 $\displaystyle\eta = \frac{\hbar\omega}{k_BT}$。

#### 爱因斯坦模型

假定晶体中所有原子都以相同频率独立地振动，
则晶体中的格波频率都相同。（适用于光学支格波）

晶体振动内能
$$U(T) = 3NS\left[\frac{1}{2} + \frac{1}{\displaystyle \exp{(\frac{\hbar\omega}{k_BT})}-1}\right]\hbar\omega$$
热容
$$
C_V = 3NSk_B(\frac{\hbar\omega}{k_BT})^2\frac{\displaystyle\exp{\frac{\hbar\omega}{k_BT}}}{\displaystyle(\exp{\frac{\hbar\omega}{k_BT}}-1)^2}
$$
引入爱因斯坦温度 $\Theta_E$：
$$ \hbar\omega_E = k_B\Theta_E $$
则
$$
C_V = 3NSk_B\left(\frac{\Theta_E}{T}\right)^2
\frac{\exp{(\Theta_E/T)}}{[\exp{(\Theta_E/T)-1}]^2}
$$

##### 高温情况
$\Theta_E/T \ll 1$，$\exp{x} \approx 1+x$，$C_V = 3NSk_B$。
##### 低温情况
$\Theta_E/T \to +\infty$，
$$ C_V = 3NSk_B\left(\frac{\Theta_E}{T}\right)^2\exp{(-\frac{\Theta_E}{T})} $$
当$T$趋近于$0$时，$C_v$以指数方式趋近于$0$，这是经典理论得不到的结果。但在非常低的温度实验曲线是$T_3$趋近于$0$，而不是以指数方式趋近于$0$。

#### 德拜模型
把晶体视为各向同性的连续弹性媒质。（适用于声学支格波）
设晶体是 $N$ 个初基原胞组成的三维单式格子（$S=1$）。
此时晶体中仅有 $3$ 支声学支格波，他们的相速 $v_p$ 都相同，
三支格波的色散关系均是线性的：
$$ \omega = v_pq $$
等频率面为球面：
$$ |\nabla_q\omega(q)| = \frac{\mathrm{d}\omega}{\mathrm{d}q} = v_p $$
态密度
$$ g(\omega) = 3 \cdot \frac{V}{(2\pi)^3} \cdot \frac{4\pi{q^2}}{v_p} $$
截止频率又称为德拜频率 $\omega_D$，由格波总数等于 $3N$ 来确定：
$$
\int_0^{\omega_D}{g(\omega)\mathrm{d}\omega} = 3N
\Longrightarrow
\omega_D^3 = \frac{6\pi^2Nv_p^3}{V}
$$
引入德拜温度 $\hbar\omega_D = k_B\Theta_D$，令
$$ x = \frac{\hbar\omega}{k_BT} $$
于是
$$ C_V = 9Nk_B\frac{T^3}{\Theta_D^3}
\int_0^{\frac{\Theta_D}{T}}{\frac{x^4\mathrm{e}^x}{(\mathrm{e}^x-1)^2} \mathrm{d}x} $$

长声学波相当于连续介质的弹性波。低温情况下，只有长声学波被激发，对比热有贡献。德拜模型所考虑的正是这些长声学波对比热的贡献。
通过使用低温时实验测得的$C_V$与理论得到的$C_V$相等来确定德拜温度。

德拜温度是用经典概念和量子概念解释比热的分界线。低于德拜温度，声子开始被冻结，要用量子统计规律处理问题。
高于德拜温度，声子全部被激发，可以用经典统计规律处理。 

##### 低温
$x = \frac{\hbar\omega}{k_BT} \to +\infty$，
$$
\int_0^\infty{\frac{x^4e^x}{(e^x-1)^2}\mathrm{d}x} = \frac{4\pi^4}{15}
$$
$$
C_V = \frac{12\pi^4}{5}Nk_B\left(\frac{T}{\Theta_D}\right)^3 
\propto T^3
$$
与德拜实验定律符合。

##### 高温
$e^x \approx 1+x$，积分 $\approx\int_0^{\Theta_D/T}{x^2\mathrm{d}x}$，
$$ C_V = 3Nk_B $$

#### 两种模型的比较
![两种模型的比较](https://abreto.github.io/final-exam/bachelor/sophomore/solidphy/avsd.jpg)

$$ U(T) = \sum_i^{\text{已激发格波}}{\bar{E}(\omega_i,T)} $$

T → 0时，比热 随温度的下降速度比实验数据 T3快，与实验曲线不符合。其原因是假设温度 T 时，所有格波都被激发，而且频率相等，而实际情况是只有 $\hbar\omega \le k_BT$ 的格波才能被激发，所以导致爱因斯坦模型在低温时与实验曲线不符合。

低温时，德拜模型结果与实验曲线符合。由于低温时，被激发的格波频率较小，波长较长，所以近似认为晶体是连续介质是可行的。温度越低，近似越好。

综上所述，高温下两种模型都正确，但爱因斯坦模型方便简单，因此在高温多用该模型；低温则多用德拜模型。对於复式格子，可以结合两个模型，德拜模型用于声频支，爱因斯坦模型用于光频支。

#### 关于德拜温度

1. $\Theta_D > \Theta_E$
2. 德拜温度是经典概念和量子概念定性解释热容现象的分界线

利用德拜模型求声子数，积分上限为 $k_BT/\hbar$（已被激发的声子的频率）

$$ \mathrm{d}N' = f_{BE}(\omega) \cdot g(\omega) \cdot \mathrm{d}\omega $$
$$ f_{BE}(\omega) = \bar{n}(\omega, T) = \frac{1}{\displaystyle\exp{\left(\frac{\hbar\omega}{k_BT}\right)}-1} $$

## 第四章 固态电子论基础

### 量子自由电子论
电子是费米子，服从泡利不相容原理的全同粒子，服从费米—狄拉克统计。
#### 自由电子的能级和能态密度

假定 $N$ 个无相互作用的自由电子被限制在边长为 $L$，
体积为 $V=L^3$ 的势阱中：
$$ -\frac{\hbar^2}{2m}\nabla^2\psi(\boldsymbol{r}) = E\psi(\boldsymbol{r}) $$
解得
$$ \psi(\boldsymbol{r})
=
\sqrt{\frac{1}{V}}\mathrm{e}^{i\boldsymbol{k}\cdot\boldsymbol{r}}
$$
$\boldsymbol{k}$ 为电子波的波矢。能量
$$ E(\boldsymbol{k}) = \frac{\hbar^2k^2}{2m}
= \frac{\hbar^2}{2m}(k_x^2+k_y^2+k_z^2) \qquad \text{(能带结构)} $$
周期性边界条件：
$$
\psi(0,y,z) = \psi(L,y,z) \\
\psi(x,0,z) = \psi(x,L,z) \\
\psi(x,y,0) = \psi(x,y,L) \\
\Downarrow \text{} \\ \text{} \\
e^{ik_xL} = e^{ik_yL} = e^{ik_zL} = 1
$$
于是
$$ k_i = \frac{2\pi}{L}n_i \qquad n_i \in \mathbb{Z},\ i \in \{x,y,z\} $$
$$ E = \frac{\hbar^2}{2m}\left(\frac{2\pi}{L}\right)^2(n_x^2+n_y^2+n_z^2) $$
每个电子能级容纳两个自旋相反的电子。

用一个波矢的 $k$ 值标志电子的一个空间运动状态 $\psi$，
由波矢 $\boldsymbol{k}$ 所代表的自由电子可能的空间运动状态称为自由电子态，
每一个电子态 $(k_x,k_y,k_z)$ 在波矢空间中用一个点表示。
波矢 $\boldsymbol{k}$ 在空间的分布是均匀的：
$$ \boldsymbol{k} = \sum_{i=1}^3 \frac{l_i}{N_i} \boldsymbol{b}_i
\qquad l_i \in \mathbb{Z} $$
沿轴方向相邻两个电子态距离为 $(2\pi)/L$，每个 $\boldsymbol{k}$ 点在 $\boldsymbol{k}$ 空间占有的“体积”为
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
$\boldsymbol{k}$ 点的密度为 $V/(2\pi)^3$、$S/(2\pi)^2$、$L/(2\pi)$.

> 考虑自旋，空间电子态为 $\boldsymbol{k}$ 的**两倍**！！

电子态密度（能态密度）：对给定体积的晶体，能级$E$附近单位能量间隔的电子状态数
$$
g(E) = \lim_{\Delta{E}\to{0}}\frac{\Delta{Z}}{\Delta{E}}
= \frac{\mathrm{d}Z}{\mathrm{d}E}
= \frac{V_c}{2\pi^2}\left(\frac{2m}{\hbar^2}\right)^{3/2}E^{1/2}
$$

能态密度函数
$$ g(E) = 2\cdot\frac{V_c}{(2\pi)^3}
\int_{S_E}\frac{\mathrm{d}S_E}{|\nabla_kE|} $$

$$
\newcommand\d{\mathrm{d}}
g(E)\d{E} = 2 \cdot
\left\{
  \begin{array}{c}
  \displaystyle \frac{L_c}{2\pi}\cdot 2 \\ \\
  \displaystyle \frac{S_c}{(2\pi)^2} \cdot 2\pi{k} \\ \\
  \displaystyle \frac{V_c}{(2\pi)^3} \cdot 4\pi{k^2}
  \end{array}
\right\}\d{k}
$$
> $k^2\hbar^2 = 2mE$.

#### 费米分布函数
电子的自旋量子数为半整数，分布服从费米—狄拉克统计规律：
$$
f_{F-D}(E, T) = \frac{1}{\displaystyle\mathrm{e}^{(E-E_F)/k_BT}+1}
$$
> 反映了能量为 $E$ 的每一个可占据的量子态被电子所占据的平均概率


$E_F$ 为全同粒子体系的化学势或费米能，是温度$T$和电子数$N$的函数：
$$ N = \int_0^\infty{}f(E)g(E)\mathrm{d}E $$
> 物理意义：在体积不变的条件下，系统增加一个粒子所需的自由能

![](https://abreto.github.io/final-exam/bachelor/sophomore/solidphy/fege.png)
![](https://abreto.github.io/final-exam/bachelor/sophomore/solidphy/fee.png)

$$
\mathrm{d}N = f(E,T)g(E)\mathrm{d}E \\ \text{} \\
\mathrm{d}\bar{U} = E\cdot\mathrm{d}N
$$

##### $T \to 0\mathrm{K}$ 时
$$
f(E,0) = \left\{
  \begin{array}{ll}
  1 & \quad E \le E_F^0 \\ \\
  0 & \quad E \ge E_F^0
  \end{array}
\right.
$$

在热力学绝对零度，能量低于 $E_F^0$ 的所有状态全部被电子所占据，高者都没有电子
$$ N = \int\mathrm{d}N = \int_0^{E_F^0}g(E)\mathrm{d}E $$
求得 
$$ E_F^0 = \frac{\hbar^2}{2m}(3\pi^2\frac{N}{V_c})^{2\over{3}} $$
每个电子的平均能量
$$ \bar{E} = \frac{1}{N}\int{E\mathrm{d}N} = \frac{3}{5} {E_F^0} $$
仍然很高。这是因为电子要遵从泡利原理，在绝对零度不可能所有的电子都填在最低能态，因而平均动能不为零。

##### $T > 0\mathrm{K}$ 时
自由电子气体的状态为热激发态。
当温度从绝对零度开始升高，电子按能量的分布将发生变化，但电子能量的任何改变必须由晶体的热能来提供。由于热能的量级 $k_BT$ 比电子能量要小得多，又要考虑泡利不相容原理，以致在通常的温度下，电子按能量的分布只能产生非常小的改变。

当 $E = E_F$ 时，$f(E,T) = 1/2$

自由系统总电子数
$$
N = \int_0^\infty{f_{F-D}(E,T)g(E)\mathrm{d}E}
$$
解得
$$
E_F \approx E_F^0\left[1-\frac{\pi^2}{12}
\left(\frac{k_BT}{E_F^0}\right)^2
\right]
$$
$E_F$ 略小于 $E_F^0$.

#### 费米面
> 费米面：电子能量等于费米能的等能面

* 费米半径 $\displaystyle k_F^0 = \left(3\pi^2\frac{N}{V}\right)^{\frac{1}{3}}$
* 费米动量（费米面上电子的动量） $p_F^0 = \hbar k_F^0$
* 费米速度 $v_F^0 = \hbar k_F^0 / m$
* 费米温度 $T_F^0 = E_F^0 / k_B$

#### 💊索末非自由电子气模型

基本假设：
1. 独立电子近似
2. 自由电子近似
3. 弹性碰撞近似
4. 电子是费米子，电子气服从费米—狄拉克统计分布

### 热容
#### 自由电子气
在温度为 $T$（稍高于绝对零度，远小于费米温度，室温也算） 时，每个电子的平均能量为
$$
\bar{E} \approx \frac{3}{5}E_F^0
\left[1+\frac{5\pi^2}{12}
\left(\frac{k_BT}{E_F^0}\right)^2
\right]
$$
自由电子气的摩尔热容应该为
$$
C_V^e = \left(\frac{\partial U}{\partial T}\right)_V
= N\frac{\mathrm{d}\bar{E}}{\mathrm{d}T}
= N\frac{\pi^2k_B}{2}\left(\frac{T}{T_F^0}\right)
= \gamma T
$$
其中 $\gamma = \frac{\pi^2k_B^2}{3}g(E_F^0)$ 为电子气的热容系数（索末非系数）。

由于只有费米面附近约 $k_BT$ 范围内的电子参与热激发，对比热有贡献，只是全部电子中极小的一部分，从而解决了经典理论对比热估计过高的困难。

#### 金属
金属的热容包括晶格振动（声子气）的贡献和自由电子气的贡献：
$$C = C_V^e + C_V^L$$

##### 高温（$T \gg \Theta_D$）
$$C_V = 3R + \gamma T$$
$$\frac{C_V^e}{C_V^l} = \frac{k_BT}{E_F^0} \sim 10^{-2}$$

##### 低温（$T \ll \Theta_D$）

$$C_V = \gamma T + b T^3$$
电子气热容随温度下降的变化比晶格热容的变化要缓慢得多，两者的大小变得可以相比。

但不少的金属的 $\gamma$ 的实验值与理论值有差别。原因在于在近自由电子的零级近似中，忽略了电子与电子，电子与晶格之间的相互作用；另外实际金属中的电子并不是在恒定势场中运动，而是在离子实的周期性市场中运动。

> 费米面附近的电子状态决定了金属的物理性质

## 第五章 固体能带论

> 每一个能带中，电子的能量与电子波矢有确定的关系，称之为能带结构

基本近似：
1. 绝热近似：$n$ 个价电子在 $N$ 个固定不动的周期排列的原子实的势场中运动
2. 单电子近似：任一电子都可视为是处在原子实周期势场和其他$(n-1)$个电子所产生的平均势场中的电子
3. 周期势场近似：晶体中电子的势能函数具有晶体的周期性，$V(\vec{r}) = V(\vec{r}+\vec{R}_n)$，$\vec{R}_n$ 为正格矢

### 固体中电子的共有化与能带

> 原子之间相互靠近而产生的相互作用使原子能级的简并消除，是固体中出现能带的关键。

* 导体：$V = V_0 + \delta{V}$
* 绝缘体：$V = V^{at} + \delta{V}$

傅里叶分解：
$$ V(r) = \sum_{G_n \ne 0}{V_n\cdot\mathrm{e}^{iG_n\cdot{r}}}
= \text{（一维）}\sum_{n\ne{0}}{V_n\mathrm{e}^{i\frac{2\pi}{a}nx}} $$
其中
$$
V_n =
\frac{1}{\Omega}\int_\Omega{V(r)\mathrm{e}^{-iG_n\cdot{r}}}\mathrm{d}r
= \text{（一维）}\frac{1}{a}\int_0^a{V(x)\mathrm{e}^{-i\frac{2\pi}{a}nx}}\mathrm{d}x
$$
$a$ 为晶格常数

能带内能级分布是准连续的

* 能级和能带一一对应
* 能带交叠
* 先交叠再分裂

### 布洛赫（Bloch）定理
在上述三个近似之下，
求解晶体中电子运动本征态的问题简化为解周期场中单电子薛定谔方程：
$$
\left[-\frac{\hbar^2}{2m}\nabla^2 + V(\boldsymbol{r})\right]\psi(\boldsymbol{k},\boldsymbol{r})
=
E\psi(\boldsymbol{k}, \boldsymbol{r})
$$

#### Bloch 定理
> 晶体中的电子波函数是按照晶格周期性进行的调幅平面波。
> 即在周期势场中，薛定谔方程的解具有如下形式：
> $$ \psi(\boldsymbol{k},\boldsymbol{r}) = U(\boldsymbol{k}, \boldsymbol{r})\mathrm{e}^{i\boldsymbol{k}\cdot\boldsymbol{r}} $$
> 其中，$U$ 与势场具有相同的周期性：
> $$ U(\boldsymbol{k}, \boldsymbol{r}) = U(\boldsymbol{k}, \boldsymbol{r}+\boldsymbol{R}_n) $$
> 晶体中电子的状态满足布洛赫定理，晶体中的电子波称为布洛赫波，晶体中电子称为布洛赫电子。

1. 电子出现的几率具有正晶格的周期性：$|\psi(\boldsymbol{k},\boldsymbol{r})|^2=|\psi(\boldsymbol{k},\boldsymbol{r}+\boldsymbol{R}_n)|^2$
2. （等价表述）在布洛赫函数中，将坐标平移一个正格矢的效果等于乘上一个相位因子：<br />$\psi(\boldsymbol{k},\boldsymbol{r}+\boldsymbol{R}_n) = \psi(\boldsymbol{k},\boldsymbol{r})\mathrm{e}^{i\boldsymbol{k}\cdot\boldsymbol{R}_n}$
3. 波函数本身并不一定具有正晶格的周期性，波矢 $\boldsymbol{k}$ 不一定是倒格矢（若考虑玻恩—卡曼边界条件，则 $\boldsymbol{k}$ 为倒格矢且均匀分布）

周期势场中的电子的波函数是自由电子的平面波 $\mathrm{e}^{ik\cdot{r}}$ 被周期函数 $u(k,r)$ 所调制，即调幅平面波。

##### 推论
1. $\boldsymbol{k}$ 态和 $\boldsymbol{k}+\boldsymbol{G}_h$ 态是相同的状态：
$$\psi(k+G_h,r)=\psi(k,r)$$
$$E(k+G_h) = E(k)$$
2. 在倒空间选取合适的坐标系：
$$E(\vec{k}) = E(-\vec{k})$$
3. 电子的能量状态 $E$ 具有与正晶格相同的对称性

#### 近自由电子模型
近自由电子模型讨论的对象是金属中的价电子。
原子实形成的周期性势场较弱，电子近似认为是自由电子，在薛定谔方程中取平均势$V_0$作为周期势$V(x)$的零级近似，而将$V(x)$的起伏部分当做微扰。

##### 能量与波函数

$$\psi^{(0)}(k,x) = L_c^{-\frac{1}{2}}\mathrm{e}^{ik\cdot{x}}$$
$$ E^{(0)}(k) = \frac{\hbar^2k^2}{2m} $$
布里渊区边界处
$$
E_k = E_k^{(0)} \pm |V_h|
$$

##### 波矢远离布区边界
$k'$ 也远离布区，为非简并情况。能量的修正项较小，近似认为是自由电子
$$E_k \approx = \frac{\hbar^2k^2}{2m}$$

##### 波矢接近布区边界
$k \to \frac{\pi}{a}$, $k' \to -\frac{\pi}{a}$，简并情况。
$$ E_{\pm} \approx T_h + |V_h| \pm o() $$

##### 在布区边界
$$ E_{\pm}(k) = E^{(0)}(k) \pm |V_n| $$
禁带宽度 $\Delta{E}_g = 2|V_n|$

![能带示意图](https://abreto.github.io/final-exam/bachelor/sophomore/solidphy/nd.png)
![色散关系图](https://abreto.github.io/final-exam/bachelor/sophomore/solidphy/ssgx.png)

因为N是很大的，因此K的取值以及相应的能级都是十分密集的，即准连续。这些准连续的能级被禁带隔开而形成一系列能带，每个能带所对应的k的取值范围都是2π/a，即一个倒易原胞的长度，而所包含的量子态数目又都是N，即等于晶体中原胞的数目。

属于同一个布里渊区的能级构成一个能带，不同的布里渊区对应于不同的能带，每个布里渊区体积相同，等于倒格子原胞的体积，每个能带的量子态数目：2N（计入自旋）。

#### 紧束缚模型
对绝缘体，其电子被紧紧地束缚在原子核周围。当原子之间相距很远时，电子被紧密束缚在原子的周围，其状态可用自由原子的波函数来描述。

在紧束缚近似下，
仅考虑最近邻原子间的波函数的交叠所得到的晶体的 $s$ 能带关系
$$
E_s(\boldsymbol{k})
 =
E_s^{at} - A - B
\sum_{\boldsymbol{R}_n \ne 0}^{\text{最近邻}}
\mathrm{e}^{
  i\boldsymbol{k}\cdot\boldsymbol{R}_n
}
$$

适用于绝缘体，相邻原子的电子波函数交替较少的半导体、金属的内层电子和过渡金属的 $d$ 电子。

能带宽度 $= E_{smax} - E_{smin}$

在紧束缚近似中，把能带同原子的能级联系起来，原子的不同能级在晶体中变成相应的能带，如S带，p带，d带等。外层电子的波函数交叠程度大将形成较宽的能带，而内层电子相应的能带比较窄。
原子可能有能量相等或相近的原子轨道，可能出现能带互相重叠的情况，这时能带与原子能级之间就没有简单的对应关系了。

### 电子的准经典运动

## 第六章 晶体中的缺陷

