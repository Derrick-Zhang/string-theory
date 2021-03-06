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
  X' ^ \mu (\tau, \sigma) &= \Lambda^\mu_{~\nu} X^\nu(\tau, \sigma) + a^\mu,\\
  \gamma'_{ab} (\tau, \sigma) &= \gamma_{ab} (\tau, \sigma)
  \end{align}
  $$
  

- World-sheet diffeomorphism invariance:

- Weyl invariance:



