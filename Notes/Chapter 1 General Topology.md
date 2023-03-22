>**广义拓扑，简单来说就是空间的定性性质。**

## 导论

### 从初等定义谈起
我们的高等数学或者说是复变函数，在我们学习集合时，经常会引入以下的几个概念：

 - 点$a$的$\delta$邻域：以$a$为圆心，以$\epsilon$为半径的一个开圆即为点$a$的邻域,记为$U_{\delta}\left(  x\right),$即满足不等式$\left\vert z-a\right\vert<\epsilon$的那些点的集合。
 - 内点：点$x$,集合$S$,$x\in S$,存在一个$\delta$邻域使得$U_{\delta}\left(x\right)\subset S,$则称$x$为$S$的内点。
 - 边界点：点$x\notin S$,但是对于$x$的任意的一个$\delta$领域$U_{\delta}\left(x\right)$ 都有：$U_{\delta}\left(  x\right)  \cap S\neq\emptyset$,且$U_{\delta}\left(  x\right) \nsubseteq S$.
 
据此，在高数中，我们定义了极限($\epsilon-\delta$语言)，连续，导数，微分(解析的含义)；在复变函数中定义了单，复连通域，进而定义了可微性与解析性。
>连续如何定义？如果用$\varepsilon-\delta$语言就是:设$f:\mathbb{R\rightarrow R}$ 是一个函数，$x_{0}\in\mathbb{R}%
,$对于任意的正数$\varepsilon>0,$总可以找到$\delta>0$,使得当 $\left\vert x-x_{0}\right\vert <\delta$时，$\left\vert f\left(  x\right)  -f\left(  x_{0}\right)\right\vert <\varepsilon.$换个角度来看这个定义，$\left\vert
x-x_{0}\right\vert <\delta$说的是存在一个$x_{0}$的邻域$U_{\delta}\left(  x_{0}\right)$;$\left\vert f\left(  x\right)  -f\left(  x_{0}\right)  \right\vert <\varepsilon$说的是对于任意的$f\left(x_{0}\right)$的邻域$V_{\varepsilon}\left(  f\left(x_{0}\right)  \right)$,其中$x_{0}\in U_{\delta}\left(x_{0}\right)$,而任意的$\varepsilon$,存在一个$\delta,$要求的是$f\left(  U\right)  \subset V$

接下来很重要的一个概念：开集，即集合$S$的点都是内点。举个例子：
>Q:对于一个单点集$\left\{a\right\}$,它是不是一个开集？
>>A:不是开集。因为点a不是集合$\left\{a\right\}$的内点。

到此我们定义的所有东西似乎都起源于一个东西：我们定义了距离$\left\vert z-a\right\vert$ 的这一概念。也就是当我们在讨论函数的连续性，可微性等解析性质时，依赖于我们定义了一个描述两点间距离的函数[^0].
[^0]:距离函数可以看作是将$X$集合的一对数对，映射到实线$R$(数)上，满足以下条件：
$$
\begin{aligned}
d\left(  p,q\right)  >0;\\
d\left(  p,q\right)  =0\Longleftrightarrow p=q;\\
d\left(  p,q\right)  =d\left(  q,p\right)  ;\\
d\left(  p,r\right)  +d\left(  r,q\right)  \geq d\left(  p,q\right).
\end{aligned}
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
借此来引入实分析里的子集的有界性，点列的收敛性，$\mathbb{E}^{3}$和其它点集的映射的连续性。那么这里就有一个问题是：实分析里面有多少的结果是依赖于距离的定义[^1]
[^1]:我们知道，当一个对象里含有一个最小的抽象结构，对于最小结构所引入的概念，那么拿掉这个较大的对象，这个概念也是成立的。反之，不成立。

但是，在闵氏空间中的距离是这样定义的：
$$\begin{equation}
\eta^{2}\left(  p,q\right)  =\left(  p^{0}-q^{0}\right)  ^{2}-\left(
p^{1}-q^{1}\right)  ^{2}-\left(  p^{2}-q^{2}\right)  ^{2}-\left(  p^{3}%
-q^{3}\right)  ^{2}%
\end{equation}
$$
很明显，$\eta^{2}\left(  p,q\right)$可以等于$0$，可以为负，所以我们描述连续等一些性质时，距离是不必须的。

## 拓扑空间
Q：在我们的印象里，说到$\mathbb{R}^{n}$与$\mathbb{E}^{n}$我们都会自然的认为这两个所表达都是$n$维空间，但是两者有什么区别呢？我们需要这一节来回答这个问题。
### 开集的引入
首先需要明确，我们为什么需要开集？实验的测量结果不可避免地要受到精度的影响，相应的一些出现在基本方程的自然常数(如薛定谔方程中的普朗克常数$\hbar$,相对论中的光速$c$,麦克斯韦方程的电子电荷$e$)都不能够被相对精确的测得[^2]
[^2]:有人可能会说,我们的不确定性原理不就是在约束我们无法测准？Attention!!!不确定性原理并不是说什么力学量都无法测准。你在一个力学量的本征态上去测，是可以测量得到其本征值的。[什么是物理常数](https://en.wikipedia.org/wiki/Physical%5C_constant).

换句话说，我们建立的物理方程的基础是在假定：如果一个物理学量是可接受的，那么必定会有一系列的误差范围内的值是可接受的。
基于此，我们需要思考，物理量属于一个集合，什么样的集合呢？在每一个可接受的值的邻域内都有另外的一个值可以被平等的被接受，以此类推。也就是说，集合被赋予了这样的一个性质：在集合里的点的周围都存在着一个相同类型的集合，我们称其为"开集" ，记住此时的开集在延续我们初等开集的概念。
$$
物理需要开集
$$
### 何为拓扑?
我们再来看一下初等开集$S$,简单的来说，开集可以看作一些内点的集合，那么开集可以表示为内点的邻域[^邻域]
[^邻域]:内点的邻域可以看作开集$S$的子集，且邻域也是开集

的并集，一个集合可以有无穷多个内点，则可以看作无穷开集的并。那么我们抽象出拓扑的定义

>对于给定的点集S,拓扑就是集合S的满足以下条件的子集族(也可被称为开集):
$$
\begin{aligned}
1.&整个集合S以及空集\emptyset都在这个子集族中;\\
2.&给定有限数量的子集U_{1},U_{2},\cdots,U_{n},他们的交\cap_{i=1}^{n}U_{i}也属于子集族中;\\
3.&给定任意数量(有限或无限)的子集族中的集合，他们的并也属于这个子集族.
\end{aligned}
$$

为什么要求有限个集合的交，仍然属于这个子集族，而不是无限数量的集合相交？如果我们要求无限个集合相交得到的可能就是一个单点集。比如考虑一个点$x_{0}$的同心圆的邻域，并且同心圆不断地缩小，你最后得到的交集的结果是一个单点集合$\left\{x_{0}\right\}$，此时$x_{0}$不是这个单点集的内点，这是一个闭集。闭集当然不在同心圆开集的子集族中。因此集合$S$上的拓扑是包含全集$S$和空集$\emptyset$的$S$的子集的集合，这个集合中的元素有限的交和任意的并都在这个集合中。其中包含了全部子集的子集族称为离散拓扑，只包含了全集与空集的子集族称为平凡拓扑。可以看出，定义拓扑就是在定义集合$S$中哪些是开集，定义拓扑就是在定义定义开集，那么自然的闭集就是定义的开集相对于全集的补集。这个开集的定义是针对点集而言的。

### 拓扑空间

我们先来看一看拓扑空间的定义：
>拓扑空间就是定义了拓扑$T$点集$S$,一般记为$\left(S,T\right)$

但是，从定义可以看出，这个拓扑空间与点集$S$
就只是差了一个定义的拓扑结构，也就是在集合$S$
上定义了开集。有一点很重要：同一个开集可以定义不同的拓扑，而同样的拓扑可以定义在不同的集合上。也即，拓扑空间$\left(
S,T\right)  $%
上的开集不一定是拓扑空间$\left(
S,T^{\prime}\right)  $定义的开集。所以有意义的是拓扑空间，单讲点集与拓扑都是没有意义的。也就是说我们在研究什么极限、连续、解析性质时，是在拓扑空间上而不是简单的在某个点集上。

\begin{example}
[有限空间]%
给定一个点集$S=\left\{  a,b,c,d\right\}
$定义其上的的拓扑$T=\left\{
\left\{  a\right\}  ,\left\{  a,b\right\}  ,\left\{  a,b,d\right\}
,S,\emptyset\right\}  $%
,可以证明满足拓扑的那三条公理化定义。同时我们也可以给出点集$S$%
上的另外一个拓扑$T^{\prime
}=\left\{  \left\{  b,c,d\right\}  ,\left\{  c,d\right\}  ,\left\{  c\right\}
,\emptyset,S\right\}  $%
可以看出拓扑$T^{\prime}$%
上的开集在拓扑$T$的意义下是闭集！
\end{example}

我们之前说过有了拓扑就有了开集，有了开集就能研究分析范畴里的东西，那么我们可以看看如何在拓扑(推广化的开集)中定义邻域。给定一个点$p\in
S$,任意的集合$U$%
都包含一个属于T的拓扑,且集合$U$%
包含$p$,称集合$U$为点$p$%
的邻域。其中$U$%
不一定要是拓扑$T$%
中的开集，所以任意的点都至少包含一个邻域就是$S$%
.

我们再来看看对于最开始的欧几里得空间，

\subsection{小结}
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTEzODYwODc3Miw0MjUwOTE2NDIsLTEzMj
A0MjcyODIsLTg5NzAwNjMxNywtNzc0NDM1MzE5LDEzNzg3MTk2
MzcsMTk3Mjc2MzA3LC0xOTA5NjA4Nzk1LC0xNDgxMTQ4Mjc5LC
0xMjU2ODA4OTI2LDM4MDM3ODI0OSwtMzY3NzAyOTM4LDE4MzE5
NDczMCwxNzU4Mjk0ODc0LC0yMDU4NTA5NzY2LDE0MTIxODg1Mi
w3ODMwMjc0NTgsMTY5NjczNDM1MywxMzAwNDM4OTI1LDQxODY0
MTE3XX0=
-->