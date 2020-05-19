# Chap. 2

## 反常霍尔效应

1988: Haldane 提出周期性词结构下的绝缘相, 手性边缘态 \(\pm e^2/\hbar\), 只沿一个方向传播

新物态: Chern 绝缘体 = 量子反常霍尔绝缘体

## 量子自旋霍尔效应

Haldane 模型中周期性磁场, 总磁场为0在石墨烯晶格中难以实现

2005: Kane 和 Mele 考虑石墨烯中的SOC, 得到 helical 边缘态 \(2e^2/\hbar\) , 量子自旋霍尔态 2D TI

## 二维拓扑绝缘体: HgTe 量子阱

[Experiment](https://arxiv.org/pdf/0710.0582.pdf)
[Spin-Hall Insulator Theory](https://arxiv.org/pdf/cond-mat/0406001.pdf)

## 计算 Berry Curvature

$$\bra{m,\bm{k}}\Big(\nabla_{\bm{k}}\ket{n,\bm{k}}\Big) = \frac {\bra{m,\bm{k}} (\nabla_{\bm{k}}\hat H(\bm{k}))\ket{n,\bm{k}}} {E_m-E_n}$$

## Berry Curvature 和宏观可测量量

### Velocity in QHE

半经典近似下:

$$\hat H = \frac 1 {2m^*} (\hat p + e \bm{A}(t))^2$$

得到:

$$\bm{v}_n(\bm{k}) = \frac 1 {\hbar} \nabla_{\bm{k}} E_n(\bm{k})$$

电流密度:

$$\bm{J} = -e \sum_n \int \frac {\td^3 \bm{k}} {(2\pi)^2} \bm{v}_n(\bm{k}) f(k)$$

其中 \(f\) 为电子的分布函数. 这个式子直接的推论就是如果体系有一个非零的 gap, 换言之电子填满若干能级, 这个积分总是 \(0\).

Hall 电导: TKNN不变量: 1982

## 第四周

自旋Hall: 无外磁场是, 不同自旋方向的电子向相反方向偏转.
观测: Kerr 效应, 体系注入自旋极化的电流

SOC: 参考基于相对论效应的Hamiltonian推导

soc将导致能带(在\(k\neq 0\))劈裂, 产生不同有效质量的空穴.

Dresselhaus Effect: 体内空间反演不对称
Rashba Effect: 结构反演不对称

其他: 非线性Hall效应(https://arxiv.org/abs/1508.00571, https://www.nature.com/articles/s41563-019-0294-7),


另外，这个视频总体上是捍卫了同人文学作为一种正经创作的地位，也就是捍卫了你们磕CP文背后的作者的尊严。你们想清楚再来攻击我吧。

## 第五周

1801110172 王朕铎

### 量子电导和弹道输运

Ohm's Law:

$$G = \sigma \frac {W} {L}$$

\(W\) 为面积, \(L\) 为导体的长度. 根据Ohm's Law, \(L\rightarrow 0\Rightarrow G\rightarrow \infty\).
实际上当 \(L\) 远小于载流子的平均自由程时, \(G\) 趋向与一个固定值而非0, 偏离Ohm's Law.

偏离是容易理解的, 因为Ohm's Law描述的是经典的扩散输运(碰撞导致电阻), 当 \(L\ll L_f\) 时, 电子为弹道输运, 没有碰撞自然是偏离Ohm's Law的.

接下来讨论这个固定值 \(G_c\) 的来源. 对于一个ballistic conductor(no scattering), 电阻应当为0. 电阻来源于电极和导体的接触界面. 宏观尺度大小的电极中, 电流被大量的transverse mode承载. 而在介观尺度的ballistic conductor中, 电流只有少数几个mode, 因此界面处电流从多模->少模, 有一个重新分布的过程.

$$G=M 2e^2/h$$

\(M\) 为窄导体的通道数(量子化的电导). 此为Landauer公式, 参见 Imry Y(1986)

### 2D里的量子Hall effect和Spin Hall effect

Bulk Insulator with Spin-dependent Kramers-pair gapless edge states

Kramers-pair Edge State: elastic backscattering forbidden by time reversal symmetry, robust against weak disorder.

**Kramers Theorem** : In systems with time-reversal symmetry, every eigenstate \(\ket{u_k}\) has a partner \(\ket{\theta u_k}\) at \(-k\) with the same energy:

$$\hat \theta \ket{u_k} = \alpha \ket{u_k} \ ; \ \hat \theta^2 \ket{u_k} = \alpha^* \theta \ket{u_k}$$

Note that time-reversal \(\hat \theta\) is anti-unitary operator.

QSHE in Graphene(Kane & Mele, PRL95, 226801)

## 第六周

时间反演算符: \(\Theta \psi = e^{\ti \pi S^y/\hbar} \psi^*\) 或对于 spin-1/2:

$$\Theta \begin{bmatrix}\psi_{up} \\ \psi_{down}\end{bmatrix} = \begin{bmatrix}\psi_{down}^* \\ -\psi_{up}^*\end{bmatrix}$$

\(\mathbb{Z}_2\) 不变量:

在保证时间反演不变点的能态兼并前提下, 从 \(\Gamma_a\) 点到 \(\Gamma_b\) 点, Fermi能级会和能带存在若干交点. 对于偶数交点为普通绝缘体, 奇数为拓扑绝缘体.

对于平庸绝缘体, 稳定的表面态数目为0, 称为 \(Z_2=0\). 否则称 \(Z_2=1\).

偶奇性质: 决定Kramer简并对的数目, 因此决定了散射与否. ref: C.Xu-JEM,C.Wu et al, 2006

三维TI: 由2-D TI 堆叠得到 week topological insulator.
对应的 \(\mathbb{Z}_2\) 不变量为费米面内部的Dirac point 数目.
