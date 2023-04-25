## Q-ball 超辐射
### *摘要*
*Q-ball是一类在场中可以相干转动的非拓扑孤立子。由于散射过程涉及两个耦合的模式，我们证明了这些相干转动可以诱导散射波的超辐射。尽管在散射过程中粒子数是守恒的，但两个模式的频率的不匹配性允许对入射波的能量和角动量的的增强。当Q-ball在实空间中转动时，额外的转动超辐射，可能导致更进一步的能量和角动量的增强。我们得到了能量和角动量超辐射发生的准则。而Zel’dovich的对于转动的超辐射准则与Q-ball系统的超辐射准则相矛盾。*

Q-ball作为孤子解[1-3]出现在很多的允许吸引的非线性相互作用的场[4].

我们将会考虑$U(1)$对称性的理论，
$$
\mathcal{L}=-\eta^{\mu\nu}\frac{\partial{\Phi^*}}{\partial{x^\mu}}\frac{\partial{\Phi}}{\partial{x^\nu}},\tag{1}
$$
其中势能$V(|\Phi|)=\mu^2|\Phi|^2-\lambda|\Phi|^4+g|\Phi|^6$作为一个实例。要求当$|\Phi|=0$作为真真空，得到$\lambda>0$以及$\mu^2g>\lambda^2/4$,使用无量纲的变量，$x=\mu x,\Phi=\lambda^{1/2}|\Phi|/\mu$以及$g=\mu^2g/\lambda^2$,这个模型可以重新写为
$$
\mathcal{L}=-\partial_\mu\Phi^*\partial^\mu\Phi-V(|\Phi|),V(|\Phi|)=|\Phi|^2-|\Phi|^4+g|\Phi|^6,\tag{2}
$$
这可以看作是一般的$U(1)$标量场的有效场论展开的低能量的截断（在2+1维重整化）。接下来除了末尾简短讨论3+1维的情况外，我们将会主要集中于2+1维的情况。
在极坐标中，一个通常的Q-ball构型具有如下的形式，
$$
\Phi_{Q}(t,r,\varphi)=\frac{1}{\sqrt{2}}f(r)e^{-i\omega_Q t+i m_Q\varphi },\tag{3}
$$
其中$\omega_Q$是Q-ball在场空间的振荡频率，$\varphi$是方位角。若$m_Q$非零，此构型的实空间的角相速度为$\Omega_Q=\omega_Q/m_Q$。非转动Q-ball是当$m_Q=0$的特殊情况，此时$f(r)$在$r=0$处达到峰值，在径向无穷大时快速降到零。对于$m_Q \neq 0$，$f(r)$将会在一个有限的$r$处达到峰值，在$r\rightarrow 0$以及$r \rightarrow \infty$时近似趋于$0$。在原点处的正则条件为$f(r\rightarrow 0)\propto r^{|m_Q|}$。不失一般性的，我们认为$\omega_Q>0$(对于转动Q-ball，$m_Q>0$)。当Q-ball存在时，$\omega_Q$必须满足$(1-(4g)^{-1})^{1/2}\lesssim \omega_Q<1$(见附录1)。孤立的Q-ball对于小的扰动具有稳定性。但是，在这篇文章中，我们将会证明在波在周围散射的“脏”环境中，Q-ball有不稳定超辐射的倾向。
以此为目的，让我们看一下对Q-ball解附近的运动的扰动方程$\Phi=\Phi_Q+\phi(t,r,\varphi)$:
$$
\Box\phi-U(r)\phi-e^{-2i(\omega_Q t-m_Q\varphi)}W(r)\phi^*=0,\tag{4}
$$
其中$U=\frac{1}{2}(\frac{d^2V}{df^2}+\frac{1}{f}\frac{dV}{df})$, $W=\frac{1}{2}(\frac{d^2V}{df^2}-\frac{1}{f}\frac{dV}{df})$。我们可以看到微扰场$\phi$与时间与角向振荡的相干Q-ball背景相互作用。确实，就像我们将看到的那样，Q-ball凝聚可以增强能量，角动量以及入射波的电荷，发生超辐射。然而，$U$和$W$依赖于$r$使得我们不能直接对空间进行傅里叶展开。
进一步的，我们限制场仅有两个频率的这种最小情况，
$$
\phi=\eta_+(\omega,m,r)e^{-i\omega_+ t+im_+\varphi}+\eta_-(\omega,m,r)e^{-i\omega_- t+im_-\varphi},\tag{5}
$$
其中$\omega_\pm=\omega_Q\pm\omega$，$m_\pm=m_Q\pm m$。普遍解将是这种情况的线性叠加。不同于一个实标量场的超辐射情况，单个频率就能满足最小情况。所以将$\phi$和$\phi^*$之间耦合是我们选择两个模式的原因。模式方程满足下面的方程，
$$
\eta_\pm''+\frac{1}{r}\eta_\pm'+(\omega_\pm^2-U-\frac{m_\pm^2}{r^2})\eta_\pm-W\eta_\mp^{*}=0,\tag{6}
$$
其中$'$代表关于$r$求导。由于$f(r\rightarrow \infty)=0$,我们可以得到$U(r\rightarrow \infty)=1,W(r\rightarrow \infty)=0$。在较大的$r$处，上面的方程约化为$\eta_\pm''+\frac{1}{r}\eta_\pm'+(\omega_\pm^2-1)\eta_\pm \rightarrow0$,这是由
$$
\eta_\pm(\omega,m,r\rightarrow \infty)\rightarrow \frac{A_\pm}{\sqrt{k_\pm r}}e^{ik_\pm r}+\frac{B_\pm}{\sqrt{k_\pm r}}e^{-ik_\pm r},\tag{7}
$$
其中波数$k_\pm=(\omega_\pm^2-1)^{1/2}$。此时，我们感兴趣的是接近与离开Q-ball的散射波。假设两种模式都在传播波，将实条件强加给 $k_\pm$:$|\omega_Q\pm\omega|>1$.不等式右边的$1$来源于标量理论的质量差(本质上，在我们的单位中标量质量$\mu=1$)。由于我们已经认为$\omega_Q>0$，这就意味着$\omega$的物理边界为
$$
|\omega|>\omega_Q+1.\tag{8}
$$
就像在图1中展示的那样，如果$\omega>0$,$A_-,B_+$项代表入射波，$A_+,B_-$项代表出射波，而下标$+(-)$代表正(负)电荷；如果$\omega<0$,波的方向翻转，$-(+)$表示正（负）电荷。
y
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE5MTM4OTEyNjQsMTQyOTczNjc5NywxNj
cwMTQ5ODA5LDE2OTY2MjIyMDAsLTQxNjA4MzM2NiwyMTA1Mzgy
MDQ3XX0=
-->