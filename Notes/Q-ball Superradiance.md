## Q-ball 超辐射
### *摘要*
*Q-ball是一类在场中可以相干转动的非拓扑孤立子。由于散射过程涉及两个耦合的模式，我们证明了这些相干转动可以诱导散射波的超辐射。尽管在散射过程中粒子数是守恒的，但两个模式的频率的不匹配性允许对入射波的能量和角动量的的增强。当Q-ball在实空间中转动时，额外的转动超辐射，可能导致更进一步的能量和角动量的增强。我们得到了能量和角动量超辐射发生的准则。而Zel’dovich的对于转动的超辐射准则与Q-ball系统的超辐射准则相矛盾。*

Q-ball作为孤子解[1-3]出现在很多的允许吸引的非线性相互作用的场[4].

我们将会考虑$U(1)$对称性的理论，
$$
\mathcal{L}=-\eta^{\mu\nu}\frac{\partial{\Phi^*}}{\partial{x^\mu}}\frac{\partial{\Phi}}{\partial{x^\nu}}\tag{1}
$$
其中势能$V(|\Phi|)=\mu^2|\Phi|^2-\lambda|\Phi|^4+g|\Phi|^6$作为一个实例。要求当$|\Phi|=0$作为真真空，得到$\lambda>0$以及$\mu^2g>\lambda^2/4$,使用无量纲的变量，$x=\mu x,\Phi=\lambda^{1/2}|\Phi|/\mu$以及$g=\mu^2g/\lambda^2$,这个模型可以重新写为
$$
\mathcal{L}=-\partial_\mu\Phi^*\partial^\mu\Phi-V(|\Phi|),V(|\Phi|)=|\Phi|^2-|\Phi|^4+g|\Phi|^6\tag{2}
$$
这可以看作是一般的$U(1)$标量场的有效场论展开的低能量的截断（在2+1维重整化）。接下来除了末尾简短讨论3+1维的情况外，我们将会主要集中于2+1维的情况。
在极坐标中，一个通常的Q-ball构型具有如下的形式，
$$
\Phi_{Q}(t,r,\varphi)=\frac{1}{\sqrt{2}}f(r)e^{-i\omega_Q t+i m_Q\varphi }\tag{3}
$$
其中$\omega_Q$是Q-ball在场空间的振荡频率，$\varphi$是方位角。若$m_Q$非零，此构型的实空间的角相速度为$\Omega_Q=\omega_Q/m_Q$。非转动Q-ball是当$m_Q=0$的特殊情况，此时$f(r)$在$r=0$处达到峰值，在径向无穷大时快速降到零。对于$m_Q \neq 0$，$f(r)$将会在一个有限的$r$处达到峰值，在$r\rightarrow 0$以及$r \rightarrow \infty$时近似趋于$0$。在原点处的正则条件为$f(r\rightarrow 0)\propto r^{|m_Q|}$。不失一般性的，我们认为$\omega_Q>0$(对于转动Q-ball$m_Q>0$)。当Q-ball存在时，$\omega_Q$必须满足$(1-(4g)^{-1})^{1/2}\lesssim \omega_Q<1$(见附录1)。孤立的Q-ball对于小的扰动具有稳定性。但是，在这篇文章中，我们将会证明在波在周围散射的“脏”环境中，Q-ball有不稳定超辐射的倾向。
以此为目的，让我们看一下对Q-ball解附近的运动的扰动方程$\Phi=\Phi_Q+\phi(t,r,\varphi)$:
$$
\Box\phi-U(r)\phi-e^{-2i(\omega_Q t-m_Q\varphi)}W(r)\phi^*=0\tag{4}
$$
其中$U=\frac{1}{2}(\frac{d^2V}{df^2}+\frac{1}{f}\frac{dV}{df})$, $W=\frac{1}{2}(\frac{d^2V}{df^2}-\frac{1}{f}\frac{dV}{df})$。我们可以看到微扰场$\phi$与时间与角向振荡的相干Q-ball背景相互作用。确实，就像我们将看到的那样，Q-ball凝聚可以增强能量，角动量以及入射波的电荷，发生超辐射。然而，$U$和$W$依赖于$r$使得我们不能直接对空间进行傅里叶展开。
进一步的，我们限制场仅有两个频率的这种最小情况，
$$
\phi=\eta_+(\omega,m,r)e^{-i\omega_+ t+im_+\varphi}+\eta_-(\omega,m,r)e^{-i\omega_- t+im_-\varphi}\tag{5}
$$


<!--stackedit_data:
eyJoaXN0b3J5IjpbNDUzNzAzNzYxLDE2NzAxNDk4MDksMTY5Nj
YyMjIwMCwtNDE2MDgzMzY2LDIxMDUzODIwNDddfQ==
-->