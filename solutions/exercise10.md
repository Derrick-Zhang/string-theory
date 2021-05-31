# Homework 10

## Problem 1

The OPEs are
$$
H(z)H(0) \sim - \ln z, \quad \psi^i(z)\psi^j(0) \sim \delta^{ij}/z~.
$$
Define the complex fermion,
$$
\psi(z) = \frac{1}{\sqrt{2}}(\psi^1(z) + i \psi^2(z)), \quad \bar\psi(z) = \frac{1}{\sqrt{2}}(\psi^1(z) - i \psi^2(z))~.
$$
We can calculate the OPE,
$$
\psi(z) \bar \psi(0) =  \frac12(\psi^1(z)+ i \psi^2(z))(\psi^1(0)-i\psi^2(0)) \sim \frac1z~.
$$
Similarly,
$$
\bar \psi(z) \psi(0) \sim \frac 1z.
$$
Moreover,
$$
:\!e^{iH(z)}\!:\,:\!e^{-iH(0)}\!: \, = \exp(-\ln z) :\!e^{iH(z)} e^{-iH(0)}\!:\,\sim \frac 1z~.
$$
Similarly,
$$
:\!e^{-iH(z)}\!:\,:\!e^{iH(0)}\!: \,\sim \frac 1z~.
$$
We can calculate
$$
\psi(z) \psi \bar \psi(0) \sim - \psi(0)/z, \quad \bar \psi(z) \psi\bar\psi(0)  \sim \bar \psi(0) /z~.
$$
And
$$
:\!e^{iH(z)}\!: i \partial H(0) = :\!\sum_{n} \frac{1}{n!}(iH(z))^n\!: i \partial H(0) \sim - :\!e^{iH(0)}\!: /z, \quad :\!e^{-iH(z)}\!: i \partial H(0)  \sim  :\!e^{-iH(0)}\!: /z
$$
The energy momentum tensor is
$$
T_H(z) = - \frac 12  :\partial H(z) \partial H(z):, \quad T_\psi(z) =-\frac 12 [ \psi(z) \partial\bar \psi(z) + \bar \psi(z) \partial \psi(z)]~.
$$
Therefore, the $TT$ OPE is given by
$$
T_H(z) T_H(0) \sim \frac 14\left(\frac{2}{z^4} -4\frac{:\partial H(0) \partial H(0):}{z^2} - 4 \frac{:\partial^2H(0)\partial H(0):}{z}\right)\sim \frac{1}{2z^4} + \frac{2 T_H(0)}{z^2}+ \frac{\partial T_H(0)}{z}~.\\
$$
For another $TT$ OPE, we can calculate that
$$
\psi(z) \partial\bar \psi(z)  \psi(0) \partial \bar\psi(0) \sim -\frac{1}{z^4} - \frac{2 \psi \partial \bar \psi}{z^2} - \frac{\partial(\psi \partial \bar \psi)}{z}~.\\
\psi(z) \partial\bar \psi(z) \bar \psi(0) \partial \psi(0) \sim \frac{2}{z^4} + \frac{2\psi \bar \psi}{z^3} - \frac{2 \bar\psi \partial \psi}{z^2} - \frac{\partial(\bar \psi \partial \psi)}{z}~.\\
\bar \psi(z) \partial \psi(z)  \psi(0) \partial \bar\psi(0) \sim \frac{2}{z^4}-\frac{2\psi \bar \psi}{z^3} - \frac{2 \psi \partial \bar \psi}{z^2} - \frac{\partial(\psi \partial \bar \psi)}{z}~.\\
\bar\psi(z) \partial \psi(z) \bar \psi(0) \partial\psi(0) \sim -\frac{1}{z^4} - \frac{2 \bar\psi \partial \psi}{z^2} - \frac{\partial(\bar\psi \partial \psi)}{z}~.\\
$$
Therefore, we can obtain,
$$
T_\psi(z) T_\psi(0) \sim \frac{1}{2z^4} + \frac{2T_\psi(0)}{z^2} + \frac{\partial T_\psi(0)}{z}~.
$$
We can also calculate OPE,
$$
T_H(z)  :e^{iH(0)}: \sim \frac{1}{2z^2} :e^{i H(0)}: + \frac{1}{z} :\partial e^{iH(0)}:~,\\
T_\psi(z) \psi(0) \sim -\frac12 \psi(z) (-1/z^2)  + \frac 12 \partial\psi(z) / z \sim\frac{1}{2z^2} \psi(0) + \frac1z \partial \psi(0)~.
$$
Similarly,
$$
T_H(z) :e^{-i H (0)}: \sim \frac{1}{2z^2} :e^{-i H(0)}: + \frac 1 z :\partial e^{-i H(0)}:~,\\
T_\psi(z) \bar \psi(0) \sim \frac{1}{2z^2} \bar\psi(0) + \frac 1z \partial \bar \psi(0)~.
$$
Also,
$$
T_H(z)  i \partial H(0) \sim \frac{1}{z^2} i \partial H(0) + \frac 1z i \partial^2 H(0)~,\\
T_\psi(z) \psi\bar\psi(0) \sim \frac{1}{2 z^3} + \frac{\psi\bar\psi(0)}{2z^2} + \frac{\partial(\psi\bar\psi)}{2z} - \frac{1}{2z^3} + \frac{\psi \bar \psi(0)}{2z^2} + \frac{\partial (\psi \bar\psi)}{2z} = \frac{1}{z^2} \psi \bar\psi(0) + \frac{1}{z} \partial (\psi \bar \psi)~.
$$
Therefore,
$$
:\!e^{iH}\!:\, \cong \psi, \quad :\!e^{-iH}\!:\, \cong \bar\psi, \quad i \partial H \cong \psi \bar \psi, \quad T_H \cong T_\psi~.
$$

---

The partition function is 
$$
Z = \frac{1}{|\eta(\tau)|^2} \sum_{n,w} q^{\frac{\alpha'}{4}\left(\frac n R + \frac{w R}{\alpha'}\right)^2} \bar q^{\frac{\alpha'}{4} \left(\frac n R - \frac{w R}{\alpha'}\right)^2}~.
$$
When $R = \sqrt{\alpha'/2}$, we have
$$
Z =\frac{1}{|\eta(\tau)|^2} \sum_{n,w} q^{\frac{\alpha'}{4}\left(\frac n R + \frac{w R}{\alpha'}\right)^2} \bar q^{\frac{\alpha'}{4} \left(\frac n R - \frac{w R}{\alpha'}\right)^2} = \frac{1}{|\eta(\tau)|^2} \sum_{n,w} q^{\frac{1}{2}\left(n + \frac{w}{2}\right)^2} \bar q^{\frac{1}{2} \left(n- \frac{w}{2}\right)^2}~.
$$
Consider $w$ is even or odd, we have
$$
\sum_{n,w} q^{\frac{1}{2}\left(n + \frac{w}{2}\right)^2} \bar q^{\frac{1}{2} \left(n- \frac{w}{2}\right)^2} = \sum_{n,k} q^{\frac12(n+k)^2} \bar q^{\frac 12(n-k)^2} + \sum_{n,k} q^{\frac{1}{2}(n+k + 1/2)^2} \bar q^{\frac 12 (n-k-1/2)^2}~.
$$
Now consider the first sum, write $m = n+k$, and $n = n-k$, $m$ and $n$ are both odd or even, we have
$$
\sum_{m,n \equiv 0 {~\rm mod}~2} q^{\frac{m^2}{2}} \bar q ^{\frac{n^2}{2}} + \sum_{m,n \equiv 1 {~\rm mod}~2} q^{\frac{m^2}{2}} \bar q ^{\frac{n^2}{2}}
$$
Also consider
$$
\frac12\left|\sum_n q^{n^2/2}\right|^2 + \frac12\left|\sum_n (-1)^nq^{n^2/2}\right|^2 = \sum_{m,n} q^{\frac{m^2}{2} } \bar q^{\frac{n^2}{2}} \frac12(1+ (-1)^{m+n})~.
$$
Only when $m$ and $n$ are both even or odd, the summand doesn't vanish. And this part is the same as above.

Now consider
$$
\sum_{n,k}q^{\frac12(n+k+1/2)^2} \bar q^{\frac 12(n-k-1/2)^2} = \sum_{m,n} q^{\frac12(m+1/2)^2} \bar q^{\frac12 (n- 1/2)^2}~,
$$
where $m$ and $n$ are both even or odd.
$$
\frac 12 \left|\sum_n q^{\frac 12(n+1/2)^2}\right|^2 = \frac{1}{2} \sum_m q^{\frac 12(m+ 1/2)^2} \sum_n \bar q^{\frac12 (n- 1/2)^2}
$$
One thing to note is that $\sum_m q^{\frac12(m+ 1/2)^2}$ is the same for $m$ odd and $m$ even; for example, change $k$ to $-1-s$,
$$
\sum_k q^{\frac12(2k + 1 + 1/2)^2} = \sum_s q^{\frac{1}{2}(2s +1/2)^2}~.
$$
Therefore, in conclusion, the partition function can be written as
$$
Z = \frac{1}{2 |\eta(\tau)|^2} \left(\left|\sum_n q^{n^2/2}\right|^2 + \left|\sum_n (-1)^nq^{n^2/2}\right|^2 + \left|\sum_n q^{\frac 12(n+1/2)^2}\right|^2\right)~.
$$

---

On the other hand,
$$
\sum_n q^{\frac{n^2}{2}} = \prod_{m = 1}^\infty (1-q^m) (1+ q^{m-\frac12})^2=\vartheta_3(\tau) ~,\\
\sum_{n}(-1)^n q^{\frac{n^2}{2}} = \prod_{m=1}^\infty(1-q^m)(1-q^{m-\frac12})^2 = \vartheta_4(\tau)~,\\
\sum_{n} q^{\frac12 (n + 1/2)^2} = 2  q^{\frac 1 8}\prod_{m=1}^\infty(1-q^m)(1+q^m)^2 = \vartheta_2(\tau) ~.
$$
Then the partition function is
$$
Z = \frac 12 \left(\left|\frac{\vartheta_2(\tau)}{\eta(\tau)}\right|^2 + \left|\frac{\vartheta_3(\tau)}{\eta(\tau)}\right|^2+ \left|\frac{\vartheta_4(\tau)}{\eta(\tau)}\right|^2\right)~.
$$

## Problem 2

### Problem 2.1

$$
\Pi_I = \frac{\delta S}{\delta \dot X^I} = \frac{1}{2\pi \alpha'}(\delta_{IJ}\dot X^J + B_{IJ}X'^J )~.
$$

Then the center-of-mass momentum is
$$
\pi_I = \int_0^{2\pi} d \sigma \Pi_I = \frac{1}{2\pi \alpha'}\int_0^{2\pi} d \sigma (\dot X^I + B_{IJ} X'^J)
$$
We have
$$
X^I = x^I + \bar x^I +\sqrt{\frac{\alpha'}{2}} p^I_R (\tau + \sigma) +\sqrt{\frac{\alpha'}{2}} p^I_L (\tau - \sigma) + i \sqrt{\frac{\alpha'}{2}} \sum_{m \neq 0} \frac1 m \left(\alpha^I_m e^{-im(\tau+ \sigma)} + \bar \alpha^I_m e^{-im(\tau - \sigma)}\right)
$$
and
$$
\dot X^I = \sqrt{\frac{\alpha'}{2}} p^I_R  +\sqrt{\frac{\alpha'}{2}} p^I_L  +  \sqrt{\frac{\alpha'}{2}} \sum_{m \neq 0}  \left(\alpha^I_m e^{-im(\tau+ \sigma)} + \bar \alpha^I_m e^{-im(\tau - \sigma)}\right)
$$
and
$$
X'^I = \sqrt{\frac{\alpha'}{2}} p^I_R  -\sqrt{\frac{\alpha'}{2}} p^I_L  +  \sqrt{\frac{\alpha'}{2}} \sum_{m \neq 0}  \left(\alpha^I_m e^{-im(\tau+ \sigma)} - \bar \alpha^I_m e^{-im(\tau - \sigma)}\right)~.
$$
This leads to
$$
\pi_I = \frac{1}{\alpha'} \sqrt{\frac{\alpha'}{2}} (p_R^I + p_L^I + B_{IJ}p_R^J-B_{IJ}p_L^J)~.
$$
Moreover, we have boundary condition,
$$
X^I(\sigma+2\pi, \tau) = X^I(\sigma, \tau) + 2\pi W^I~,
$$
which leads to
$$
\sqrt{\frac{\alpha'}{2}}(p^I_R - p_L^I) = W^I~.
$$
Therefore, we obtain,
$$
\sqrt{\frac{\alpha'}{2}} p_R^I = \frac12\left(\alpha' \pi_I - B_{IJ} W^J + W^I\right)\\
\sqrt{\frac{\alpha'}{2}} p_L^I = \frac12\left(\alpha' \pi_I - B_{IJ} W^J - W^I\right)
$$
Simplify it further, we obtain,
$$
p_R^I = \sqrt{\frac{\alpha'}{2}}\left(\pi_I +(\delta_{IJ}- B_{IJ}) \frac{W^J}{\alpha'}\right)\\
p_L^I = \sqrt{\frac{\alpha'}{2}}\left(\pi_I -(\delta_{IJ}+ B_{IJ}) \frac{W^J}{\alpha'}\right)
$$

### Problem 2.2

We have
$$
(p_I)_{R,L} = e^{*i}_I\left(\sqrt{\frac{\alpha'}{2}} m_i \pm \frac{1}{\sqrt{2\alpha'} } g_{ij}n^j - \frac{1}{\sqrt{2\alpha'} } b_{ij} n^j\right)~.
$$
Then, using $e^{*i}_Ie^{*j}_I = (g^{-1})_{ij}$
$$
p_R^2 = \frac{\alpha'}{2} e^{*i}_I  e^{*j}_I m_i m_j +\frac{1}{2\alpha'} e^{*i}_I (g_{ij}-b_{ij})n^je^{*k}_I (g_{kl}-b_{kl})n^l +  e^{*i}_I m_ie^{*k}_I (g_{kl}-b_{kl})n^l\\
= \frac{\alpha'}{2} {\bf m}^T {\bf g}^{-1}{\bf m} + \frac{1}{2\alpha'}{\bf n}^T({\bf g}^T - {\bf b}^T){\bf g}^{-1}({\bf g} - {\bf b}){\bf n} + {\bf m}^T{\bf g}^{-1}({\bf g}- {\bf b}){\bf n}\\
= \frac{\alpha'}{2} {\bf m}^T {\bf g}^{-1}{\bf m} + \frac{1}{2\alpha'}{\bf n}^T({\bf g}^T - {\bf b}^T){\bf g}^{-1}({\bf g} - {\bf b}){\bf n} + {\bf m}^T{\bf g}^{-1}({\bf g}- {\bf b}){\bf n}
$$
Similarly,
$$
p_L^2 = \frac{\alpha'}{2} e^{*i}_I  e^{*j}_I m_i m_j +\frac{1}{2\alpha'} e^{*i}_I (g_{ij}+b_{ij})n^je^{*k}_I (g_{kl}+b_{kl})n^l - e^{*i}_I m_ie^{*k}_I (g_{kl}+b_{kl})n^l\\
= \frac{\alpha'}{2} {\bf m}^T {\bf g}^{-1}{\bf m} + \frac{1}{2\alpha'}{\bf n}^T({\bf g}^T + {\bf b}^T){\bf g}^{-1}({\bf g} + {\bf b}){\bf n} - {\bf m}^T{\bf g}^{-1}({\bf g}+ {\bf b}){\bf n}\\
= \frac{\alpha'}{2} {\bf m}^T {\bf g}^{-1}{\bf m} + \frac{1}{2\alpha'}{\bf n}^T({\bf g}^T + {\bf b}^T){\bf g}^{-1}({\bf g} +{\bf b}){\bf n} - {\bf m}^T{\bf g}^{-1}({\bf g}+{\bf b}){\bf n}
$$
Therefore,
$$
\alpha' M^2 = p_L^2 + p_R^2 +2(N + \bar N -2) = \alpha'{\bf m}^T {\bf g}^{-1}{\bf m} + \frac{1}{\alpha'}{\bf n}^T({\bf g} - {\bf b}{\bf g}^{-1}{\bf b}){\bf n} + 2{\bf n}^T{\bf b}{\bf g}^{-1}{\bf m} + 2(N + \bar N -2)~.
$$
And level matching condition is
$$
N - \bar N = {\boldsymbol \pi} \cdot {\bf W} = {\bf m}^T {\bf n}
$$

### Problem 2.3

Under this map,
$$
p_L^2 + p_R^2 = \alpha'{\bf m}^T {\bf g}^{-1}{\bf m} + \frac{1}{\alpha'}{\bf n}^T({\bf g} - {\bf b}{\bf g}^{-1}{\bf b}){\bf n} + 2{\bf n}^T{\bf b}{\bf g}^{-1}{\bf m}
\\ \to\frac{1}{\alpha'}{\bf n}^T ({\bf g} - {\bf b}{\bf g}^{-1}{\bf b}){\bf n} + \alpha'{\bf m}^T {\bf g}^{-1}{\bf m} - 2{\bf m}^T{\bf g}^{-1}{\bf b}{\bf n} \\
= \frac{1}{\alpha'}{\bf n}^T ({\bf g} - {\bf b}{\bf g}^{-1}{\bf b}){\bf n} + \alpha'{\bf m}^T {\bf g}^{-1}{\bf m} +2{\bf n}^T{\bf b}{\bf g}^{-1}{\bf m}~.
$$
The invariance of level-matching condition is obvious to see. Therefore, the spectrum is invariant.

### Problem 2.4

We have
$$
{\bf g} = \alpha' \frac{\omega_2}{\tau_2} \begin{pmatrix}1 & \tau_1\\
\tau_1 & |\tau|^2\end{pmatrix},\quad {\bf n} = \begin{pmatrix}n_1\\n_2\end{pmatrix}, \quad {\bf m}=\begin{pmatrix}m_1 \\ m_2\end{pmatrix}, \quad {\bf b} = \begin{pmatrix}0 & -B\\ B & 0\end{pmatrix}\quad {\bf g}^{-1} =\frac{1}{\alpha'} \frac{1}{\omega_2 \tau_2} \begin{pmatrix}|\tau|^2 & -\tau_1\\
-\tau_1 & 1\end{pmatrix} ~.
$$
After tedious calculation, we get,
$$
p_L^2 = \frac{1}{2 \alpha'^2 \omega_2 \tau_2}(2\alpha'B(m_1 n_1 \tau_1 -m_2n_1-m_2 n_2 \tau_1+ m_1 n_2 |\tau|^2) + B^2(n_1^2 + 2n_1 n_2 \tau_1 +n_2^2 |\tau|^2)\\
+ \alpha'^2(m_2^2 + n_1^2 \omega_2^2 + 2n_1 \omega_2(n_2 \omega_2 \tau_1 - m_1 \tau_2)-2m_2(m_1 \tau_1 + n_2 \omega_2\tau_2) +(m_1^2 +n_2^2\omega_2^2)|\tau|^2))~,
$$
and
$$
p_R^2 = \frac{1}{2 \alpha'^2 \omega_2 \tau_2}(2\alpha'B(m_1 n_1 \tau_1 -m_2n_1-m_2 n_2 \tau_1+ m_1 n_2 |\tau|^2) + B^2(n_1^2 + 2n_1 n_2 \tau_1 +n_2^2 |\tau|^2)\\
+ \alpha'^2(m_2^2 + n_1^2 \omega_2^2 + 2n_1 \omega_2(n_2 \omega_2 \tau_1 + m_1 \tau_2)-2m_2(m_1 \tau_1 - n_2 \omega_2\tau_2) +(m_1^2 +n_2^2\omega_2^2)|\tau|^2))~,
$$
Now write $B/\alpha' = \omega_1$ and $\omega = \omega_1 + i \omega_2$, we can simplify the results
$$
p_R^2 = \frac{1}{2\omega_2 \tau_2} |m_2 - \tau m_1 + \bar \omega(n_1 + \tau n_2)|^2, \quad\\
p_L^2 = \frac{1}{2\omega_2 \tau_2} |m_2 - \tau m_1+ \omega(n_1 + \tau n_2)|^2~.
$$

- mirror symmetry, $\omega \leftrightarrow \tau$, we have $(m_1, m_2, n_1, n_2) \to (-n_1,m_2, -m_1, n_2)$.
- T-duality, $(m_1, m_2, n_1, n_2) \to (m_1 d-n_2 b, m_2 d +n_1 b, m_2 c +n_1 a, n_2 a-m_1 c)$.
- Torus modular transformation, $(m_1, m_2, n_1, n_2) \to (m_1 a - m_2 c, m_2 d - m_1 b, n_1 d + n_2 b, n_2 a+ n_1 c)$.









