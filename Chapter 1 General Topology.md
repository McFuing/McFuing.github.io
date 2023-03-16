广义拓扑，简单来说就是空间的定性的性质。
# Chapter1 General Topology
## 导论
### 从初等定义谈起
我们的高等数学或者说是复变函数，在我们学习集合时，经常会引入以下的几个概念：

 - 点$a$的$\delta$邻域：以$a$为圆心，以$\epsilon$为半径的一个开圆即为点$a$的邻域,记为$U_{\delta}\left(  x\right),$即满足不等式$\left\vert z-a\right\vert<\epsilon$的那些点的集合。
 - 内点：点$x$,集合$S$,$x\in S$,存在一个$\delta$邻域使得$U_{\delta}\left(x\right)\subset S,$则称$x$为$S$的内点。
 - 边界点：点$x\notin S$,但是对于$x$的任意的一个$\delta$领域$U_{\delta}\left(x\right)$ 都有：$U_{\delta}\left(  x\right)  \cap S\neq\emptyset$,且$U_{\delta}\left(  x\right) \nsubseteq S$.
据此，在高数中，我们定义了极限($\epsilon-\delta$语言)，连续，导数，微分(解析的含义)；在复变函数中定义了单，复连通域，进而定义了可微性与解析性。

接下来很重要的一个概念：开集：集合$S$的点都是内点。到此我们定义的所有东西似乎都起源于一个东西：我们定义了距离$\left\vert z-a\right\vert$ 的这一概念。也就是当我们在讨论函数的连续性，可微性等解析性质时，依赖于我们定义了一个描述两点间距离的函数
>距离函数可以看作是将$X$集合的一对数对，映射到实线$R$
(数)上，满足以下条件：
$$
\begin{align}
d\left(  p,q\right)  >0;\\
d\left(  p,q\right)  =0\Longleftrightarrow p=q;\\
d\left(  p,q\right)  =d\left(  q,p\right)  ;\\
d\left(  p,r\right)  +d\left(  r,q\right)  \geq d\left(  p,q\right).
\end{align}
$$

$$
\begin{equation}
d\left(  x,y;x_{1},y_{1}\right)  =\sqrt{\left(  x-x_{1}\right)  ^{2}+\left(
y-y_{1}\right) ^{2}}%
\end{equation}
$$
才产生了各种曲线，即对应的就是我们在解析里使用的各种函数。

进一步，来看我们周围的三维欧几里得空间，我们定义一个开球:
$$
\begin{equation}
B_{r}\left(  p\right)  =\left\{  d\left(  q,p\right)  <r\ |\ q\in
E^{3}\right\}
\end{equation}
$$
借此来引入实分析里的子集的有界性，点列的收敛性，$\mathbb{E}^{3}$和其它点集的映射的连续性。那么这里就有一个问题是：实分析里面有多少的结果是依赖于距离的定义
>我们知道，当一个对象里含有一个最小的抽象结构，对于最小结构所引入的概念，那么拿掉这个较大的对象，这个概念也是成立的。反之，不成立。？

在闵氏空间中的距离
$$\begin{equation}
\eta^{2}\left(  p,q\right)  =\left(  p^{0}-q^{0}\right)  ^{2}-\left(
p^{1}-q^{1}\right)  ^{2}-\left(  p^{2}-q^{2}\right)  ^{2}-\left(  p^{3}%
-q^{3}\right)  ^{2}%
\end{equation}
$$
很明显，$\eta^{2}\left(  p,q\right)$可以等于$0$，可以为负，所以我们描述连续等一些性质时，开球是不必须的.

## 拓扑空间
### 开集的引入
Q：在我们的印象里，说到$\mathbb{R}^{n}$与$\mathbb{E}^{n}$我们都会自然的认为这两个所表达都是$n$维空间，但是两者有什么区别呢？我们需要这一节来回答这个问题。

首先需要明确，我们为什么需要开集？实验的测量结果不可避免地要受到精度的影响，相应的一些出现在基本方程的自然常数(如薛定谔方程中的普朗克常数$\hbar$,相对论中的光速$c$,麦克斯韦方程的电子电荷$e$)都不能够被相对精确的测得
>有人可能会说,我们的不确定性原理不就是在约束我们无法测准？Attention!!!不确定性原理并不是说什么力学量都无法测准。你在一个力学量的本征态上去测，是可以测量得到其本征值的。什么是[物理常数](https://en.wikipedia.org/wiki/Physical%5C_constant).

换句话说，我们建立的物理方程的基础是在假定：如果一个物理学量是可接受的，那么必定会有一系列的误差范围内的值是可接受的。
基于此，我们需要思考，物理量属于一个集合，什么样的集合呢？在每一个可接受的值的邻域内都有另外的一个值可以被平等的被接受，以此类推。也就是说，集合被赋予了这样的一个性质：在集合里的点的周围都存在着一个相同类型的集合，我们称其为"开集" ，记住此时的开集在延续我们初等开集的概念。
$$
物理需要开集。
$$
### 何为拓扑?


<!--stackedit_data:
eyJoaXN0b3J5IjpbNDE4NjQxMTcsMTA0OTYxMDU0MywxMDAwMD
U2NjY1XX0=
-->