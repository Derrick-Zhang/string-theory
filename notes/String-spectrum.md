# The string spectrum

## BRST quantization

The gauge transformation satisfy the algebra
$$
[\delta_a, \delta_b] = f^\gamma_{~\alpha\beta} \delta_\gamma~.
$$
The path integral fields are denoted $\phi_i$. Now fix the gauge by conditions
$$
F^A(\phi) = 0~,
$$
Following the Faddeev-Popov procedure, the path integral becomes
$$
\int \frac{[d\phi_i]}{V_{\rm gauge}} \exp(-S_1) \to \int [d\phi_i d B_A db_A d c^\alpha]\exp(-S_1 - S_2 -S_3)~,
$$
where $S_1$ is the original gauge-invariant action, $S_2$ is the gauge-fixing action
$$
S_2 = -i B_A F^A(\phi)~,
$$
and $S_3$ is the Faddeev-Popov action
$$
S_3 = b_A c^\alpha \delta_\alpha F^A(\phi)~.
$$
We have introduced the field $B_A$ to produce an integral representation of the gauge fixing $\delta(F^A)$.

---

The overall action is invariant under the BRST transformation
$$
\begin{align}
\delta_B \phi_i &= -i \epsilon c^\alpha \delta_\alpha \phi_i,\\
\delta_B B_A &= 0, \\
\delta_B b_A &= \epsilon B_A,\\
\delta_B c^\alpha &= \frac i2 \epsilon f^\alpha_{~\beta \gamma} c^\beta c^\gamma
\end{align}
$$
This transformation mixes commuting and anticommuting objects, so that $\epsilon$ must be taken to be anti commuting. There is a conserved ghost number, which is +1 for $c^\alpha$, $-1$ for $b_A$ and $\epsilon$, and 0 for all other fields.

- The original action $S_1$ is invariant because the action of $\delta_B$ on $\phi_i$ is just a gauge transformation with parameter $i\epsilon c^\alpha$

- $$
  \delta_B S_2 = -i B_A\delta_B F^A(\phi) = -i B_A \frac{\partial F^A(\phi)}{\partial \phi^i} \delta_B \phi_i = - B_A \frac{\partial F^A(\phi)}{\partial \phi^i} \epsilon c^\alpha \delta_\alpha \phi_i = -B_A \epsilon c^\alpha \delta_\alpha F^A(\phi)
  $$

- The contribution from $S_3$ are

  - $$
    (\delta_B b_A) c^\alpha \delta_\alpha F^A(\phi)=\epsilon B_Ac^\alpha \delta_\alpha F^A(\phi)
    $$

  - $$
    b_A (\delta_B c^\alpha) \delta_\alpha F^A(\phi) = \frac i 2 f^\alpha_{~\beta \gamma}b_A \epsilon c^\beta c^\gamma \delta_\alpha F^A(\phi)
    $$

  - $$
    b_A c^\alpha \delta_\alpha \delta_B F^A(\phi) = b_A c^\alpha \delta_\alpha \frac{\partial F^A(\phi)}{\partial \phi_i} \delta_B \phi_i = b_A c^\alpha \delta_\alpha \frac{\partial F^A(\phi)}{\partial \phi_i} (-i)\epsilon c^\beta \delta_\beta \phi_i\\ = -i \epsilon b_A c^\gamma c^\beta \frac{\partial F^A(\phi)}{\partial \phi_i}\delta_\gamma \delta_\beta \phi_i
    = - i \epsilon b_A c^\gamma c^\beta \frac{\partial F^A(\phi)}{\partial \phi_i} \frac12 f^\alpha_{\gamma \beta} \delta_\alpha \phi_i
    $$

Another key point here is that
$$
\delta_B (b_A F^A) = i\epsilon (S_2 + S_3)
$$
Now consider a small change $\delta F$ in the gauge-fixing condition. The change in the gauge-fixing and ghost action gives
$$
\epsilon \delta \langle f | i \rangle = i \langle f|\delta_B(b_A \delta F^A)|i\rangle = -\epsilon\langle f |\{Q_B, b_A \delta F^A\} |i\rangle~
$$
Therefore, physcial states must satisfy
$$
\langle \psi | \{Q_B, b_A \delta F^A\} | \psi'\rangle = 0
$$
Now this equation holds for arbitrary $\delta F^A$, so we have
$$
Q_B |\psi\rangle = Q_B |\psi'\rangle = 0
$$
There is one more key idea. In order to move around in the space of gauge choices, the BRST charge must remain conserved. Thus it must commute with the change in the Hamiltonian
$$
0 = [Q_B, \{Q_B, b_A \delta F^A\}] = [Q_B^2, b_A \delta F^A]~.
$$
In order for this to vanish for general changes of gauge, we need
$$
Q^2_B = 0~.
$$
That is, the BRST charge is nilpotent. The possibility $Q_B^2 =$ constant is excluded because $Q_B^2$ has ghost number 2

---

More generally, in the gauge algebra, the structure constants might be dependent of the fields. There might be additional terms proportional to the equations of motion. In this case, the BRST doesn't give a nilpotent transformation, leading to the BV formalism.

The nilpotency of $Q_B$ hs an important consequence. A state of the form
$$
Q_B |\chi \rangle
$$
will be annihilated by $Q_B$ for any $\chi$ and so is physical. However, it is orthogonal to all physical states including itself
$$
\lang \psi | Q_B |\chi\rangle = 0
$$
if $Q_B | \psi\rangle = 0$. All physical amplitudes involving such a null state thus vanish. Two physical state that differ by a null state,
$$
|\psi'\rangle = |\psi \rangle + Q_B |\chi \rangle
$$
will have the same innter products with all physical states and are therefore physically equivalent. Thus,
$$
\mathscr H_{\rm BRST} = \mathscr H_{\rm closed} / \mathscr H_{\rm exact}~.
$$

## BRST quantization of the string

In string theory, the BRST quantization is
$$
\delta_B X^\mu = i\epsilon(c \partial + \bar c \bar \partial) X^\mu \\
\delta_B b = i\epsilon(T^X + T^g), \quad \delta_B \bar b = i\epsilon(\bar T^X + \bar T^g)\\
\delta_B c = i \epsilon c \partial c, \quad \delta_B \bar c = i \epsilon \bar c \bar \partial \bar c
$$
Noether's theorem gives the BRST current
$$
j_B = cT^m + \frac12 :cT^g: + \frac32 \partial^2 c = c T^m + :bc\partial c: + \frac32 \partial^2 c
$$
The final term in the current is a total derivative and does not contribute to the BRST charge; it has been added by hand to make the BRST current a tensor. It is a total derivative and does not contribute to the BRST charge. The OPEs of the BRST current with the ghost fields and with a general matter tensor field are
$$
j_B b(0) \sim \frac{3}{z^3} + \frac{1}{z^2} j^g(0) + \frac1 z T^{m+g}(0)~,
$$

The BRST operator is
$$
Q_B = \frac{1}{2\pi i} \oint (dz j_B - d\bar z \bar j_B)
$$
By the usual contour argument, the OPE implies
$$
\{Q_B, b_m\} = L_m^m + L_m^g~.
$$
In terms of the ghost modes,

$$
Q_B = \sum_n (c_n L_{-n}^m + \bar c_n \bar L_{-n}^m) + \sum_{m,n} \frac{m-n}{2}:(c_m c_n b_{-m-n}+\bar c_m \bar c_n \bar b_{-m-n}): + a^B (c_0 + \bar c_0)
$$
with $a^B = a^g = 1$. Moreover, 
$$
j_B(z) j_B(0) \sim - \frac{c^m - 18}{2 z^3} c \partial c(0) - \frac{c^m - 18}{4 z^2}c \partial^2 c(0) - \frac{c^m - 26}{12z} c \partial^3 c(0)~.
$$
The single pole implies that $\{Q_B, Q_B\} = 0$ when $c^m = 26$.