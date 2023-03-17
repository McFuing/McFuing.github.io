## 引入问题

在狭义相对论中，我们定义四维动量
$$
\begin{align}
p^{\mu}  &  =m\frac{dx^{\mu}}{d\tau}=m\left(  \frac{dt}{d\tau},\frac
{d\mathbf{x}}{d\tau}\right) \\
&  =\left(  \gamma m,\gamma m\mathbf{v}\right)  =\left(  \gamma m,\gamma
\mathbf{p}\right)
\end{align}
$$
至此，所有的结果都是平庸的，不平庸的是
$$
\begin{equation}
E\overset{def}{=}\gamma m
\end{equation}
$$
但是为什么这样定义？

## 分析与解决

相对论性的自由粒子的拉式量
$$
\begin{equation}
L=-m\sqrt{1-\mathbf{v}^{2}}
\end{equation}
$$
对于拉式量(4)关于时间平移不变性$\[\overline{t}=t+\epsilon\]$
相应的广义坐标的变化\begin{equation}
q\left(  t+\epsilon\right)  =q\left(  t\right)  +\epsilon\eta\label{q}%
\end{equation}
且\begin{equation}
\eta=\lim_{\epsilon\rightarrow0}\frac{q\left(  t+\epsilon\right)  -q\left(
t\right)  }{\epsilon}=\dot{q}%
\end{equation}


对于作用量\begin{align}
S\left(  \epsilon\right)   &  =\int_{t_{1}}^{t_{2}}L\left(  q\left(  t\right)
+\epsilon\eta,\dot{q}+\epsilon\dot{η},t\right)  dt\\
S\left(  0\right)   &  =\int_{t_{1}}^{t_{2}}L\left(  q,\dot{q},t\right)  dt
\end{align}
按$\epsilon$展开，\begin{align*}
S\left(  \epsilon\right)  -S\left(  0\right)    & =\int_{t}^{t+\epsilon
}L\left(  q+\epsilon\eta,\dot{q}+\epsilon\dot{η},t\right)  -L\left(
q,\dot{q},t\right)  dt\\
& =\int_{t}^{t+\epsilon}\epsilon\left(  \frac{\partial L}{\partial q}%
\eta+\frac{\partial L}{\partial\dot{q}}\dot{η}\right)  dt\\
& =\epsilon\int_{t}^{t+\epsilon}\frac{\partial L}{\partial q}\eta+\frac{d}%
{dt}\left(  \frac{\partial L}{\partial\dot{q}}\eta\right)  -\eta\frac{d}%
{dt}\left(  \frac{\partial L}{\partial\dot{q}}\right)  dt\\
& =\epsilon\int_{t}^{t+\epsilon}\frac{\partial L}{\partial q}\eta-\eta\frac
{d}{dt}\left(  \frac{\partial L}{\partial\dot{q}}\right)  dt+\epsilon\int%
_{t}^{t+\epsilon}\frac{d}{dt}\left(  \frac{\partial L}{\partial\dot{q}}%
\eta\right)  dt\\
& =\epsilon\int_{t}^{t+\epsilon}\left[  \frac{\partial L}{\partial q}-\frac
{d}{dt}\left(  \frac{\partial L}{\partial\dot{q}}\right)  \right]  \eta
dt+\epsilon\left(  \frac{\partial L}{\partial\dot{q}}\eta\right)  |_{t_{1}%
}^{t_{2}}%
\end{align*}
当$q$满足运动方程时\begin{equation}
S\left(  \epsilon\right)  -S\left(  0\right)  =\epsilon\left(  \frac{\partial
L}{\partial\dot{q}}\eta\right)  |_{t_{1}}^{t_{2}}%
\end{equation}%
\begin{equation}
\left(  \frac{\partial L}{\partial\dot{q}}\eta\right)  |_{t}^{t+\epsilon
}=\frac{S\left(  \epsilon\right)  -S\left(  0\right)  }{\epsilon}\label{pL}%
\end{equation}
即\begin{align}
\lim_{\epsilon\rightarrow0}\frac{S\left(  \epsilon\right)  -S\left(  0\right)
}{\epsilon}  & =\frac{\partial S\left(  \epsilon\right)  }{\partial\epsilon
}|_{\epsilon0}=\int_{t}^{t+\epsilon}\frac{\partial L\left(  \epsilon\right)
}{\partial\epsilon}dt\nonumber\\
& =\int_{t}^{t+\epsilon}\frac{\partial L}{\partial t}dt=L|_{t}^{t+\epsilon
}\label{S}%
\end{align}
联立式(\ref{pL})与式(\ref{S})%
\begin{equation}
\left(  \frac{\partial L}{\partial\dot{q}}\eta\right)  |_{t}^{t+\epsilon
}=L|_{t}^{t+\epsilon}%
\end{equation}
所以守恒荷为\begin{equation}
Q=\frac{\partial L}{\partial\dot{q}}\dot{q}-L
\end{equation}
由式(\ref{L})%
\begin{align}
Q &  =\frac{\partial L}{\partial\mathbf{v}}\mathbf{v}-L=H\nonumber\\
&  =\frac{m\mathbf{v}^{2}}{\sqrt{1-\mathbf{v}^{2}}}+m\sqrt{1-\mathbf{v}^{2}%
}\nonumber\\
&  =\frac{m}{\sqrt{1-\mathbf{v}^{2}}}=\gamma m
\end{align}
可以看出这就是哈密顿量。

<!--stackedit_data:
eyJoaXN0b3J5IjpbNTkwNDU3NDM4LC0yMDg4NzQ2NjEyXX0=
-->