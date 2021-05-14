## Problem 1

Write $\Lambda$ as
$$
\Lambda = \begin{pmatrix} A & B\\ C & D \end{pmatrix}, \quad 
\Lambda^T = \begin{pmatrix} A^T & C^T\\ B^T & D^T\end{pmatrix}~,
$$
where $A, B, C, D$ are $k\times k$ matrices.

- From $P \Lambda^T P = \Lambda$, we can obtain
  $$
  A = D^T, \quad B = -B^T, \quad C = -C^T~.
  $$
  The degree of freedom is
  $$
  k^2 + \frac{k(k-1)}{2} + \frac{k(k-1)}{2} = 2k^2 -k = \frac12 n(n-1)~.
  $$

- From $P \Lambda^T P = - \Lambda$, we can obtain
  $$
  A = - D^T, \quad B = B^T, \quad C = C^T~.
  $$
  The degree of freedom is
  $$
  k^2 + \frac{k(k+1)}{2} + \frac{k(k+1)}{2} = 2k^2 + k = \frac12 n(n+1)~.
  $$

---

We have
$$
\Omega_\Lambda = P \Lambda^T P \Lambda^{-1} = \begin{cases}+1, & P\Lambda^TP = \Lambda \\
-1, & P \Lambda^T P = - \Lambda\end{cases}~.
$$
 Therefore,
$$
{\rm tr}_\Lambda[\Omega_\Lambda] = \frac 12 n(n-1) - \frac12 n(n+1) = -n~.
$$

## Problem 2

Since $\psi^\mu$ and $\bar \psi^\mu$ are primary fields, they transform as
$$
\psi^\mu(w) = \left(\frac{\partial w}{\partial z}\right)^{-\frac12} \psi^\mu(z), \quad \bar \psi^\mu(w) = \left(\frac{\partial \bar w}{\partial \bar z}\right)^{-\frac 12} \bar \psi^\mu(z)~.
$$
Also, $z = \exp(-iw)$, $\bar z = \exp(i \bar w)$, with $w = it + \sigma$. Therefore,
$$
\psi^\mu (w) = \sqrt{-i} z^{\frac12} \psi^\mu(z) = \sqrt{-i} \sum_{n \in \mathbb Z + \nu} \frac{\psi^\mu_n}{z^n}=i^{-1/2}\sum_{n \in \mathbb Z + \nu} \psi^\mu_n \exp(in(it + \sigma)) = \sum_{n \in \mathbb Z + \nu} b_n^\mu \exp(in (it + \sigma))~,
$$
where $b^\mu_n = i^{-1/2} \psi^\mu_n$. We also have
$$
\bar \psi^\mu(\bar w) = \sqrt{i} \bar z^{\frac 12} \bar \psi^\mu(\bar z) = \sqrt{i} \sum_{n \in \mathbb Z + \bar\nu} \frac{\bar \psi^\mu_n}{\bar z^n} = i^{1/2} \sum_{n \in \mathbb Z + \bar \nu} \bar \psi_n^\mu \exp(in(it-\sigma)) = \sum_{n \in \mathbb Z + \bar \nu} \bar b^\mu_n \exp(in (it - \sigma))~.
$$
Compare the relative sign, we find that the worldsheet parity operator interchanges the left-mover and the right-mover,
$$
\Omega: \psi^\mu(t, \sigma)  \leftrightarrow  \bar \psi^\mu(t, 2\pi - \sigma)~.
$$
In the R sector, we have
$$
\sum_{n \in \mathbb Z} \Omega b_n^\mu \Omega^{-1} \exp(in (it + \sigma)) = \sum_{n \in \mathbb Z} \bar b^\mu_n \exp(in (it + \sigma)) \exp(-2\pi i n)  \quad \Rightarrow \quad  \Omega: b_n^\mu \leftrightarrow \bar b_n^\mu~.
$$
In the NS sector, we have
$$
\sum_{n \in \mathbb Z+ 1/2} \Omega b_n^\mu \Omega^{-1} \exp(in (it + \sigma)) = \sum_{n \in \mathbb Z + 1/2} \bar b^\mu_n \exp(in (it + \sigma)) \exp(-2\pi i n)  \quad \Rightarrow \quad  \Omega: b_n^\mu \leftrightarrow -\bar b_n^\mu~.
$$

---

In type IIB theory, only RR-field that is invariant under $\Omega$ can survive under the projection $(1 + \Omega)/2$. Since $\Omega$ interchange the left-mover and the right-mover, we have to require
$$
\bar \psi^L_+ \Gamma^{\mu_1 \cdots \mu_{p+2}} \psi_+^R = \bar \psi^R_+ \Gamma^{\mu_1 \cdots \mu_{p+2}} \psi_+^L~.
$$
 Also, the spinor bilinear is real, meaning
$$
\bar \psi_+^L \Gamma^{\mu_1 \cdots \mu_{p+2}} \psi_+^R = - \psi^{R\dagger}_+(\Gamma^{\mu_1 \cdots \mu_{p+2}})^\dagger (\Gamma^0)^\dagger \psi^L_+~,
$$
where the minus sign comes from the statistics. Therefore, we need to impose
$$
(\Gamma^{\mu_1 \cdots \mu_{p+2}})^\dagger(\Gamma^0)^\dagger = -\Gamma^0 \Gamma^{\mu_1 \cdots \mu_{p+2}}~.
$$
In the originial type IIB theory, we could have $p = -1, 1,3$ and their magnetic dual. We also have
$$
(\Gamma^\mu)^\dagger = - \Gamma^0 \Gamma^\mu \Gamma^0, \quad (\Gamma^0)^2=-1~.
$$

- $p = -1$,
  $$
  (\Gamma^\mu)^\dagger (\Gamma^0)^\dagger = - \Gamma^0 \Gamma^\mu \Gamma^0\Gamma^0 = \Gamma^0 \Gamma^\mu \neq - \Gamma^0 \Gamma^\mu~.
  $$
  Thus, it vanishes under projection.

- $p=1$,
  $$
  (\Gamma^{[\mu_1} \Gamma^{\mu_2} \Gamma^{\mu_3]})^\dagger (\Gamma^0)^\dagger = \Gamma^{[\mu_3 \dagger} \Gamma^{\mu_2 \dagger} \Gamma^{\mu_1 \dagger]} (\Gamma^0)^\dagger = - \Gamma^0\Gamma^{[\mu_3\dagger}\Gamma^0(-1)\Gamma^0 \Gamma^{\mu_2\dagger} \Gamma^0(-1) \Gamma^0 \Gamma^{\mu_1 \dagger]}\Gamma^0 \Gamma^0\\
  = \Gamma^0 \Gamma^{[\mu_3} \Gamma^{\mu_2} \Gamma^{\mu_1 ]} = - \Gamma^0 \Gamma^{[\mu_1} \Gamma^{\mu_2} \Gamma^{\mu_3 ]}~.~~~~~~~~~~~~~~~~~~
  $$
  Therefore, it survives under the projection.

- $p = 3$, similarly, we can obtain
  $$
  (\Gamma^{[\mu_1} \Gamma^{\mu_2} \Gamma^{\mu_3} \Gamma^{\mu_4}\Gamma^{\mu_5]})^\dagger (\Gamma^0)^\dagger = \Gamma^0 \Gamma^{[\mu_5} \Gamma^{\mu_4} \Gamma^{\mu_3} \Gamma^{\mu_2} \Gamma^{\mu_1]} = \Gamma^0 \Gamma^{[\mu_1} \Gamma^{\mu_2} \Gamma^{\mu_3} \Gamma^{\mu_4} \Gamma^{\mu_5]}~.
  $$
  Therefore, it vanishes under projection.

In conclusion, only 3-form filed strength and its dual 7-form field strength survive. The RR-field potential  $C$ is related to RR-field strength as $G_{(m+1)} = d C_{(m)} $. Therefore, only the 2-form RR-field potentail survives under the projection.

## Problem 3

For closed bosonic string, the orientifold action is
$$
\Omega_p : \begin{cases} X^i(t, \sigma) \leftrightarrow X^i(t, -\sigma) & \quad i = 0,1,\cdots,p\\
X^a (t, \sigma) \leftrightarrow - X^a (t, - \sigma) & \quad a = p+1, \cdots, D-1
\end{cases}~.
$$
Now expand the field in terms of the modes
$$
X^\mu (\tau, \sigma) = x^\mu + \alpha' p^\mu \tau + i \sqrt{\frac{\alpha'}{2}} \sum_{n \neq 0} \frac 1 n \left(\bar \alpha_n^\mu e^{-in \sigma^+} + \alpha^\mu_n e^{-in \sigma^-}\right)~.
$$
In terms of the Euclidean time, it is
$$
X^\mu (t, \sigma)  = x^\mu - i \alpha' p^\mu t + i \sqrt{\frac{\alpha'}{2}} \sum_{n\neq 0} \frac 1n \left[\alpha^\mu_n \exp(in(it + \sigma)) + \bar \alpha_n^\mu \exp(in (it - \sigma))\right]~.
$$
We have
$$
\Omega_p: x^i \leftrightarrow x^i, p^i \leftrightarrow p^i, \alpha_n^i \leftrightarrow\bar \alpha_n^i, \quad i = 0,1,\cdots, p~,
$$
and
$$
\Omega_p : x^a \leftrightarrow - x^a, p^a \leftrightarrow -p^a, \alpha^a_n \leftrightarrow -\bar\alpha_n^a, \quad a = p+1, \cdots ,D-1~.
$$

---

Consider at fixed time in $(X_{24}, X_{25})$-plane, a closed oriented string and its mirror is illustrated as below,

![closed string with O23-plane](/Users/zhanghao/Documents/string-theory/solutions/exercise9.assets/string.jpeg)

The closed string is oriented. As long as the closed string is away from the orientifold plane, it is oriented. The orientifold plane acts like a mirror.

---

Massless states are given by
$$
|\Phi\rangle  = \int \prod_{i,a} dp^i dp^a \Phi^\pm _{IJ} (\tau, p^i, p^a) \left(\alpha^I_{-1} \bar \alpha^J_{-1} \pm \alpha^J_{-1} \bar \alpha^I_{-1}\right) |p^i, p^a\rangle~,
$$
For $\Omega_p$ invariant states, we need to impose $\Omega_p |\Phi\rangle = |\Phi\rangle$. We have
$$
\Omega_p |\Phi\rangle = \int \prod_{i,a } dp^i (-dp^a) \Phi^\pm_{IJ}(\tau, p^i, p^a)  \Omega_p(\alpha^I_{-1} \bar\alpha^J_{-1} \pm \alpha^J_{-1} \bar \alpha^I_{-1})\Omega_p^{-1} \Omega_p|p^i, p^a\rangle\\
=\int \prod_{i,a} dp^i d(-p^a) \Phi^\pm_{IJ}(\tau, p^i, p^a) \Omega_p(\alpha^I_{-1}\bar \alpha^J_{-1} \pm \alpha^J_{-1} \bar \alpha^I_{-1})\Omega_p^{-1} |p^i, -p^a\rangle\\
=\int \prod_{i,a} dp^i dp^a \Phi^\pm_{IJ} (\tau, p^i, -p^a) \Omega_p(\alpha^I_{-1} \bar \alpha_{-1}^J \pm \alpha_{-1}^J \bar \alpha^I_{-1})\Omega_p^{-1} |p^i, p^a\rangle
$$
Therefore, we should have
$$
\Phi^\pm_{IJ} (\tau, p^i, p^a) (\alpha^I_{-1} \bar \alpha^J_{-1} \pm \alpha^J_{-1} \bar \alpha^I_{-1}) = \Phi^\pm_{IJ}(\tau, p^i, -p^a) \Omega_p(\alpha^I_{-1} \bar \alpha^J_{-1} \pm \alpha^J_{-1} \bar \alpha^I_{-1})\Omega_p^{-1}~.
$$
Using $\Omega_p \alpha^i_n \Omega_p^{-1} = \bar \alpha^i_n$, $\Omega_p \alpha_n^a \Omega_p^{-1} = - \bar \alpha^a_n$, we obtain
$$
\Phi^\pm_{ab} (\tau, p^i, p^a) = \pm \Phi^\pm_{ab}(\tau, p^i, - p^a) ,\quad \Phi^\pm_{ia} (\tau, p^i, p^a) = \mp \Phi^\pm_{ia}(\tau, p^i, - p^a), \quad \Phi^\pm_{ij} (\tau, p^i, p^a) = \pm \Phi^\pm_{ij}(\tau, p^i, - p^a)~.
$$

## Problem 4

We have
$$
L_0 = \frac 12 \sum_n :\alpha_{-n} \alpha_n: = \sum_{n \ge 1} \alpha_{-n}\alpha_n + \frac12\alpha_0^2 = \sum_{n \ge 1} \alpha_{-n}\alpha_n + \frac{\alpha'}{4}\left(\frac n R + \frac{w R}{\alpha'}\right)^2~,
$$
and
$$
\bar L_0 = \frac 12 \sum_n :\bar \alpha_{-n} \bar \alpha_n: = \sum_{n \ge 1} \bar\alpha_{-n}\bar\alpha_n + \frac12\bar\alpha_0^2 = \sum_{n \ge 1} \bar\alpha_{-n}\bar\alpha_n + \frac{\alpha'}{4}\left(\frac n R - \frac{w R}{\alpha'}\right)^2~.
$$
Therefore, the $S^1$ partition function is 
$$
Z_{\rm circ} = {\rm Tr}(q^{L_0 - \frac{1}{24}} \bar q^{\bar L_0 - \frac{1}{24}}) = Z_{\rm bos }\cdot \sum_{n,w} q^{\frac{\alpha'}{4}\left(\frac n R + \frac{w R}{\alpha'}\right)^2} \bar q^{\frac{\alpha'}{4} \left(\frac n R - \frac{w R}{\alpha'}\right)^2}\\
=\frac{1}{|\eta(\tau)|^2} \sum_{n,w} q^{\frac{\alpha'}{4}\left(\frac n R + \frac{w R}{\alpha'}\right)^2} \bar q^{\frac{\alpha'}{4} \left(\frac n R - \frac{w R}{\alpha'}\right)^2}~.~~~~~~~~~~~~~~~~~~~~~
$$

---

$$
X(z, \bar z) = x + \bar x -i \sqrt{\frac{\alpha'}{2}} \alpha_0 \log z-i \sqrt{\frac{\alpha'}{2}} \bar \alpha_0\log \bar z + i \sqrt{\frac{\alpha'}{2}} \sum_{n\neq 0} \frac 1n\left(\frac{\alpha_n}{z^n} + \frac{\bar \alpha_n}{\bar z ^n}\right)
$$

Since $R$ is defined as $R X(z, \bar z) R^{-1} = - X(z,\bar z)$, $R^{-1} = R$, we obtain
$$
R \alpha_n R^{-1} = - \alpha_n, \quad R\bar \alpha_n R^{-1} = - \bar \alpha_n, \quad n \in \mathbb Z~.
$$
and
$$
R x R^{-1} = - x, \quad R\bar x R^{-1} = -\bar x~. 
$$
We have
$$
\alpha_0 |n,w\rangle = \sqrt{\frac{\alpha'}{2}} \left(\frac n R + \frac{w R}{\alpha'}\right) |n,w\rangle, \quad \bar \alpha_0 =\sqrt{\frac{\alpha'}{2}}\left(\frac n R - \frac{w R}{\alpha'}\right) |n,w\rangle~.
$$
Then,
$$
\alpha_0(R |n,w\rangle) = R R\alpha_0R|n,w\rangle = R(-\alpha_0)|n,w\rangle = -\sqrt{\frac{\alpha'}{2}} \left(\frac{n}{R}+ \frac{w R}{\alpha'}\right) R|n,w\rangle~.
$$
And similarly for $\bar \alpha_0$, 
$$
\bar\alpha_0(R |n,w\rangle) = R R\bar\alpha_0R|n,w\rangle = R(-\bar\alpha_0)|n,w\rangle = -\sqrt{\frac{\alpha'}{2}} \left(\frac{n}{R}- \frac{w R}{\alpha'}\right) R|n,w\rangle~.
$$
Therefore,
$$
R|n,w\rangle = |-n, -w\rangle~.
$$

---

Under the projection, the momentum and winding quantum numbers change signs. Only states with $|n = 0, w= 0\rangle$ will survive the projection. Then the trace should be similar to the bosonic partition function. We write the Fock space as,
$$
|\Phi\rangle \equiv|n_1, \bar n_1; \cdots; n_k, \bar n_k;\cdots\rangle = (\alpha_{-1})^{n_1} (\bar\alpha_{-1})^{\bar n_1}\dots (\alpha_{-k})^{n_k} (\bar \alpha_{-k})^{\bar n_k}\cdots |0\rangle~.
$$
Then,
$$
\sum_{k=1}^{\infty} \alpha_{-k} \alpha_{k} |\Phi\rangle  = \sum_{k=1}^\infty kn_k |\Phi\rangle~, \quad \sum_{k=1}^{\infty}\bar \alpha_{-k} \bar \alpha_{k} |\Phi\rangle = \sum_{k=1}^\infty k\bar n_k |\Phi\rangle~,
$$
and because $R \alpha_nR = - \alpha_n$, $R \bar \alpha_n R = - \bar \alpha_n$, we have
$$
R|\Phi \rangle = (-1)^{n_1 +\bar n_1 \cdots + n_k+\bar n_k +\cdots} |\Phi\rangle~.
$$
Therefore,
$$
\frac12{\rm Tr}\left(R q^{L_0 - \frac{1}{24}} \bar q^{\bar L_0 - \frac{1}{24}}\right) = \frac12 (q \bar q)^{-\frac{1}{24}} \sum_{n_1=0}^\infty \sum_{\bar n_1=0}^\infty\cdots \sum_{n_k=0}^\infty \sum_{\bar n_k=0}^\infty\cdots \langle \Phi|R q^{L_0}\bar q^{\bar L_0} |\Phi\rangle.\\
= \frac12 (q \bar q)^{-\frac{1}{24}}\sum_{n_1=0}^\infty(-1)^{n_1} q^{n_1} \sum_{\bar n_1 = 0}^\infty (-1)^{\bar n_1} \bar q^{\bar n_1} \cdots \sum_{n_k = 0}^\infty (-1)^{n_k} q^{kn_k} \sum_{\bar n_k = 0}^\infty (-1)^{\bar n_k} \bar q^{k\bar n_k}\cdots\\
= \frac 12 (q\bar q)^{-\frac{1}{24}} \frac{1}{1+q}\frac{1}{1+\bar q}\cdots \frac{1}{1+q^k}\frac{1}{1+ \bar q^k} \cdots = \frac12 (q\bar q)^{-\frac{1}{24}} \prod_{n=1}^\infty\frac{1}{1+q^n} \frac{1}{1+\bar q^n}~,
$$
which can be written as
$$
\left|\frac{\eta(\tau)}{\vartheta_2(\tau)}\right|,
$$
where
$$
\eta(\tau) = q^{\frac{1}{24}} \prod_{n=1}^\infty(1-q^n), \quad \vartheta_2(\tau) = 2 q^{\frac18}\prod_{n=1}^\infty (1-q^n)(1+q^n)^2~.
$$
We can easily see that
$$
\frac{\eta(\tau)}{\vartheta_2(\tau)} = \frac 12 q^{-\frac{1}{12}} \prod_{n=1}^\infty\frac{1}{(1+q^n)^2}~,
$$
and
$$
\left|\frac{\eta(\tau)}{\vartheta_2(\tau)}\right| = \frac12 (q\bar q)^{-\frac{1}{24}} \prod_{n=1}^\infty \frac{1}{1+q^n} \frac{1}{1+\bar q^n}~.
$$
It is invariant under T transformation. However, under S transformation,
$$
S: \left|\frac{\eta(\tau)}{\vartheta_2(\tau)}\right| \to \left|\frac{\eta(\tau)}{\vartheta_4(\tau)}\right|~.
$$
Therefore, it is not modular invariant.

---

In the twisted sector, $X$ satisfies antiperiodic boundary condition, 
$$
X(e^{2\pi i }z) = RX(z)R = - X(z)~.
$$
It forbids any center-of-mass coordinate or momentum. Thus the mode expansion is in terms of half-integer modes,
$$
X(z) = i \sqrt{\frac{\alpha'}{2}} \sum_{n \in \mathbb Z + \frac12} \frac{1}{n} \frac{\alpha_n}{z^n}~.
$$

---

$L_0$ is given by
$$
L_0 = \frac 12 \sum_{n \in \mathbb Z + \frac 12} :\alpha_{-n} \alpha_n: + \frac{1}{16}~.
$$
Similar to the bosonic case, just add an additional $(q\bar q)^{1/16}$ and change the variable $n$ from integers to half-integers, also notice that there are two twisted sectors which cancels the $\frac12$ factor, we have
$$
\frac12{\rm Tr}\left(q^{L_0-\frac{1}{24}}\bar q^{\bar L_0 - \frac{1}{24}}\right) = 
(q\bar q)^{\frac{1}{16} - \frac{1}{24}} \prod_{n =0}^\infty \frac{1}{1-q^{n+\frac12}}\frac{1}{1-\bar q^{n+\frac12}}=\left|\frac{\eta(\tau)}{\vartheta_4(\tau)}\right|~.
$$
And similar to what we have discussed above, we have
$$
\frac 12{\rm Tr} \left( R q^{L_0-\frac{1}{24}} \bar q^{\bar L_0 - \frac{1}{24}}\right) =(q\bar q)^{\frac{1}{16} - \frac{1}{24}} \prod_{n=0}^\infty \frac{1}{1+q^{n+\frac 12}} \frac{1}{1+ \bar q^{n + \frac 12}} = \left|\frac{\eta(\tau)}{\vartheta_3(\tau)}\right|
$$
Therefore,
$$
Z_{\rm tw} = \left|\frac{\eta(\tau)}{\vartheta_4(\tau)}\right| + \left|\frac{\eta(\tau)}{\vartheta_3(\tau)}\right|~.
$$

---

Then the sum is
$$
Z_{\rm orb} + Z_{\rm tw} = \frac12 Z_{\rm circ} + \left|\frac{\eta(\tau)}{\vartheta_2(\tau)}\right|  + \left|\frac{\eta(\tau)}{\vartheta_3(\tau)}\right| + \left|\frac{\eta(\tau)}{\vartheta_4(\tau)}\right|~.
$$
It is easy to see that its modular invariant. First, under T transformation, $|\eta|$ and $|\vartheta_2|$ are invariant, $|\vartheta_3|$ and $|\vartheta_4|$ interchange. Under S transformation, we have
$$
S : \left|\frac{\eta(\tau)}{\vartheta_2(\tau)}\right| \leftrightarrow \left|\frac{\eta(\tau)}{\vartheta_4(\tau)}\right|
$$
and $\left|\frac{\eta(\tau)}{\vartheta_3(\tau)}\right|$ is S transformation invariant. Therefore, the overall partition function is modular invariant.

