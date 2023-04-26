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
有了这些约定，我们通过将其看作关于$r$的初值问题解方程(6) 。我们可以设定在$r=0$附近的$\eta_+,\eta_-$的值，然后通过方程（6）演化到较大的$r$去获得$A_\pm,B_\pm$。在原点附近我们要求$\eta_\pm(\omega,m,r\rightarrow 0)\rightarrow F_\pm(k_\pm r)^{|m_\pm|}$。$F_\pm$是复常数，用来提供初始条件来解这个系统。除此之外，因为这个系统是线性的，如果$(\eta_+,\eta_-)$是一个解，那么$(\zeta\eta_+,\zeta^*\eta_-)$也是解，其中$\zeta$是复常数。这就意味着我们可以重新标度这个常数(即$F_+$)归一，在$r\rightarrow0$时选择下面的初始条件：
$$
\eta_\pm(m,r)=(k_+r)^{|m_+|,\eta_-=F_-(k_-r)^{|m_-|}}.\tag{9}
$$
对于每一个$F_-$,初值问题都会给出一组$A_+,A_-,B_+,B_-$.因此，普遍的，我们有两个入射和出射波。如果我们想要仅仅一个入射波，我们可以使用打靶法去调整$F_-$使得当$\omega>0$时，$A_-=0$或$B_-=0$,(由于方程的对称性，在$r$较大时，让入射的$\eta_+$模式为0并不给出新的结果。) 。求解方程的数值求解方案详细放在附录2.
首先，为了更好监视Q-ball如何改变入射波，我们可以定义一些量。首先，我们可以看在远离原点环形区域的平均能量(从$r_1$到$r_2$)：
$$
\begin{aligned}
E_\circledcirc=&\frac{1}{r_2-r_1} \int_{r_1}^{r_2}rdr\langle|\partial_t\phi|^2+|\partial_r\phi|^2+|\phi|^2\rangle,\tag{10}\\
=&2\frac{\omega_+^2}{k_+}(|A_+|^2+|B_+|^2)+2\frac{\omega_-^2}{k_-}(|A_-|^2+|B_-|^2),
\end{aligned}
$$
其中$r_2-r_1$至少包含一个最长波的完全空间振荡周期，$\langle\rangle$是若干振荡的时间平均值，仅保留领先阶。我们使用微扰场去计算能量是因为Q-ball构型在较大的$r$快速趋于$0$，振幅因子可以被定义为出射场能量与入射场能量的比值，
$$
\mathcal{A}_E=\left(\frac{\frac{\omega_+^2}{k_+}|A_+|^2+\frac{\omega_-^2}{k_-}|B_-^2|}{\frac{\omega_+^2}{k_+}|B_+|^2+\frac{\omega_-^2}{k_-}|A_-^2|}\right)^{sign(\omega)},\tag{11}
$$
其次，我们也可以监视波的角动量在散射过程中是如何改变的。角动量密度为$T^{t}{}_{\varphi}=-\partial_t\Phi^*\partial_\varphi\Phi-\partial_t\Phi\partial_\varphi\Phi^*$,在远离原点的环形区域中取平均包括时间平均，领先阶为
$$
\begin{aligned}
L_\circledcirc=&\frac{-1}{r_2-r_1}\int^{r_2}_{r_1}rdr\left<\partial_t\phi^*\partial_\varphi\phi+\partial_t\phi\partial_\varphi\phi^*\right>\tag{12}\\
=&2(|A_+|^2+|B_+|^2)\frac{\omega_+m_+}{k_+}+2(|A_-|^2+|B_-|^2)\frac{\omega_-m_-}{k_-}.
\end{aligned}
$$
角动量的振幅因子为
$$
\mathcal{A}_L=\left(\frac{\frac{\omega_+m_+}{k_+}|A_+|^2+\frac{\omega_-m_-}{k_-}|B_-|^2}{\frac{\omega_+m_+}{k_+}|B_+|^2+\frac{\omega_-m_-}{k_-}|A_-|^2}\right)^{sign(\omega)}
$$
我们想要看到粒子流在散射过程中是如何变化的。粒子流在远离原点的环形区域的平均以及时间平均为$N_\circledcirc=2(|A_+|^2+|B_+|^2+|A_-|^2+|B_-|^2)$,振幅因子为$\mathcal{A}_N=\left((|A_+|^2+|B_-|^2)/(|B_+|^2+|A_-|^2)\right)^{sign(\omega)}$.
但是，对于模式$\eta_+,\eta_-$的$U(1)$对称性，我们总是有$\mathcal{A}_N=1$,为了去证明这个问题，注意到运动方程可以通过下面的拉格朗日量得到，
$$
L(\eta,\eta')=\sum_{s=\pm}\left[(|\sqrt{r}\eta_s)'|^2-r(\omega_s^2-U-\frac{4m_s^2-1}{4r^2})|\eta_s|^2\right]+rW(\eta^*_+\eta^*_-+\eta_+\eta_-)\tag{14}
$$
把$r$看作“时间”，拉式量在$U(1)$变换下是不变的，即
$$
\eta_+=e^{i\alpha}\eta_+,\eta_-=e^{-i\alpha}\eta_-,\alpha=const.\tag{15}
$$
对应$U(1)$对称性的“诺特荷”为
$$
M_\eta=ir(\eta^*_+{'}\eta_+-\eta^*_+\eta_+{'})-ir(\eta^*_-{'}\eta_--\eta^*_-\eta_-{'})\tag{16}
$$
满足$\partial{r}M_\eta=0$,意味着$M_\eta$是独立于$r$的。在较大的$r$处，代入渐近解(7),我们可以得到领先阶，$M_{\eta}=2(|A_+|^2-|B_+|^2-|A_-|^2+|B_-|^2)$.另外一方面，因为$\eta_\pm$在原点$r=0$是解析的，所以我们可以得到$M_\eta=0$.这就得到了对于一般的入射波和出射波，在散射过程中的粒子数守恒
$$
|A_+|^2+|B_-|^2=|B_+|^2+|A_-|^2\tag{17}
$$
尽管在散射过程中粒子数守恒，由于频率$\omega$和Q-ball的频率$\omega_Q$,我们仍然可以有波能量的吸收与增强.事实上，结合约束(17)和方程(11) ，我们可以看到描述能量的吸收与增强的阈值频率$\omega_E$，即当$\mathcal{A}_E=1$时，给出$\omega_+^2/k_+=\omega^2_-/k_-$,即
$$
\frac{(\omega_Q+\omega_E)^2}{\sqrt{(\omega_Q+\omega_E)^2-1}}=\frac{(\omega_Q-\omega_E)^2}{\sqrt{(\omega_Q-\omega_E)^2-1}}\tag{18}
$$
也即是能量的超辐射判据出现在$\omega_E$。类似的，在方程(13)中，我们可以看到对于一个角动量模式$m_L$，代表角动量的吸收与增强的阈值频率$\omega_L$,即当$\mathcal{A}_L=1$时
$$
\frac{(\omega_Q+\omega_L)(m_Q+m_L)}{\sqrt{(\omega_Q+\omega_L)^2-1}}=\frac{(\omega_Q-\omega_L)(m_Q-m_L)}{\sqrt{(\omega_Q-\omega_L)^2-1}}\tag{19}
$$
#### 非转动Q-ball 
让我们看一下对于仅仅有一个入射波$\eta_+(m=0)$，能量振幅因子$\mathcal{A}_E$随入射频率$\omega$和背景$\omega_Q$如何变化，如图2所示。(如果我们仅仅有入射$\eta_-$波，放大曲线将会是图2的$\omega\rightarrow-\omega$的翻转)。从判据(18),我们可以知道超辐射发生的条件为
$$
\omega<-|\o|
$$
<!--stackedit_data:
eyJoaXN0b3J5IjpbNDYwODM5MjE0LC03ODEwMjM3MzUsMTE4Nz
E1NTQwMywtMTM0Njk2NDAwMiwxMzUwNzM3MDAsLTE0MzUzMTkx
MDQsLTE4MzU2MDYxMzQsMTQyOTczNjc5NywxNjcwMTQ5ODA5LD
E2OTY2MjIyMDAsLTQxNjA4MzM2NiwyMTA1MzgyMDQ3XX0=
-->