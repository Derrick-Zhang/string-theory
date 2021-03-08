## Action principles

What we are studying?

- classical and quantum mechanics of a one-dimensional object, a string

- String moves in $D$ flat spacetime dimensions, with metric
  $$
  \eta = {\rm diag}(-,+,+,\cdots,+)
  $$

---

### Point particle

The spacetime position is parametrized by $\tau$, and we write $X^\mu(\tau)$ . The action is given by
$$
S = -m \int d \tau \sqrt{-\part_\tau X^\mu \part_\tau X_\mu}~.
$$
Its variation is given by
$$
\delta S = m \int d\tau \frac{\part_\tau X_\mu \delta(\part_\tau X^\mu)}{\sqrt{-\part_\tau X^\mu \part_\tau X_\mu}} = -m \int d\tau\part_\tau u_\mu \delta X^\mu~,
$$
where 
$$
u^\mu = \frac{\part_\tau X^\mu}{\sqrt{-\part_\tau X^\mu \part_\tau X_\mu}}
$$
is the normalized $D$-velocity.

---

 It is useful to introduce an auxiliary field on the worldline, the worldline metric $\gamma_{\tau \tau}(\tau)$ . Writing $\eta(\tau) = \sqrt{-\gamma_{\tau\tau}(\tau)}$ , we can define another action
$$
S' = \frac1 2 \int d\tau (\eta^{-1} \part_\tau X^\mu \part_\tau X_\mu - \eta m^2)~.
$$
Its variation with respect to $\eta$ gives
$$
\delta S' = \frac12 \int d \tau (-\eta^{-2}\part_\tau X^\mu \part_\tau X_\mu - m^2)\delta \eta~,
$$
which leads to
$$
\eta^2 = - \frac{1}{m^2} \part_\tau X^\mu \part_\tau X_\mu.
$$
Plug this back into the action $S'$ would reproduce $S$ .

---

### String

A one-dimensional object will sweep out a two-dimensional world-sheet, which can be described in terms of two parameters $X^\mu(\tau, \sigma)$ .

- Nambu-Goto action

  Introduce the induced metric $h_{ab}$ where indices run over $\{\tau, \sigma\}$ :
  $$
  h_{ab} = \part_a X^\mu \part_b X_\mu~.
  $$
  The action is given by
  $$
  S_{\rm NG} = -\frac{1}{2\pi \alpha'}\int d\tau d\sigma \sqrt{-\det h_{ab}}~.
  $$
  The constant $\alpha'$ has units of spacetime-length-squared, is called the Regge slope. The tension of a string is related to Regge slope by
  $$
  T = \frac{1}{2 \pi \alpha'}~.
  $$
  
- Polyakov action

  Introducing an auxiliary field, the world-sheet metric $\gamma_{ab}(\tau, \sigma)$ , the action is
  $$
  S_{\rm P} = -\frac{1}{4\pi \alpha'} \int d \tau d \sigma \sqrt{-\gamma} \gamma^{ab} \part_a X^\mu \part_b X_\mu~,
  $$
  where $\gamma = \det \gamma_{ab}$ .

  Since
  $$
  \gamma = \sum_a\gamma_{a b} \Delta^{a b}~,\quad \gamma^{ab} = \frac{\Delta^{ab}}{\gamma}~,
  $$
  we have
  $$
  \part \gamma/\part \gamma_{ab} = \Delta^{ab} = \gamma \gamma^{ab}~,
  $$
  which leads to
  $$
  \delta \gamma = \gamma \gamma^{ab} \delta \gamma_{ab} = - \gamma \gamma_{ab}\delta \gamma^{ab}~.
  $$
  

  The variation of the action with respect to metric is
  $$
  \delta_\gamma S_{\rm P} = -\frac{1}{4 \pi \alpha'} \int d\tau d\sigma \left(h_{ab}-\frac12\gamma_{ab}\gamma^{cd}h_{cd}\right) \sqrt{-\gamma}\delta \gamma^{ab}~,
  $$
  $\delta_\gamma S_{\rm P} = 0$ implies that
  $$
  h_{ab} = \frac12 \gamma_{ab} \gamma^{cd} h_{cd}~.
  $$
  We can view this as an identity between matrix $h_{ab}$ and $\gamma_{ab}$ . To get rid of the scalar $\frac12 \gamma^{cd} h_{cd}$ , we divide by the square root of the determinant.
  $$
  \frac{h_{ab}}{\sqrt{-h}} = \frac{\gamma_{ab}}{\sqrt{-\gamma}}~.
  $$
  Plug this back into the Polyakov action would give the Nambu-Goto action.

### Symmetries of Polyakov action

- $D$-dimensional Poincaré invariance:
  $$
  \begin{align}
  X' ^ \mu (\tau, \sigma) &= \Lambda^\mu_{~\nu} X^\nu(\tau, \sigma) + a^\mu~,\\
  \gamma'_{ab} (\tau, \sigma) &= \gamma_{ab} (\tau, \sigma)~.
  \end{align}
  $$

- World-sheet diffeomorphism invariance:
  $$
  \begin{align}
  X'^\mu(\tau', \sigma') &= X^\mu(\tau, \sigma)~,\\
  \frac{\part \sigma'^c}{\part \sigma^a} \frac{\part \sigma'^d}{\part \sigma^b} \gamma'_{cd}(\tau', \sigma') &= \gamma_{ab}(\tau, \sigma)~.
  \end{align}
  $$

- Weyl invariance:
  $$
  \begin{align}
  X'^\mu (\tau, \sigma) &= X^\mu(\tau, \sigma)~,\\
  \gamma_{ab}'(\tau, \sigma) &= \exp(2\omega(\tau, \sigma))\gamma_{ab}(\tau,\sigma)~.
  \end{align}
  $$

---

### Equation of motion

The variation of the action with respect to the metric defines the energy-momentum tensor,
$$
T^{ab} (\tau, \sigma) = -(4\pi) \sqrt{-\gamma}\frac{\delta}{\delta \gamma_{ab}}S_{\rm P} = -\frac{1}{\alpha'} (h^{ab} - \frac{1}{2} \gamma^{ab} \gamma_{cd} h^{cd})~.
$$
Varying $\gamma_{ab}$ in the action gives the equation of motion
$$
T_{ab} = 0~.
$$
Varying $X^\mu$ gives the equation of motion
$$
\part^a \part_a X^\mu = 0~.
$$

### Boundary conditions

For world-sheet with boundary there is also a surface term in the variation of the action. To be specific, take the coordinate region to be
$$
-\infty < \tau <\infty, \quad 0 \le \sigma \le \ell~.
$$
Then the boundary term in the variation of action is given by
$$
-\frac{1}{2\pi \alpha'}\int ^\infty_{-\infty} d\tau \sqrt{-\gamma} \delta X^\mu \part^\sigma X_\mu \bigg|^{\sigma = \ell}_{\sigma = 0}~.
$$
The boundary term vanishes if 
$$
\part^\sigma X^\mu (\tau, 0) = \part^\sigma X^\mu(\tau, \ell) = 0~.
$$
These are **Neumann** boundary conditions on $X^\mu$ . Stated more covariantly,
$$
n^a \part_a X_\mu = 0 \quad {\rm on } ~ \part M~,
$$
where $n^a$ is normal to the boundary of $\part M$ . The ends of the open string move freely in spacetime.

The surface term in the equation of motion will also vanish if we impose
$$
X^\mu(\tau, \ell) = X^\mu (\tau, 0)~, \quad \part^\sigma X^\mu(\tau, \ell) = \part^\sigma X^\mu(\tau, 0)~, \quad \gamma_{ab} (\tau,\ell) = \gamma_{ab} (\tau,0)~.
$$
That is, the fields are **periodic** .

### Open string spectrum

We will use $x$ to denote spacetime coordinates and $X$ for world-sheet coordinates. Define light-cone coordinates in spacetime:
$$
x^{\pm} = \frac{1}{\sqrt{2}} (x^0 \pm x^1)~, \qquad x^i, i = 2, \cdots, D-1~.
$$
In these coordinates the metric is
$$
a^\mu b_{\mu}  = -a^+ b_- - a^- b^+  + a^i b^i~,
$$
and 
$$
a_- = - a^+ ~,\quad a_+ = - a^-~, a_i = a^i~.
$$
We will set the world-sheet parameter $\tau$ at each point of the world-sheet to be equal to the spacetime coordinates $x^+$ . So $x^+$ will play the role of time and $p^-$ that of energy. The longitudinal variables $x^-$ and $p^+$ are then like spatial coordinates and momenta, as are the traverse $x^i$ and $p^i$ .

---

### Point particle

First we have $X^+(\tau) = \tau$ . The action then becomes
$$
S' = \frac12 \int d \tau (-2 \eta^{-1} \part_\tau X^- + \eta^{-1}\part_\tau X^i \part_\tau X^i - \eta m^2)~.
$$
The canonical momenta $p_\mu = \part L / \part (\part_\tau X^\mu)$ are
$$
p_- = - \eta^{-1}~,\quad p_i = \eta^{-1} \part_\tau X^i~.
$$
The Hamiltonian is
$$
H = p_- \part_\tau X^- + p_i \part_\tau X^i - L= \frac{p^i p^i + m^2}{2 p^+}~.
$$
Note that neither $X^+$ nor $\eta$ is dynamic fields. To quantize, impose canonical commutators,
$$
[p_i, X^j] = - i \delta _i ^{~j}~, \quad [p_-, X^-] = -i~.
$$
Momentum eigenstates $|k_-, k^i\rang$ form a complete set.

### Open string

Since there are three local symmetries (the choice of two world-sheet coordinates plus the Weyl scaling), we choose light-cone gauge and impose two conditions on the metric

- $X^+ = \tau$ ,
- $\part_\sigma \gamma_{\sigma \sigma} = 0$ ,
- $\det \gamma_{ab} = -1$ .

The independent components in $\gamma_{ab}$ are $\gamma_{\sigma \sigma} = a(\sigma)$ and $\gamma_{\tau \sigma} = b(\tau, \sigma)$ . The inverse metric is
$$
\begin{bmatrix}
\gamma^{\tau \tau} & \gamma^{\tau \sigma} \\
\gamma^{\sigma \tau} & \gamma^{\sigma \sigma}
\end{bmatrix}
=
\begin{bmatrix}
-a & b\\
b & a^{-1}(1-b^2)
\end{bmatrix}~.
$$
Now let us solve for $a$  and $b$.

---

The Lagrangian then becomes
$$
L = - \frac{1}{4\pi \alpha'} \int_{0}^{\ell} d \sigma [a(2 \part_\tau X^- - \part_\tau X^i \part_\tau X^i)- 2b(\part_\sigma X^- - \part_\tau X^i \part_\sigma X^i) + a^{-1}(1-b^2)\part_\sigma X^i \part_\sigma X^i]
$$
If we separate $X^-(\tau, \sigma)$ into two pieces $x^-(\tau)$ and $Y^-(\tau, \sigma)$ :
$$
\begin{align}
x^-(\tau) = \frac{1}{\ell} \int _0^\ell d \sigma X^-(\tau, \sigma)~,\\
Y^-(\tau, \sigma) = X^-(\tau, \sigma) - x^-(\tau) ~.
\end{align}
$$
Note that $x^-(\tau)$ is the mean of $X^-(\tau, \sigma)$ while $Y^-(\tau, \sigma)$ has zero mean.

Therefore, the Lagrangian is written as
$$
L = - \frac{1}{4\pi \alpha'} \int_{0}^{\ell} d \sigma [a(2 \part_\tau x^- - \part_\tau X^i \part_\tau X^i)- 2b(\part_\sigma Y^- - \part_\tau X^i \part_\sigma X^i) + a^{-1}(1-b^2)\part_\sigma X^i \part_\sigma X^i]
$$
The field $Y^-$ acts as a Lagrange multiplier, giving  a constraint,
$$
\part^2_\sigma b = 0~.
$$
In this gauge, the Neumann boundary condition looks like
$$
\part^\sigma X^\mu = \gamma^{\sigma \tau}\part_\tau X^\mu + \gamma^{\sigma \sigma}\part_\sigma X^\mu = 0 \quad {\rm at}~\sigma = 0, \ell~.
$$

- For $\mu = +$ , $X^+ = \tau$ , we have

$$
\gamma^{\sigma \tau } = \gamma_{\sigma \tau} = b(\tau, \sigma) = 0\quad {\rm at}~\sigma = 0, \ell~.
$$

​	Since $\part_\sigma^2 b = 0$, $\gamma_{\sigma \tau }$ vanishes everywhere.

- For $\mu = i$, the boundary condition is 
  $$
  \part_\sigma X^i = 0\quad {\rm at}~ \sigma = 0, \ell~.
  $$

---

Now the system reduce to
$$
L = -\frac{\ell}{2\pi \alpha'} \gamma_{\sigma\sigma} \part_\tau x^-+\frac{1}{4\pi \alpha'} \int_{0}^{\ell}d \sigma(\gamma_{\sigma\sigma} \part_\tau X^i \part_\tau X^i- \gamma_{\sigma\sigma}^{-1}\part_\sigma X^i \part_\sigma X^i)~.
$$
The momentum conjugate to $x^-$ is 
$$
p_-= - p^+ = \frac{\part L}{\part(\part_\tau x^-)}=-\frac{\ell}{2\pi \alpha'}\gamma_{\sigma\sigma}~.
$$
As with $\eta$ in the particle example, $\gamma_{\sigma\sigma}$ is a momentum and not a coordinate. The momentum density conjugate to $X^i(\tau, \sigma)$ is 
$$
\Pi_i = \frac{\part L}{\part (\part_\tau X^i)} = \frac{1}{2\pi \alpha'} \gamma_{\sigma\sigma} \part_\tau X^i = \frac{p^+}{\ell}\part_\tau X^i~.
$$
The Hamiltonian is then
$$
\begin{align}
H &= p_- \part_\tau x^- + \int_0 ^\ell d \sigma ~\Pi_i\part_\tau X^i-L\nonumber\\
  & = \frac{1}{4\pi \alpha'}\int_0^\ell d\sigma(\gamma_{\sigma\sigma} \part_\tau X^i\part_\tau X^i + \gamma_{\sigma\sigma}^{-1} \part_\sigma X^i \part_\sigma X^i)
\nonumber\\
  & = \frac{\ell}{4\pi \alpha' p^+}\int_0^\ell d\sigma(2\pi \alpha' \Pi_i \Pi_i + \frac{1}{2\pi \alpha'} \part_\sigma X^i \part_\sigma X^i)~.
\end{align}
$$
This is just the Hamiltonian for $D-2$ free fields $X^i$, with $p^+$ a conserved quantity. The equations of motion are
$$
\part_\tau x^- = \part H/\part p_- = H / p^+, \quad
\part_\tau {p^+} = \part H / \part x^-= 0
$$

$$
\part_\tau X^i = \delta H / \delta \Pi_i = 2\pi \alpha' c \Pi_i, \quad \part_\tau \Pi_i = - \delta H / \delta X^i = \frac{c}{2\pi \alpha'} \part^2_\sigma X^i~.
$$

The implies the wave equation
$$
\part^2_\tau X^i = c^2 \part^2_\sigma X^i~,
$$
with velocity $c = \ell /(2\pi \alpha' p^+)$ . It is useful to choose the string coordinate length $\ell$ such that $c = 1$. Since $p^+$ is positive and conserved, the total string length is also conserved.

---

The general solution to the wave equation with boundary condition is
$$
X^i(\tau, \sigma) = x^i + \frac{p^i}{p^+}\tau + i\sqrt{2\alpha'} \sum_{n\in \mathbb{Z}_*} \frac{1}{n} \alpha_n^i \exp\left(-\frac{\pi i n c\tau}{\ell}\right) \cos\left(\frac{\pi n \sigma}{\ell}\right)~.
$$

Reality of $X^i$ requires $(\alpha^i_{n})^\dagger = \alpha^i_{-n}$ . Recall the center-of-mass variables
$$
\begin{align}
x^i(\tau) &= \frac 1 \ell \int_0^\ell d\sigma X^i(\tau, \sigma)~,\\
p^i(\tau) &= \int_0^\ell d\sigma ~\Pi_i(\tau, \sigma) = \frac{p^+}{\ell} \int_0^\ell d\sigma ~\part_\tau X^i(\tau,\sigma)~,
\end{align}
$$
which are the average position and the toal momentum. 

To quantize, impose the equal time canonical commutation relations
$$
[x^-, p^+] = i \eta^{-+} = -i,\quad [X^i(\sigma)~, \Pi^j(\sigma')] = i \delta^{ij}\delta(\sigma-\sigma')~.
$$
In terms of the Fourier components,
$$
[x^i,p^j] = i \delta^{ij}, \quad [\alpha^i_m~, \alpha^j_n] = m \delta^{ij} \delta_{m,-n}~.
$$
For each $m$ and $i$ the modes satisfy a harmonic oscillator algebra with normailization
$$
\alpha^i_m = \sqrt{m}\, a~, \quad \alpha^i_{-m} = \sqrt{m}\, a^\dagger~, \quad m>0~,
$$
where $[a, a^\dagger] = 1$. The oscillators are labeled by the direction of oscillation $i$ and the harmonic $m$ .

---

The state $|0;k\rang$ where $k = (k^+, k^i)$ is defined to be annihilated by the lowering operators and to be an eigenstate of the center-of-mass momenta,
$$
p^+ |0;k\rang = k^+|0;k\rang~, \quad p^i|0;k\rang = k^i |0;k\rang~,\quad \alpha^i_m|0;k\rang = 0~,\quad m>0~.
$$
A general state can be built by acting on $|0;k\rang$ with the raising operators,
$$
|N;k\rang = \prod_{i = 2}^{D-1} \prod_{n=1}^\infty \frac{(\alpha^i_{-n})^{N_{in}}}{\sqrt{n^{N_{ in }}N_{in}!}} |0;k\rang~,
$$
where $N_{in}$ is the occupation number for each mode $(i,n)$ .

**Note** the states form a Hilber space $\mathscr H_1$ of a single open string and the state $|0;0\rang$ is the ground state of single string with zero momentum, not the zero-string vacuum state, denoted by $|{\rm vacuum}\rang$ . The full Hilbert space of string theory
$$
\mathscr H = |{\rm vacuum}\rang \oplus \mathscr H_1 \oplus \mathscr H_2 \oplus \cdots~.
$$

---

Inserting the mode expansion into the Hamiltonian gives
$$
H = \frac{p^i p^i}{2 p^+} + \frac{1}{2p^+\alpha'}\left(\sum_{n=1}^\infty \alpha^i_{-n} \alpha^i_n + A\right)~.
$$
Hint on calculation, first convert production of sines and cosines into the sum of cosines, then perform the integral. The unknown constant $A$ is from the commutators. How to determine this constant?

- Find Lorentz transformation generators $M^{\mu \nu}$
- Calculate their algebra with $p^\mu$ and each other
- We can find that $A = -1$
- and only if the spacetime dimensionality is precisely $D = 26$ .

Considering summing the zero-point energies
$$
A = \frac{D-2}{2} \sum_{n=1}^\infty n~ = -\frac{D-2}{24}~.
$$
Then 
$$
m^2 = 2p^+ H - p^i p^i = \frac{1}{\alpha'} \left(N + \frac{2 - D}{24}\right)~,
$$
where $N$ is the **level**
$$
N = \sum_{i = 2}^{D-1} \sum_{n = 1}^\infty n N_{in}~.
$$

---

Let us look at some light string states. The lightest is
$$
|0;k\rang~, \quad m^2 = \frac{2-D}{24 \alpha'}~.
$$
The state is a tachyon. The lowest excited states of the string are
$$
\alpha^i_{-1} |0;k\rang~, \quad m^2 = \frac{26 - D}{24 \alpha'}~.
$$
How Lorentz invariance requires a specific value of D?

> The analysis of spin is different for massive and massless particles. For a massive particle, one goes to the rest frame $p^\mu = (m,0,\cdots,0)$. The internal states then form a representation of the spatial rotation group $SO(D-1)$ . For a massless particle there is no rest frame; choose the frame $p^\mu = (E, E, 0, \cdots,0)$ . The $SO(D-2)$ acting on the transverse directions leaves $p^\mu$ invariant, and the internal states form a representation of this smaller group.

In $D$ dimensions, a massive vector particle thus has $D-1$ spin states while a massless vector need have only $D-2$ states. At the first level, we found only the $D-2$ states $\alpha^i_{-1}|0;k\rang$ , so these must be massless and 
$$
A = -1, \quad D = 26~.
$$

> The spectrum is Lorentz-invariant **only** if the number of spacetime dimensions is $D = 26$ . The classical theory is Lorentz-invariant for any $D$ but there is an anomaly, the symmetry is no preserved by the quantization except when $D = 26$.

