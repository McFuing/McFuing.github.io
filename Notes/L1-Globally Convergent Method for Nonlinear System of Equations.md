## Shooting Method
### 微分方程和边界条件
我们有一个微分方程组
$$
\frac{dy_i}{dx}=g_i(x,y_1,\dots,y_N),i=1,2,\dots,N\tag{1}
$$
在点$x_1$处，解满足条件
$$
B_{1j}(x_1,y_1,\dots,y_N)=0,i=1,2,\dots,n_1\tag{2}
$$
在点$x_2$满足
$$
B_{2k}(x_2,y_1,\dots,y_N)=0,i=1,2,\dots,n_2\tag{3}
$$
>解微分方程的核心思想是将微分方程看作一种演化，这种演化是由积分来实现的，由初值决定系统的后来的演化结果。

### 打靶法思想及实现
我们先讨论纯粹的打靶法：从$x_1$积分到$x_2$，然后我们希望使得由$x_1$初值演化的结果符合$x_2$边界条件，如图所示：

在初始点$x_1$，需要指定$N$个初值$y_i$，但是要受$n_1$个条件的约束，因此有$n_2=N-n_1$可自由指定的初值。将这些自由指定的变量看作矢量$\bold{V}$的分量，维数为$n_2$。我们已知初始边界条件$B_{1j}$的函数形式，通过改变$\bold{V}$的$n_2$个自由分量，可以反解出$N$个完备的一组初始值$\bold{y}$，使其满足$x_1$处的初始条件，此时我们有$n_1$个未知参量，$n_1=N-n_2$个约束，即（2）可化为
$$
y_i(x_1)=y_i(x_1;V_1,\dots,V_{n_2}),i=1,2,\dots,N\tag{4}
$$
给定一个

## Shooting to a Fitting Point


## Line Searches and Backtracking

<!--stackedit_data:
eyJoaXN0b3J5IjpbNjIwNDI3MzA5LC05MzU1Nzc4ODYsNTQ3OD
MxMzEyLDQxMTQ2MDU5Miw1Njg0NTkwMjUsMTQ5NDQxNDcwOSwx
NDk0NDE0NzA5LC0xMjQ4NDY2MDk1LC0yMDg4NzQ2NjEyXX0=
-->