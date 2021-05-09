## Problem 1

I used different notation in the partition function.

### Problem 1.1

The torus partition function of the bosonic string on a circle $S^1$ of radius $R$ is given by
$$
Z^{25} = |\eta(\tau)|^{-2} \sum_{n,w} q^{\frac{\alpha'}{4} p_L^2} \bar{q}^{\frac{\alpha'}{4} p^2_R}~,
$$
with
$$
p_R = \frac n R - \frac{R w}{\alpha'}~, \quad p_L = \frac n R + \frac{R w}{\alpha'}~.
$$
The non-compact direction gives
$$
Z^{1, 24} = {\rm const} \times|\eta(\tau)|^{-46}~.
$$
Therefore, 
$$
Z^{1,24} Z^{25} = {\rm const} \times |\eta(\tau)|^{-48} \sum_{n,w} q^{\frac{\alpha'}{4} p_L^2} \bar{q}^{\frac{\alpha'}{4} p^2_R}~.
$$
Expand the Dedekind $\eta$-function,
$$
|\eta(\tau)|^{-48} = (q \bar q)^{-1} + 24 q^{-1}+ 24 \bar q^{-1}+ 24^2 + ...
$$
These terms correspond to $N=\bar N = 0$; $N = 0, \bar N = 1$; $N = 1, \bar N = 0$; $N = \bar N = 1$. Also, 
$$
\sum_{n,w}q^{\frac{\alpha'}{4} p_L^2} \bar{q}^{\frac{\alpha'}{4} p^2_R} = 1+2(q\bar q)^{\frac{\alpha'}{4} \frac{R^2}{\alpha'^2}}+2(q\bar q)^{\frac{\alpha'}{4}\frac{1}{R^2}}\\
+ 2 q^{\frac{\alpha'}{4}\left(\frac{1}{R^2}+\frac{R^2}{\alpha'^2} \right)-\frac12}
\bar q^{\frac{\alpha'}{4}\left(\frac{1}{R^2}+\frac{R^2}{\alpha'^2} \right) + \frac12}
+ 2 q^{\frac{\alpha'}{4}\left(\frac{1}{R^2}+\frac{R^2}{\alpha'^2} \right) + \frac 12}
\bar q^{\frac{\alpha'}{4}\left(\frac{1}{R^2}+\frac{R^2}{\alpha'^2} \right) - \frac 12}
+\cdots~,
$$
These terms corresponds to $n=0, w=0$; $n = 0, w = \pm 1$; $n=\pm 1, w = 0$; $n=-w=\pm1$; $n = w=\pm1$. Now consider the product of these two contributions. We can drop the terms whose $q$ exponent is not the same as the $\bar q$ exponent, for they give zero after performing integration over $\tau_1$. The remaining terms are
$$
(q\bar q)^{-1} + 2(q \bar q)^{\frac{\alpha'}{4}\frac{R^2}{\alpha'^2}-1} + 2(q\bar q)^{\frac{\alpha'}{4}\frac{1}{R^2}-1}+ 48 (q \bar q)^{\frac{\alpha'}{4}\left(\frac{1}{R^2}+ \frac{R^2}{\alpha'^2}\right)-\frac 12} + 48 (q \bar q)^{\frac{\alpha'}{4}\left(\frac{1}{R^2} + \frac{R^2}{\alpha'^2}\right)-\frac12} +24^2+\cdots
$$
These terms correspond to the mass spectrum
$$
M^2 = \frac{n^2}{R^2} + \frac{w^2 R^2}{\alpha'^2} + \frac{2}{\alpha'} (N + \bar N -2)
$$
with 

| $n$     | $w$     | $N$  | $\bar N$ |
| ------- | ------- | ---- | -------- |
| 0       | 0       | 0    | 0        |
| 0       | $\pm 1$ | 0    | 0        |
| $\pm 1$ | 0       | 0    | 0        |
| $\pm1$  | $\mp 1$ | 1    | 0        |
| $\pm1$  | $\pm 1$ | 0    | 1        |
| 0       | 0       | 1    | 1        |

which satisfy the level matching condition,
$$
nw + N - \bar N = 0~.
$$

### Problem 1.2

We want to show that
$$
Z^{25} = |\eta(\tau)|^{-2} \sum_{n,w} q^{\frac{\alpha'}{4} p_L^2} \bar{q}^{\frac{\alpha'}{4} p^2_R} = |\eta(\tau)|^{-2}\sum_{n,w} \exp\left[-\pi \tau_2 \alpha'\left(\frac{n^2}{R^2} + \frac{w^2 R^2}{\alpha'^2}\right) + 2\pi i \tau_1 n w\right]
$$
is modular invariant.

For summation over $n$, use the Poisson resummation formula,
$$
\begin{align}
Z^{25} & = |\eta(\tau)|^{-2} \sum_w \exp\left(-\pi \tau_2 \frac{w^2 R^2}{\alpha'}\right) 
\frac{R}{\sqrt{\alpha' \tau_2}} \sum_m \exp\left(- \frac{\pi R^2 (m - \tau_1 w)^2}{\tau_2 \alpha'}\right)\\
&=\frac{R}{\sqrt{\alpha'}} \frac{1}{\sqrt{\tau_2} |\eta(\tau)|^2} \sum_{m,w} \exp\left(- \pi R^2 \frac{|m-w\tau|^2}{\tau_2 \alpha'}\right)~.
\end{align}
$$
Using modular property of Dedekind $\eta$-function,
$$
\eta(\tau + 1) = e^{i \pi /12} \eta(\tau), \quad \eta(-1/\tau) = \sqrt{-i \tau} \eta(\tau)~,
$$
we have
$$
|\eta(\tau+1)|^2 = |\eta(\tau)|^2, \quad |\eta(-1/\tau)|^2 = |\tau|\, |\eta(\tau)|^2.
$$
Also $\tau_2$ is invariant under T-transformation. Under S-transformation, we have
$$
\tau_2  \to \frac{\tau_2}{|\tau|^2}~.
$$
Therefore, the prefactor in front of the summation is modular invariant. The summation is invariant under T-transformation $\tau \to \tau + 1$, by making a change of variables $m \to m + w$. It is also invariant under S-transformation $\tau \to -1/\tau$, by making a change of variables $m \to w, w \to -m$.

### Problem 1.3

At self-dual radius $R = \sqrt{\alpha'}$, the partition function is given by
$$
Z^{25} = |\eta(\tau)|^{-2} \sum_{n,w} q^{\frac{1}{4} (n-w)^2} \bar{q}^{\frac{1}{4} (n+w)^2}~.
$$
Now consider the summation over $n$ and $w$. When both $n$ and $w$ are even $n = 2s, w = 2t$, or odd $n = 2s +1 , w = 2t +1$, we have
$$
\sum_{s,t} q^{(s-t)^2} \bar q^{(s+t)^2} + \sum_{s,t} q^{(s-t)^2}\bar q^{(s+t+1)^2}~.
$$
Now shift the summation variables, $s \to s+t$, we obtain
$$
\sum_{s,t} q^{s^2} \bar q^{(s+2t)^2} + \sum_{s,t} q^{s^2}\bar q^{(s+2t+1)^2} = \sum_{s,k} q^{s^2} \bar q^{(s+k)^2} = \sum_s q^{s^2} \sum_k \bar q^{k^2}~.
$$
Now consider $n = 2s +1, w = 2t$ and $n = 2s, w = 2t +1$, we have
$$
\sum_{s,t} q^{\left(s-t+ \frac12\right)^2}\bar q^{\left(s+t+\frac12\right)^2}+\sum_{s,t} q^{\left(s-t- \frac12\right)^2}\bar q^{\left(s+t+\frac12\right)^2}~.
$$
Now shift the summation variables, $s \to s-t$, we obtain
$$
\sum_{s,t} q^{\left(s-2t+ \frac12\right)^2}\bar q^{\left(s+\frac12\right)^2}+\sum_{s,t} q^{\left(s-2t-1+ \frac12\right)^2}\bar q^{\left(s+\frac12\right)^2} = \sum_k q^{\left(k+\frac12\right)^2} \sum_s \bar q^{\left(s+\frac12\right)^2}~.
$$
Therefore,
$$
Z^{25} = |\chi_1 (q)|^2 + |\chi_2 (q)|^2, \quad \chi_1 = \frac 1 \eta \sum_n q^{n^2}, \quad \chi_2 = \frac 1 \eta \sum_n q^{(n+1/2)^2}~.
$$
Now expand $Z^{25} Z^{1,24}$, we find the constant term is 676 which corresponds to the massless states. Some of them are special cases of those shown in problem 1.1

- $n = w = 0$, $N = \bar N = 1$, gives $24^2= 576$ states
- $n =w = \pm 1$, $N = 0$, $\bar N = 1$, gives $2 \times 24 = 48$ states
- $n = -w = \pm 1$, $N = 1, \bar N = 0$, gives $2 \times 24 = 48$ states
- $n = \pm 2, w = 0 $, $N = \bar N = 0$, gives 2 states
- $n = 0, w = \pm 2$, $N = \bar N = 0$, gives 2 states

Therefore, in total there are 676 massless states.

### Problem 1.4

The currents in the bosonic string theory are
$$
j^\pm (z) =j^1(z) \pm i j^2(z) = e^{\pm 2i X^{25}(z)/\sqrt{\alpha'}}, \quad j^3(z) = i \partial X^{25}(z)/\sqrt{\alpha'}~.
$$
For simplicity, let's write $X$ instead of $X^{25}$. We also write $k_\pm = \pm 2 /\sqrt{\alpha'}$. The OPE is given by
$$
j^\pm(z) j^3(0) = \frac{i}{\sqrt{\alpha'}}e^{ik_\pm X(z)} \partial X(0)\sim \mp \frac{e^{ik_\pm X(0)}}{z} = \mp \frac{j^\pm(0)}{z}.
$$

$$
j^+(z) j^-(0)=e^{ik_+ X(z)} e^{ik_- X(0)} \sim z^{\alpha' k_+ k_-/2} e^{ik_+ X(z)} e^{ik_-X(0)} = \frac{1}{z^2} e^{ik_+ X(z)} e^{ik_- X(0)} \sim \frac{1}{z^2} + \frac1 z i k_+ \partial X(0).
$$

Similarly, $j^-(z)j^+(0) \sim 1/z^2 + i k_- \partial X(0)/z$ and $j^+(z)j^+(0)\sim j^-(z)j^-(0)\sim0$. Therefore,
$$
\begin{align}
j^1(z) j^1(0) &= \frac12(j^+(z)+ j^-(z)) \frac{1}{2} (j^+(0)+j^-(0)) \sim \frac{1}{2z^2}~,\\
j^2(z) j^2(0) &= \frac{1}{2i}(j^+(z)- j^-(z))\frac{1}{2i}(j^+(z)- j^-(z))\sim \frac{1}{2z^2}~,\\j^3(z) j^3(0) &= - \frac{1}{\alpha'} \part X(z) \part X(0) \sim \frac{1}{2z^2}~,\\
j^1(z) j^2(0) &=\frac{1}{2}(j^+(z)+ j^-(z))\frac{1}{2i}(j^+(0)- j^-(0))\sim \frac{i}{z} j^3(0)~.\\
j^2(z) j^3(0) &= \frac{1}{2i} (j^+(z) - j^-(z)) j^3(0) \sim \frac{i}{2z}(j^+(0)+j^-(0))=\frac i z j^1(0)~.\\
j^3(z) j^1(0) &= j^3(z) \frac{1}{2}(j^+(0)+j^-(0))\sim \frac{1}{2z} (j^+(0) - j^-(0)) = \frac i zj^2(0)~.
\end{align}
$$
In conclusion,
$$
j^a (z) j^b (0) \sim \frac{\delta^{ab}}{2z^2} + \frac{i \epsilon^{abc} j^c(0)}{z}~.
$$
Write the currents in terms of oscillator modes
$$
j^a(z) = \sum_m \frac{j^a_m}{z^{m+1}},\quad j^a_m = \int \frac{dz}{2\pi i} z^m j^a(z)~.
$$
Therefore,
$$
\begin{align}
[j^a_m, j^b_n] &= \int_w \frac{dz}{2\pi i} \int \frac{dw}{2\pi i} z^m w^n j^a(z) j^b(w)\\
&= \int \frac{dw}{2\pi i} \int_w \frac{dz}{2\pi i} z^m w^n \left(\frac{\delta^{ab}}{2(z-w)^2} + \frac{i \epsilon^{abc} j^c(w)}{z-w}\right)\\
&=\int \frac{dw}{2\pi i} \left(\frac12 m w^{m+n-1}\delta^{ab} + w^{m+n} i \epsilon^{abc} j^c(w)\right)\\
&= \frac m 2\delta_{m+n,0} \delta^{ab} + i \epsilon^{abc} j^c_{m+n}~.
\end{align}
$$
The zero modes satisfy the SU(2) algebra
$$
[j_0^a, j^b_0] = i \epsilon^{abc} j^c_0~.
$$

## Problem 2

The chirality operator is given by
$$
\Gamma_{11} = \Gamma^0 \Gamma^1 \cdots \Gamma^9~,
$$
chiral spinors are defined by
$$
\Gamma_{11} \psi_\pm = \pm \psi_\pm~.
$$
Take the Hermitian conjugate we obtain
$$
\psi_\pm ^\dagger \Gamma_{11}^\dagger = \psi^\dagger_\pm (\Gamma^9)^\dagger \cdots (\Gamma^0)^\dagger = \psi^\dagger_\pm \Gamma^0 \Gamma^9\Gamma^8 \cdots\Gamma^1 = \pm \psi_\pm^\dagger
$$
So we have
$$
\bar \psi_\pm \Gamma^9 \Gamma^8 \cdots \Gamma^0 = \pm \bar \psi_\pm
$$
and
$$
\Gamma^9 \Gamma^8 \cdots \Gamma^0 = (-1)^{1+2 +\cdots+9} \Gamma^0 \cdots \Gamma^9 = - \Gamma_{11}~.
$$
Therefore,
$$
\bar \psi_\pm \Gamma_{11} = \mp \bar \psi_\pm~.
$$

---

For type IIA, the spinor bilinears are given by
$$
\bar \psi_-^L \Gamma^{\mu_1 \cdots \mu_{p+2}} \psi_+^R = \bar \psi_- ^L \Gamma_{11} \Gamma^{\mu_1 \cdots \mu_{p+2}} \Gamma_{11} \psi_+^R~.
$$
For type IIB, the spinor bilinears are given by
$$
\bar \psi_+^L \Gamma^{\mu_1 \cdots \mu_{p+2}} \psi_+^R = - \bar \psi_+^L \Gamma_{11} \Gamma^{\mu_1 \cdots \mu_{p+2}} \Gamma_{11} \psi_+^R~.
$$
First, it is easy to see that,
$$
\Gamma_{11} \Gamma^i = - \Gamma^i \Gamma_{11},\quad (\Gamma_{11})^2 = 1~.
$$
If $p$ is even, then
$$
\Gamma_{11} \Gamma^{\mu_1 \cdots \mu_{p+2}} \Gamma_{11} = \Gamma^{\mu_1 \cdots \mu_{p+2}}~.
$$
If $p$ is odd, then
$$
\Gamma_{11} \Gamma^{\mu_1 \cdots \mu_{p+2}} \Gamma_{11} = - \Gamma^{\mu_1 \cdots \mu_{p+2}}~.
$$
Therefore, for type IIA, $p$ has to be even and for type IIB, $p$ has to be odd.

---

$$
\{\beta_9, \Gamma^9\} = \{\Gamma^9 \Gamma_{11}, \Gamma^9\} = \Gamma^9 \{\Gamma_{11}, \Gamma_9\} = 0~.
$$

For $\mu \neq 9$,
$$
[\beta_9, \Gamma^\mu] = [\Gamma^9 \Gamma_{11}, \Gamma^\mu] = \Gamma^9 \Gamma_{11} \Gamma^\mu - \Gamma^\mu \Gamma^9 \Gamma_{11} = (-1)^9 \Gamma^9 \Gamma^\mu \Gamma_{11} + \Gamma^9 \Gamma^\mu \Gamma_{11} = 0~.
$$

---

The action of duality transform the IIA and IIB spinor bilinears to
$$
\bar \psi_-^L \Gamma^{\mu_1 \cdots \mu_{p+2}}\Gamma^9 \psi_+^R,\quad
\bar \psi_+^L \Gamma^{\mu_1 \cdots \mu_{p+2}}\Gamma^9 \psi_+^R
$$
When $\Gamma^{\mu_1 \cdots \mu_{p+2}}$ contains $\Gamma^9$, multiply a $\Gamma^9$ would cancel the orignial one. If $\Gamma^{\mu_1 \cdots \mu_{p+2}}$ does not contain $\Gamma^9$, multiply a $\Gamma^9$ would add another matrix. Therefore, T-duality transforms the RR field strengths in IIA to those in IIB, and vice versa.

## Problem 3

### Problem 3.1

If we performing T-duality on one of the directions in NN, it would change this direction to DD, and vice versa. If we performing T-duality on one of the directions in ND, it would change this direction to DN, and vice versa. In short, T-duality switches NN $\leftrightarrow$ DD and ND $\leftrightarrow$ DN. So (#NN + #DD) and (#ND + #DN) are invariant under T-duality.

### Problem 3.2

We can have one D3-brane intersecting one D1-brane and they do not share any common spatial directions. For example,

|      |    0     |    1     |    2     |    3     |  4   |  5   |    6     |  7   |  8   |  9   |
| :--: | :------: | :------: | :------: | :------: | :--: | :--: | :------: | :--: | :--: | :--: |
|  D3  | $\times$ | $\times$ | $\times$ |          |      |      | $\times$ |      |      |      |
|  D1  | $\times$ |          |          | $\times$ |      |      |          |      |      |      |

We can also have one D3-brane intersecting another D3-brane and they share one same spatial directions. For example,

|      |    0     |    1     |    2     |    3     |    4     |  5   |    6     |  7   |  8   |  9   |
| :--: | :------: | :------: | :------: | :------: | :------: | :--: | :------: | :--: | :--: | :--: |
|  D3  | $\times$ | $\times$ | $\times$ |          |          |      | $\times$ |      |      |      |
|  D3  | $\times$ | $\times$ |          | $\times$ | $\times$ |      |          |      |      |      |

We can also have one D3-brane intersecting one D5-brane and they share two same spatial directions. For example,

|      |    0     |    1     |    2     |    3     |    4     |    5     |    6     |  7   |  8   |  9   |
| :--: | :------: | :------: | :------: | :------: | :------: | :------: | :------: | :--: | :--: | :--: |
|  D3  | $\times$ | $\times$ | $\times$ |          |          |          | $\times$ |      |      |      |
|  D5  | $\times$ | $\times$ | $\times$ | $\times$ | $\times$ | $\times$ |          |      |      |      |

We can also have one D3-brane intersecting one D7-brane and they share three same spatial directions. For example,

|      |    0     |    1     |    2     |    3     |    4     |    5     |    6     |    7     |  8   |  9   |
| :--: | :------: | :------: | :------: | :------: | :------: | :------: | :------: | :------: | :--: | :--: |
|  D3  | $\times$ | $\times$ | $\times$ |          |          |          | $\times$ |          |      |      |
|  D7  | $\times$ | $\times$ | $\times$ | $\times$ | $\times$ | $\times$ | $\times$ | $\times$ |      |      |

---

All these configurations are T-dual to the following D1-D5 configuration:

|      |    0     |    1     |    2     |    3     |    4     |    5     |  6   |  7   |  8   |  9   |
| :--: | :------: | :------: | :------: | :------: | :------: | :------: | :--: | :--: | :--: | :--: |
|  D1  | $\times$ | $\times$ |          |          |          |          |      |      |      |      |
|  D5  | $\times$ | $\times$ | $\times$ | $\times$ | $\times$ | $\times$ |      |      |      |      |

In the example given above,

- D3 and D1, take T-dual in the 3, 4 direction
- D3 and D3, take T-dual in the 3, 4 direction
- D3 and D5, take T-dual in the 2, 6 direction
- D3 and D7, take T-daul in the 2, 6 direction

would lead to the above D1-D5 configuration.