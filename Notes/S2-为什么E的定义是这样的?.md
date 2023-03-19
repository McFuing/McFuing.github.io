>这个问题来自于周双勇老师的广义相对论的课程思考（一个简单的理论力学习题）
## 引入问题

在狭义相对论中，我们定义四维动量
$$
\begin{align}
p^{\mu}  &  =m\frac{dx^{\mu}}{d\tau}=m\left(  \frac{dt}{d\tau},\frac
{d\mathbf{x}}{d\tau}\right) \tag{1}\\
&  =\left(  \gamma m,\gamma m\mathbf{v}\right)  =\left(  \gamma m,\gamma
\mathbf{p}\right)\tag{2}
\end{align}
$$
至此，所有的结果都是平庸的，不平庸的是
$$
\begin{equation}
E\overset{def}{=}\gamma m \tag{3}
\end{equation}
$$
但是为什么这样定义？

## 分析与解决

相对论性的自由粒子的拉式量
$$
\begin{equation}
L=-m\sqrt{1-\mathbf{v}^{2}} \tag{4}
\end{equation}
$$
对于拉式量(4)关于时间平移不变性$\overline{t}=t+\epsilon$相应的广义坐标的变化
$$
\begin{equation}
q\left(  t+\epsilon\right)  =q\left(  t\right)  +\epsilon\eta \tag{5}
\end{equation}
$$
且
$$
\begin{equation}
\eta=\lim_{\epsilon\rightarrow0}\frac{q\left(  t+\epsilon\right)  -q\left(
t\right)  }{\epsilon}=\dot{q} \tag{6}
\end{equation}
$$

对于作用量
$$
\begin{align}
S\left(  \epsilon\right)   &  =\int_{t_{1}}^{t_{2}}L\left(  q\left(  t\right)
+\epsilon\eta,\dot{q}+\epsilon\dot{η},t\right)  dt \tag{7}\\
S\left(  0\right)   &  =\int_{t_{1}}^{t_{2}}L\left(  q,\dot{q},t\right)  dt \tag{8}
\end{align}
$$
按$\epsilon$展开，
$$
\begin{align}
S\left(  \epsilon\right)  -S\left(  0\right)    \tag{9}& =\int_{t}^{t+\epsilon
}L\left(  q+\epsilon\eta,\dot{q}+\epsilon\dot{η},t\right)  -L\left(
q,\dot{q},t\right)  dt \\
&\tag{10} =\int_{t}^{t+\epsilon}\epsilon\left(  \frac{\partial L}{\partial q}%
\eta+\frac{\partial L}{\partial\dot{q}}\dot{η}\right)  dt\\
& \tag{11}=\epsilon\int_{t}^{t+\epsilon}\frac{\partial L}{\partial q}\eta+\frac{d}%
{dt}\left(  \frac{\partial L}{\partial\dot{q}}\eta\right)  -\eta\frac{d}%
{dt}\left(  \frac{\partial L}{\partial\dot{q}}\right)  dt\\
& \tag{12}=\epsilon\int_{t}^{t+\epsilon}\frac{\partial L}{\partial q}\eta-\eta\frac
{d}{dt}\left(  \frac{\partial L}{\partial\dot{q}}\right)  dt+\epsilon\int%
_{t}^{t+\epsilon}\frac{d}{dt}\left(  \frac{\partial L}{\partial\dot{q}}%
\eta\right)  dt\\
& \tag{13}=\epsilon\int_{t}^{t+\epsilon}\left[  \frac{\partial L}{\partial q}-\frac
{d}{dt}\left(  \frac{\partial L}{\partial\dot{q}}\right)  \right]  \eta
dt+\epsilon\left(  \frac{\partial L}{\partial\dot{q}}\eta\right)  |_{t_{1}%
}^{t_{2}}
\end{align}
$$
当$q$满足运动方程时
$$
\begin{equation}
S\left(  \epsilon\right)  -S\left(  0\right)  =\epsilon\left(  \frac{\partial
L}{\partial\dot{q}}\eta\right)  |_{t_{1}}^{t_{2}} \tag{14}
\end{equation}
$$
$$
\begin{equation}
\left(  \frac{\partial L}{\partial\dot{q}}\eta\right)  |_{t}^{t+\epsilon
}=\frac{S\left(  \epsilon\right)  -S\left(  0\right)  }{\epsilon}  \tag{15}
\end{equation}
$$
即
$$
\begin{align}
\lim_{\epsilon\rightarrow0}\frac{S\left(  \epsilon\right)  -S\left(  0\right)
}{\epsilon}  & =\frac{\partial S\left(  \epsilon\right)  }{\partial\epsilon
}|_{\epsilon0}=\int_{t}^{t+\epsilon}\frac{\partial L\left(  \epsilon\right)
}{\partial\epsilon}dt\nonumber\\  \tag{16}
& =\int_{t}^{t+\epsilon}\frac{\partial L}{\partial t}dt=L|_{t}^{t+\epsilon
}%
\end{align}
$$
联立式(15)与式(16)
$$
\begin{equation}
\left(  \frac{\partial L}{\partial\dot{q}}\eta\right)  |_{t}^{t+\epsilon}=L|_{t}^{t+\epsilon}  \tag{17}
\end{equation}
$$
所以守恒荷为
$$
\begin{equation}
Q=\frac{\partial L}{\partial\dot{q}}\dot{q}-L  \tag{18}
\end{equation}
$$
由式(4)
$$
\begin{align}
Q &  =\frac{\partial L}{\partial\mathbf{v}}\mathbf{v}-L=H\nonumber\\  \tag{19}
&  =\frac{m\mathbf{v}^{2}}{\sqrt{1-\mathbf{v}^{2}}}+m\sqrt{1-\mathbf{v}^{2}%
}\nonumber\\  \tag{20}
&  =\frac{m}{\sqrt{1-\mathbf{v}^{2}}}=\gamma m
\end{align}
$$
可以看出这就是哈密顿量.
>Noether定理要求的时间平移不变性对应能量守恒。

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE0NjQ5Mzc1OTYsLTc3NTM5NDk2NSw5Mz
IwMTEsODEyMDIyNDAwLC0yMDg4NzQ2NjEyXX0=
-->