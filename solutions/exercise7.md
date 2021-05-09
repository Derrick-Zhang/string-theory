## Problem 1

### Problem 1.1

$$
\begin{align}
\{\Gamma^{a+}, \Gamma^{b-}\} &= \frac14\{\Gamma^{2a}+i\Gamma^{2a+1}, \Gamma^{2b} - i \Gamma^{2b+1}\}\\
&=\frac 14 \{\Gamma^{2a}, \Gamma^{2b}\} -\frac i4\{\Gamma^{2a}, \Gamma^{2b+1}\}+ \frac i4 \{\Gamma^{2a+1},\Gamma^{2b}\} + \frac 14 \{\Gamma^{2a+1}, \Gamma^{2b+1}\}\\
&= \frac 12 \delta ^{ab} + 0 + 0 + \frac 12 \delta^{ab}= \delta^{ab}~.
\end{align}
$$

$$
\begin{align}
\{\Gamma^{a+}, \Gamma^{b+}\} &= \frac14\{\Gamma^{2a}+i\Gamma^{2a+1}, \Gamma^{2b} + i \Gamma^{2b+1}\}\\
&=\frac 14 \{\Gamma^{2a}, \Gamma^{2b}\} +\frac i4\{\Gamma^{2a}, \Gamma^{2b+1}\}+ \frac i4 \{\Gamma^{2a+1},\Gamma^{2b}\} - \frac 14 \{\Gamma^{2a+1}, \Gamma^{2b+1}\}\\
&= \frac 12 \delta ^{ab} + 0 + 0 - \frac 12 \delta^{ab}= 0~.
\end{align}
$$

$$
\begin{align}
\{\Gamma^{a-}, \Gamma^{b-}\} &= \frac14\{\Gamma^{2a}-i\Gamma^{2a+1}, \Gamma^{2b} - i \Gamma^{2b+1}\}\\
&=\frac 14 \{\Gamma^{2a}, \Gamma^{2b}\} -\frac i4\{\Gamma^{2a}, \Gamma^{2b+1}\}- \frac i4 \{\Gamma^{2a+1},\Gamma^{2b}\} - \frac 14 \{\Gamma^{2a+1}, \Gamma^{2b+1}\}\\
&= \frac 12 \delta ^{ab} + 0 + 0 - \frac 12 \delta^{ab}= 0~.
\end{align}
$$

The dimension of the representation is $$ 2^{k+1}$$. $\zeta$ has label ${\bf s} = \left(-\frac12,-\frac12, \cdots, -\frac 12\right)$.

### Problem 1.2

Let $A = \Gamma^{2a}, B= \Gamma^{2a+1}, C= \Gamma^{2b}, D= \Gamma^{2b+1}$. Since $a \neq b$, these four matrices anticommute with each other.
$$
\left[\Sigma^{2a, 2a+1}, \Sigma^{2b, 2b+1}\right] = -\frac{1}{16}\left[\left[A, B\right],\left[C, D\right]\right]~.\\
= - \frac{1}{16}([AB,CD]-[AB,DC]-[BA,CD]+[BA,DC])
$$
Each commutator vanishes. For example,
$$
[AB,CD] = ABCD-CDAB = ABCD - ABCD=0~,
$$
where we have used the property that $A,B,C,D$ anticommute with each other.

---

When $a \neq 0$,
$$
S_a \equiv \Sigma^{2a , 2a+1} = -\frac i 4 [\Gamma^{2a}, \Gamma^{2a+1}]~.
$$
Since $\Gamma^{a\pm} = \frac12\left(\Gamma^{2a} \pm i \Gamma^{2a+1}\right)$ when $a \neq 0$, we have
$$
\Gamma^{2a} = \Gamma^{a+} + \Gamma^{a-}, \quad \Gamma^{2a+1}= -i (\Gamma^{a+} - \Gamma^{a-})~.
$$
Therefore, 
$$
S_a = -\frac 1 4 [\Gamma^{a+}+ \Gamma^{a-}, \Gamma^{a+}-\Gamma^{a-}]= \frac 12 [\Gamma^{a+}, \Gamma^{a-}] = \Gamma^{a+}\Gamma^{a-}- \frac 12~,
$$
where in the last step, we have used the fact that $\{\Gamma^{a+}, \Gamma^{a-}\} = 1$.

Similarly, when $a = 0$, $\Gamma^{0 \pm} = \frac 12 (\pm \Gamma^0 + \Gamma^1)$, $\Gamma^0 = \Gamma^{0+}- \Gamma^{0-}$, $\Gamma^1 = \Gamma^{0+}+ \Gamma^{0-}$,
$$
S_0 \equiv i \Sigma^{0,1} = \frac 14[\Gamma^0, \Gamma^1] = -\frac 12 [\Gamma^{0-}, \Gamma^{0+}] = \Gamma^{0+}\Gamma^{0-}- \frac 12~.
$$

---

$$
\zeta^{(\bf s)} = \left(\Gamma^{k+}\right)^{s_k + \frac 12} \cdots \left(\Gamma^{a+}\right)^{s_a + \frac 12} \cdots \left(\Gamma^{0+}\right)^{s_0 + \frac 12} \zeta~, \quad s_a = \pm \frac 12~.
$$

Now consider $S_a$ acting on $\zeta^{(\bf s)}$. When $s_a = - \frac 12$,
$$
S_a \zeta^{(\bf s)} = \Gamma^{a+} \Gamma^{a-}\zeta^{(\bf s)} - \frac 12 \zeta^{(\bf s)}~.
$$
Since there are no $\Gamma^{a+}$ in $\zeta^{(\bf s)}$, $\Gamma^{a-}$ in $S_a$ anticommutes with $\Gamma^{b+}$ ($b \neq a$) in $\zeta^{(\bf s)}$, and $\Gamma^{a-}$ annihilates $\zeta$, we have
$$
S_a \zeta^{(\bf s)} = - \frac 12 \zeta^{(s)} = s_a \zeta^{(\bf s)}, \quad s_a = - \frac 12.
$$
When $s_a = \frac 12$, there is one $\Gamma^{a+}$ in $\zeta^{(\bf s)}$, $\Gamma^{a-} \Gamma^{a + } = 1 - \Gamma^{a+}\Gamma^{a-}$,
$$
S_a \zeta^{(\bf s)} = \Gamma^{a+}\Gamma^{a-}\zeta^{(\bf s)} - \frac{1}{2} \zeta^{(\bf s)} = \zeta^{(\bf s)} - \frac 12 \zeta^{(\bf s)} = \frac 12 \zeta^{(\bf s)}~.
$$
Combine these two results together, we obtain, 
$$
S_a \zeta^{(\bf s)} = s_a \zeta^{(\bf s)}~.
$$

### Problem 1.3

Define
$$
\Gamma = i^{-k} \Gamma^0 \Gamma^1 \cdots \Gamma^{D-1}.
$$
Then
$$
\Gamma^2 = (-1)^ k \Gamma^0 \Gamma^1 \cdots \Gamma^{D-1} \Gamma^0 \Gamma^1 \cdots \Gamma^{D-1}
$$
Since $\{\Gamma^\mu, \Gamma^\nu\} = 2 \eta ^{\mu \nu}$, 
$$
\Gamma^2 = (-1)^k (-1)^{D-1}\left(\Gamma^0\right)^2 (-1)^{D-2}\left(\Gamma^1\right)^2 \cdots (-1)^0 \left(\Gamma^{D-1}\right)^2 = (-1)^k (-1)^{\frac{D(D-1)}{2}}(-1) =  (-1)^{2(k+1)^2} = 1~.
$$

---

$$
i^k \{\Gamma, \Gamma^\mu\} = \Gamma^0 \cdots \Gamma^{D-1} \Gamma^\mu + \Gamma^\mu \Gamma^0 \cdots \Gamma^{D-1} = [(-1)^{D-1-\mu}+ (-1)^\mu]\Gamma^0 \cdots (\Gamma^\mu)^2\cdots \Gamma^{D-1}
$$

Since $D$ is even, $(-1)^{D-1-\mu} + (-1)^\mu = 0$, therefore,
$$
\{\Gamma, \Gamma^\mu\} = 0~.
$$

---

$$
4 i [\Gamma, \Sigma^{\mu \nu}] = [\Gamma, [\Gamma^\mu, \Gamma^\nu]] = [\Gamma, \Gamma^\mu \Gamma^\nu - \Gamma^\nu \Gamma^\mu]= \Gamma\Gamma^\mu \Gamma^\nu - \Gamma\Gamma^\nu \Gamma^\mu - \Gamma^\mu \Gamma^\nu \Gamma + \Gamma^\nu \Gamma^\mu \Gamma~.
$$

Now using $\{\Gamma, \Gamma^\mu \} = 0$, it is easy to verfity that the above formula equals 0. Therefore,
$$
[\Gamma, \Sigma^{\mu \nu}] = 0~.
$$

---

When $s_a$ include even number of $-\frac12$s, $\Gamma$-eigen value is $+1$. When $s_a$ include odd number of $-\frac 12$s, $\Gamma$-eigen value is $-1$.

### Problem 1.4

Since the $\Gamma$ matrices satisfy the Clifford algebra,
$$
\{\Gamma^\mu, \Gamma^\nu\} = \Gamma^\mu \Gamma^\nu + \Gamma^\nu \Gamma^\mu = 2 \eta^{\mu \nu}~.
$$
Taking the complex conjugate, we obtain
$$
\{\Gamma^{\mu *}, \Gamma^{\nu *}\} = 2 \eta^{\mu \nu}~.
$$
Moreover, 
$$
\{- \Gamma^{\mu *}, - \Gamma^{\nu *}\} = \{\Gamma^{\mu *}, \Gamma^{\nu *}\} = 2 \eta^{\mu \nu}~.
$$
Therefore, $\pm\Gamma^{\mu *}$ also satisfy the Clifford algebra.

---

When $\Gamma^{a+}$ acts on $\bf s$, when $s_a = - 1/2$, it changes $s_a$ to $1/2$. When $s_a = 1/2$, $\Gamma^{a+} {\bf s} = 0$ since $\left(\Gamma^{a+}\right)^2$.  When $\Gamma^{a-}$ acts on $\bf s$, when $s_a = -1/2$, $\Gamma^{a-} {\bf s} = 0$. When $s_a = 1/2$, acting $\Gamma^{a-}$ changes $s_a$ to $-1/2$. Therefore, the matrix element of $\Gamma^{a \pm}$ should be real.

Then from the definition $\Gamma^{a\pm} = \frac 12(\Gamma^{2a} \pm i \Gamma^{2a+1})$, then $\Gamma^{2a+1} = -i(\Gamma^{a+} - \Gamma^{a-})$ should be imaginary for $a = 1, \cdots ,k$. And $\Gamma^{2a} = \Gamma^{a+} + \Gamma^{a-}$ are real, $\Gamma^0 = \Gamma^{0+}-\Gamma^{0-}$ and $\Gamma^1 = \Gamma^{0+}+ \Gamma^{0-}$ are also real.

---

Define
$$
B_1 = \Gamma^3 \Gamma^5 \cdots \Gamma^{D-1}, \quad B_2 = \Gamma B_1
$$
and their inverse is given by
$$
B_1^{-1} = \Gamma^{D-1} \Gamma^{D-3} \cdots \Gamma^3, \quad B_2^{-1} = - i^k B_1^{-1} \Gamma^{D-1}\Gamma^{D-2} \cdots \Gamma^0~.
$$
Therefore, 
$$
B_1 \Gamma^\mu B_1^{-1} = \Gamma^3 \Gamma^5 \cdots \Gamma^{D-1} \Gamma^\mu \Gamma^{D-1} \Gamma^{D-3} \cdots \Gamma^3
$$
Now using anticommutation rules to move $\Gamma^\mu$ all the way to the right. If $\mu \in \{3, 5, \cdots, D-1\}$, $\Gamma^\mu$ is imaginary. 
$$
\Gamma^{\mu *} = - \Gamma^\mu
$$
When moving $\Gamma^\mu$, among $k$ swappings, $k-1$ of them gives $-1$, one of them (swapping $\Gamma^\mu , \Gamma^\mu$) gives $+1$, so
$$
B_1 \Gamma^\mu B_1^{-1}= (-1)^{k-1} \Gamma^\mu = (-1)^k \Gamma^{\mu *}~.
$$
Similarly, if $\mu \notin \{3, 5, \cdots, D-1\}$, $\Gamma^\mu $ is real, $\Gamma^{\mu *} = \Gamma^\mu$. We obtain,
$$
B_1 \Gamma^\mu B_1^{-1} = (-1)^k \Gamma^\mu = (-1)^k \Gamma^{\mu *}~.
$$

---

Consider
$$
B_2 \Gamma^\mu B_2^{-1} = - \Gamma^0 \Gamma^1 \cdots \Gamma^{D-1} \Gamma^3 \Gamma^5\cdots \Gamma^{D-1} \Gamma^\mu \Gamma^{D-1} \cdots \Gamma^5 \Gamma^3 \Gamma^{D-1} \cdots \Gamma^1 \Gamma^0~.
$$
Now move $\Gamma^\mu $ all the way back to the right. When move through $\Gamma^{D-1} \cdots \Gamma^5 \Gamma^3$, it is the same as above. Now if we pass $\Gamma^\mu$ through the remaining $\Gamma^{D-1} \cdots \Gamma^1 \Gamma^0$, it would give $(-1)^{D-1} =-1$. Therefore,
$$
B_2 \Gamma^\mu B_2^{-1} = (-1)^{k+1} \Gamma^{\mu *}~.
$$

---

Now 
$$
B_1 \Sigma^{\mu \nu}B_1^{-1} = - \frac i 4B_1 [\Gamma^\mu, \Gamma^\nu]B_1^{-1} = - \frac i4(B_1\Gamma^\mu B_1^{-1} B_1 \Gamma^\nu B_1^{-1} - B_1 \Gamma^\nu B_1^{-1} B_1 \Gamma^\mu B_1^{-1}) = - \frac i 4 (\Gamma^{\mu *} \Gamma^{\nu *} - \Gamma^{\nu *}\Gamma^{\mu *}) 
$$
while 
$$
\Sigma^{\mu \nu *} = \frac{i}{4}[\Gamma^{\mu *} , \Gamma^{\nu *}]~.
$$
Therefore $B_1 \Sigma^{\mu \nu} B_1^{-1}= -\Sigma^{\mu \nu *} $. Similarly, $B_2 \Sigma^{\mu \nu} B_2^{-1}= -\Sigma^{\mu \nu *} $.

---

$$
B_1 \Gamma B_1^{-1} = i^{-k}  B_1\Gamma^0 B_1^{-1} B_1\Gamma^1B_1^{-1} \cdots B_1\Gamma^{D-1}B_1^{-1} \\
= (-1)^{kD} i^{-k}( \Gamma^{0} \cdots \Gamma^{D-1})^* = i^{-k}(\Gamma^0 \cdots \Gamma^{D-1})^*
$$

while
$$
\Gamma^* = (-1)^k i^{-k} (\Gamma^0 \cdots \Gamma^{D-1})^*~.
$$
For $B_2$, it is basically the same situation. Therefore, we obtain,
$$
B_1 \Gamma B_1^{-1} = B_2 \Gamma B_2^{-1}= (-1)^k \Gamma^*~.
$$
For $D=10$, $k = 4$, which is the case of the light-cone quantization of superstring, the Weyl representation is its own conjugate.

---

### Problem 1.5

$$
B_1 = \Gamma^3 \Gamma^5 \cdots \Gamma^{D-1} , \quad B_1^* = (-1)^k \Gamma^3 \Gamma^5 \cdots\Gamma^{D-1} = (-1)^k B_1~.
$$

Therefore,
$$
B_1^* B_1 = (-1)^k B_1^2 = (-1)^k (-1)^{k-1} \cdots (-1)^0 = (-1)^{\frac{k(k+1)}{2}}~.
$$
For $B_2$,
$$
B_2^* = \Gamma^* B_1^* = (-1)^k \Gamma B_1~.
$$
Therefore,
$$
B_2^* B_2 = (-1)^k \Gamma B_1 \Gamma B_1 = (\Gamma^0 \cdots \Gamma^{D-1} \Gamma^3 \Gamma^5 \cdots \Gamma^{D-1})^2 ((-1)^{D-1-3}(-1)^{D-1-5} \cdots (-1)^0 \Gamma^0 \Gamma^1 \Gamma^2 \Gamma^4 \cdots \Gamma^{D-2})^2 \\
= (\Gamma^0 \Gamma^1 \Gamma^2 \Gamma^4 \cdots \Gamma^{D-2})^2= (\Gamma^0 \Gamma^1)^2 (\Gamma^2 \Gamma^4 \cdots \Gamma^{D-2})^2 = 1 \cdot (-1)^{k-1}(-1)^{k-2}\cdots (-1)^0 = (-1)^{\frac{k(k-1)}{2}}~.
$$

---

Impose the constraint $B_1^* B_1 = 1$, we find 
$$
k \equiv 0,3 ~{\rm mod}~4~.
$$
Impose the constraint $B_2^* B_2 = 1$, we find
$$
k \equiv 0, 1 ~{\rm mod}~4~.
$$
From Weyl condition, $k$ has to be even. Then $k$ is a multiple of $4$. The spaetime dimension is 
$$
D = 8 n + 2, \quad n \in \mathbb Z_{\ge 0}~.
$$


## Problem 2

### Problem 2.1

At the massless level, in NS sector, we have $\psi_{-1/2}^\mu |0;k\rangle_{\rm NS}$ with 8 degrees of freedom, which form the vector representation $\bf 8_v$. In R sector, there are 16 ground states  $|+1/2, s_1, s_2, s_3, s_4; k\rangle$ with $s_i = \pm 1/2$. These can be decomposed into two family of 8 states, with odd number of $-1/2$, denoted by $|-\rangle_{\rm R}$ and with even number of $-1/2$, denoted by $|+\rangle_{\rm R}$. These form the spinor representation of SO(8), denoted by $\bf 8_s$ and $\bf 8_c$. GSO projection would pick one of them. Taking the same projection for left- and right-moving spectrum leads to Type IIB, while taking the opposite leads to Type IIA. 

The product of two vectors can be decomposed into a scalar, an antisymmetric tensor and a traceless symmetric tensor. For a product of vector representation, denoting a state in ${\bf 8_v} \otimes {\bf 8_s}$ by $|i, {\bf s}\rangle$. We can form the eight linear combinations $|i, {\bf s}\rangle \Gamma^i_{\bf s s'}$ which transform in the $\bf 8_{c}$ representation. The other $56$ states form an irreducible representation $\bf 56_s$.  For the product of spinors, it will have integers and can be decomposed into antisymmetric tensors or forms. We will use $[m]$ to denote antisymmetric tensor with $m$ indices. We will use the subscript $+$ to indicate that the tensor is self-dual.

- Type IIA
  - NS-NS sector, ${\bf 8_v}\otimes {\bf 8_v} = \phi \oplus B_{\mu \nu}\oplus G_{\mu \nu} = {\bf 1} \oplus {\bf 28} \oplus {\bf 35}$. Bosons.
  - NS-R sector, ${\bf 8_v}\otimes {\bf 8_c} = \lambda^+_\alpha \oplus \psi^-_{m, \alpha} = {\bf 8_s} \oplus {\bf 56_c}$. Fermions.
  - R-NS sector, ${\bf 8_s}\otimes {\bf 8_v} = \lambda^-_\alpha \oplus \psi^+_{m, \alpha} = {\bf 8_c} \oplus {\bf 56_s}$. Fermions.
  - R-R sector, ${\bf 8_s}\otimes {\bf 8_c} = C_n \oplus C_{nmp} = [1] \oplus [3] = {\bf 8_v} \oplus {\bf 56_t}$. Bosons.
- Type IIB
  - NS-NS sector, ${\bf 8_v}\otimes {\bf 8_v} = \phi \oplus B_{\mu \nu}\oplus G_{\mu \nu} = {\bf 1} \oplus {\bf 28} \oplus {\bf 35}$. Bosons.
  - NS-R sector, ${\bf 8_v}\otimes {\bf 8_s} = \lambda^-_\alpha \oplus \psi^+_{m, \alpha} = {\bf 8_c} \oplus {\bf 56_s}$. Fermions.
  - R-NS sector, ${\bf 8_s}\otimes {\bf 8_v} = \lambda^-_\alpha \oplus \psi^+_{m, \alpha} = {\bf 8_c} \oplus {\bf 56_s}$. Fermions.
  - R-R sector, ${\bf 8_s}\otimes {\bf 8_s} = C \oplus C_{mn} \oplus C_{mnpq} = [0] \oplus [2] \oplus[4]_+ = {\bf 1} \oplus {\bf 28} \oplus {\bf 35}_+$. Bosons.

### Problem 2.2

At the first massive level, in the NS sector, the states are
$$
\alpha_{-1}^\mu \psi_{-1/2}^\nu |0;k\rangle_{\rm NS}, \quad \psi^\mu_{-1/2}\psi^\nu_{-1/2}\psi^\rho_{-1/2}|0;k\rangle_{\rm NS},\quad \psi^\mu_{-3/2} |0; k\rangle_{\rm NS}~.
$$
The first gives $8\times 8 = 64$ states; the second gives ${8 \choose 3} = 56$ states; and the last one gives $8$ states. Altogether there are 128 bosons.

In the R sector, the states are
$$
\alpha_{-1}^\mu |\pm\rangle_{\rm R} , \quad \psi_{-1}^\mu |\mp \rangle_R.
$$
The ground spinor representation has 8 states, therefore there are $8 \times 8 + 8 \times 8 = 128$ fermions.

---

So there are $128$ bosons in NS sector and $128$ fermions in R sector. So there are $128^2$ bosons in NS-NS sector and R-R sector and $128^2$ fermions in NS-R sector and R-NS sector.

