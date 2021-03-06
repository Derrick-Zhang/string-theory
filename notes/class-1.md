## Action principles

What we are studying?

- classical and quantum mechanics of a one-dimensional object, a string

- String moves in $D$ flat spacetime dimensions, with metric
  $$
  \eta = {\rm diag}(-,+,+,\cdots,+)
  $$

---

### Point particle

The spacetime position is prametrized by $\tau$, and we write $X^\mu(\tau)$ . The action is given by
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

 It is useful to introduce an auxiliary field on the worldline, the worldline metrix $\gamma_{\tau \tau}(\tau)$ . Writing $\eta(\tau) = \sqrt{-\gamma_{\tau\tau}(\tau)}$ , we can define another action
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

We wil use $x$ to denote spacetime coordinates and $X$ for world-sheet coordinates. Define light-cone coordinates in spacetime:
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

- point particle

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

- open string

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
  The action then becomes

  