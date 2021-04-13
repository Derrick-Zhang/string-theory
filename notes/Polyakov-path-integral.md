# The Polyakov path integral

## The Polyakov path integral

We use the Euclidean worldsheet metric $g_{ab}(\sigma^1, \sigma^2)$ with signature $(+,+)$. The integral runs over all Euclidean metrics and over all embeddings $X^\mu(\sigma^1, \sigma^2)$ of the worldsheet in Minkowski spacetime,
$$
\int [d X \, dg] \exp(-S)
$$
The Euclidean action is 
$$
S = S_X + \lambda \chi~,
$$
with
$$
S_X = \frac{1}{4\pi \alpha'} \int_M d^2 \sigma \sqrt{g} g^{ab}\part_a X^\mu \part_b X_\mu~,\\
\chi = \frac{1}{4\pi} \int_M d^2 \sigma \sqrt{g} R + \frac{1}{2\pi} \int_{\part M} ds k~,
$$
where $k$ is the geodesic curvature of the boundary.

---

- One important thing to note is the equivalence of the Minkowski and Euclidean path integrals. They define the same amplitudes, respectively in the light-cone and conformal gauges. 
- Also, $\chi$ is locally a total derivative in two dimensions and therefore depends only on the topology of the world-sheet, it is the Euler number of the world-sheet.
- We can define the open string coupling as $g \sim e^{\lambda/2}$ and closed string coupling as $g \sim e^{\lambda}$.

## Gauge fixing

The path integral above is not exactly correct. It contains a lot of redundancy because configurations $(X, g)$ and $(X', g')$ that are related to one another by the local diff$\times$Weyl symmetry represent the same physical configuration. We need to divide by the volume of this local symmetry group.
$$
\int \frac{[d X dg]}{V_{\rm diff \times Weyl}} \exp(-S) \equiv Z~.
$$
How to carry out this integration?

- gauge-fixing
- integrating over a slice that cuts through each gauge equivalence class once
- obtaining the correct measure on the slice by the Faddeev-Popov method

---

Note that the symmetric metric has three independent components, and there are three gauge functions, the two coordinates and the local scale of the metric. Thus there is just enough gauge freedom to eliminate the integration over the metric, fixing it at some specific functional form which we will call the _fiducial_ metric,
$$
g_{ab} (\sigma) \to \hat g_{ab} (\sigma)~.
$$
A simple choice is the flat or _unit gauge_ metric
$$
\hat g_{ab} (\sigma) = \delta_{ab}
$$
We can consider the effect of Weyl group alone by using the _conformal gauge_
$$
\hat g_{ab}(\sigma) = \exp(2\omega(\sigma)) \delta_{ab}
$$

---

There is a little bit of extra gauge freedom: there are diff$\times$Weyl transformations that leave the metric in unit gauge. In complex coordinate $z = \sigma^1 + i \sigma^2$, the flat metric is $ds^2 = dz d\bar z$. Consider a coordinate transformation such that $z'$ is a holomorphic function of $z$,
$$
z' = f(z),
$$
combined with a Weyl transformation. The new metric is
$$
ds'^2 = \exp(2\omega) |\partial_z f|^{-2} dz' d\bar z'~.
$$
Then for
$$
\omega = \ln|\partial_z f|
$$
the metric is invariant. However, this extra gauge freedom does not conflict with our earlier counting because the set of holomorphic reparameterizations, is of measure zero compared to all reparameterizations.

### The Faddeev-Popov determinant

Let $\zeta$ be shorthand for a combined coordinate and Weyl transformation,
$$
\zeta: g \to g^{\zeta}, \quad g^\zeta_{ab} (\sigma') = \exp(2\omega(\sigma)) \frac{\partial \sigma^c}{\partial \sigma'^a}\frac{\partial \sigma^d}{\partial \sigma'^b} g_{cd}(\sigma)~.
$$
We define the Faddeev-Popov measure $\Delta_{\rm FP}$ by
$$
1 = \Delta_{\rm FP} (g) \int [d\zeta] \delta(g - \hat g^\zeta)
$$
where $\hat g_{ab}$ is the fiducial metric, $[d\zeta]$ is a gauge-invariant measure on the diff$\times$Weyl group. The delta function is actually a delta functional because $g$ depends on the local coordinate $\sigma$.

---

Inserting this into the path integral
$$
Z[\hat g] = \int \frac{[d\zeta\, dX\, dg]}{V_{\rm diff \times Weyl}} \Delta_{\rm FP}(g)\delta(g - \hat g^\zeta) \exp(-S[X,g])~.
$$
Carry out the inegration over $g_{ab}$ and also rename the dummy variable $X \to X^\zeta$, to obtain
$$
Z[\hat g] = \int \frac{[d\zeta \, dX^\zeta]}{V_{\rm diff \times Weyl}} \Delta_{\rm FP}(\hat g^\zeta) \exp(-S[X^\zeta, \hat g^\zeta])~.
$$

> Gauge invariance of $\Delta_{\rm FP}$ is shown as
> $$
> \Delta_{\rm FP}(g^\zeta)^{-1} = \int [d\zeta']\, \delta(g^\zeta - \hat g^{\zeta'}) = \int [d\zeta'] \, \delta(g - \hat g^{\zeta^{-1} \zeta'}) = \int [d\zeta''] \delta(g - \hat g^{\zeta''}) = \Delta_{\rm FP}(g)^{-1}
> $$
> where $\zeta'' = \zeta^{-1} \zeta'$. We have used the gauge invariance of the delta function and the measure.

Since the Faddeev-Popov determinant, the action and the integral measure $[dX]$ are gauge invariant, we obtain
$$
Z[\hat g] = \int \frac{[d\zeta dX]}{V_{\rm diff\times Weyl}} \Delta_{\rm FP}(\hat g) \exp(-S[X,\hat{g}])~.
$$
Finally, nothing in the integrand depends on $\zeta$, so the integral over $\zeta$ just produces the volume of the gauge group and cancels the denominator, leaving
$$
Z[\hat g] = \int [dX] \Delta_{\rm FP}(\hat g) \exp(-S[X,\hat g])~.
$$
Thus, $\Delta_{\rm FP}(\hat g)$ is the correct measure on the slice.

---

For $\zeta$ near the identity, we can expand
$$
\delta g_{ab} = 2 \delta \omega g_{ab} - \nabla_a \delta \sigma_b - \nabla_b \delta \sigma_a
= (2 \delta \omega - \nabla_c \delta \sigma^c) g_{ab} - 2(P_1 \delta \sigma)_{ab}~.
$$
We have defined a differential operator $P_1$ that takes vectors into traceless symmetric 2-tensors.
$$
(P_1 \delta \sigma)_{ab} = \frac12(\nabla_a \delta \sigma_b + \nabla_b \delta \sigma_a -g_{ab} \nabla_c \delta \sigma^c)~.
$$
Near the identity, we have
$$
\Delta_{\rm FP} (\hat g)^{-1} = \int [d \delta \omega\, d \delta \sigma] \delta [-(2 \delta \omega - \hat \nabla \delta \sigma)\hat g + 2 \hat P_1 \delta \sigma]\\
= \int [d \delta \omega\, d\beta\, d \delta \sigma] \exp\left\{ 2\pi i \int d^2 \sigma \sqrt{\hat g} \beta^{ab} [-(2 \delta \omega - \hat \nabla \delta \sigma)\hat g + 2 \hat P_1 \delta \sigma]_{ab}\right\}\\
= \int [d \beta' d \delta \sigma] \exp\left\{4 \pi i \int d^2 \sigma \sqrt{\hat g} \beta'^{ab}(\hat P_1 \delta \sigma)_{ab}\right\}
$$
where we integrate over $\delta \omega$, which produces a delta function forcing $\beta^{ab}$ to be traceless. Therefore, it is a functional integral over a vector field $\delta \sigma^a$ and over a traceless symmetric tensor $\beta'^{ab}$.

---

We can invert this path integral by replacing each bosonic field with a corresponding Grassmann ghost field
$$
\delta \sigma^a \to c^a, \quad \beta'_{ab} \to b_{ab}
$$
with $b^{ab}$ being traceless. Thus
$$
\Delta_{\rm FP}(\hat g) = \int [db dc] \exp(-S_g),
$$
where the ghost action $S_g$ is given by
$$
S_g = \frac{1}{2\pi} \int d^2 \sigma\sqrt{\hat g} b_{ab} \hat \nabla^a c^b = \frac{1}{2\pi} \int d^2 \sigma \sqrt{\hat g} b_{ab} (\hat P_1 c)^{ab}~.
$$
Locally on the world-sheet, the Polyakov path integral is now
$$
Z[\hat g] = \int [dX\, db\, dc] \exp(-S_X - S_g)~. 
$$
The result is listed without proof,
$$
Z[\hat g] = (\det \hat \nabla^2)^{-D/2} \det\hat P_1~,
$$
the first determinant coming from the $X$ integration and the second from the ghost integration.

---

In conformal gauge, $\hat g_{ab}(\sigma) = \exp(2\omega(\sigma))\delta_{ab}$, the ghost action is
$$
S_g = \frac{1}{2\pi} \int d^2z b_{zz} \left(\nabla_{\bar z} c^z + b_{\bar z\bar z} \nabla_z c^{\bar z}\right) = \frac{1}{2\pi} \int d^2z b_{zz} \left(\partial_{\bar z} c^z + b_{\bar z\bar z} \partial_z c^{\bar z}\right)
$$
This is a $bc$ CFT with $(h_b, h_c) = (2,-1)$.

In the gauge-fixed form, the essential content of the gauge symmetry is still present as BRST invariance.

## The Weyl anomaly

The anomaly is in the Weyl symmetry, $T^a_{~a}$ vanishes classically, but not in the quantum theory. We need to check if 
$$
Z[g^\zeta] = Z[g] ?
$$
We will also be interested in path integrals wiith additional insertions,
$$
\langle ... \rangle_g \equiv \int [dX\, db\, dc] \exp(-S[X, b,c,g])...~.
$$
Then we also require
$$
\langle ... \rangle_{g^\zeta}  = \langle ... \rangle_g ~.
$$

---

The energy-momentum tensor $T^{ab}$ is the infinitesimal variation of the path integral with respect to the metric
$$
\delta \langle ... \rangle_g = - \frac{1}{4\pi} \int d^2 \sigma \sqrt{g(\sigma)} \delta g_{ab}(\sigma) \langle T^{ab}(\sigma) ... \rangle_g~.
$$
Classically, $T^{ab}$ comes entirely from the variation of the action, and this coincides with the Noether definition
$$
T^{ab}(\sigma)  = \frac{4\pi}{\sqrt{g(\sigma)}} \frac{\delta}{\delta g_{ab}(\sigma)}S.
$$
For a Weyl transformation, we have
$$
\delta_W \langle ... \rangle_g = - \frac{1}{2\pi} \int d^2 \sigma \sqrt{g(\sigma)} \delta \omega(\sigma) \langle T^{a}_{~a}(\sigma) ... \rangle_g~.
$$
Classically, $T^a_{~a}$ vanishes, but in the quantum theory,
$$
T^a _{~a} = a_1 R
$$

---

**Calculation of the Weyl anomaly** 

In conformal gauge,
$$
T_{z \bar z} = \frac{a_1}{2} g_{z \bar z} R~.
$$
Taking the covariant derivative,
$$
\nabla^{\bar z} T_{z \bar z} = \frac{a_1}{2} \nabla^{\bar z} (g_{z \bar z} R) = \frac{a_1}{2} \partial_z R~,
$$
where we have used the fact that the metric is covariantly constant. Then by conservation of $T_{ab}$,
$$
\nabla^z T_{zz} = - \nabla^{\bar z} T_{\bar z z} = - \frac{a_1}{2} \partial_z R~.
$$

> The Weyl transformation of Ricci scalar is
> $$
> \sqrt{g'}R' = \sqrt{g} (R - 2 \nabla^2 \omega)
> $$

The Weyl transformation of the right is
$$
a_1 \partial_z \nabla^2 \delta \omega \approx 4 a_1 \partial_z^2 \partial_{\bar z} \delta \omega~,
$$
To get the Weyl transformation of $T_{zz}$ we use first the conformal transformation
$$
\epsilon^{-1} \delta T_{zz} (z) = - \frac{c}{12} \partial^3_z v^z(z) - 2 \partial_z v^z(z) T_{zz}(z) - v^z(z) \partial_z T_{zz}(z)~.
$$
This confromal tansformation consists of a coordinate transformation $\delta z = \epsilon v$ plus a Weyl transformation $2 \delta \omega = \epsilon \partial v + \epsilon (\partial v)^*$. The last two terms in the variation are the coordinate transformation of the tensor, so the Weyl  transformation, to leading order around flat space, is
$$
\delta_W T_{zz} = -\frac{c}{6} \partial_z^2 \delta \omega
$$
Acting with $\partial ^z = 2\partial _ {\bar z}$ and compare with above formula, we obtain,
$$
c = - 12 a_1, \quad T^{a}_{~a} = -\frac{c}{12}R~.
$$

## Scattering amplitudes

Each string source becomes a local disturbance on the world-sheet. To a given incoming or outgoing string, with $D$-momentum $k^\mu$ and internal state $j$, there corresponds a local **vertex operator** $\mathscr V_j(k)$. Incoming and outgoing states are distinguished by the sign of $k^0$. An $n$-particle S-matrix element is given by
$$
S_{j_1,..., j_n} (k_1, ... , k_n) = \sum \int \frac{[dX\, dg]}{V_{\rm diff \times Weyl}} \exp(-S_X - \lambda\chi) \prod_{i=1}^n \int d^2 \sigma_i \sqrt{g(\sigma_i)} \mathscr V_{j_i}(k_i, \sigma_i)~,
$$
where the summation is over compact topologies. To make the vertex operator insertions diff-invariant, we have integrated them over the world-sheet.

Any compact, connected, oriented two-dimensional surface without boundary is topologically equivalent to a sphere with $g$ handles; $g$ is known as the **genus** of the surface. Any compact, connected, oriented two-dimensinal surface is topologically equivalent to a sphere with $g$ handles and $b$ holes.

To describe unoriented surfaces, it is useful to introduce the cross-cap, cut a hole in the surface and identify diametrically opposite points. Any compact, connected closed surface, can be obtained by adding $g$ handles, $b$ holes and $c$ cross-caps to the sphere.

>  Besides cross-caps and handles, we can add cross-handles. These three classes are not independent
>
> - A cross-handle is homeomorphic to two cross-caps
> - Handles and cross-handles are equivalent in the presence of a crosscap

The Euler number is given by
$$
\chi = 2- 2g - b-c~.
$$

## Vertex operators

Using the state-operator mapping, the vertex operator for the closed string tachyon is
$$
V_0 = 2 g_c \int d^2 \sigma \sqrt{g} e^{ikX} \to g_c \int d^z :e^{ikX}:
$$
The (diff$\times$Weyl)-invariance requires that the operator is a tensor  of weight $(1,1)$. By a straightforward OPE calculation, $e^{ikX}$ is a tensor of weight $h = \bar h = \alpha' k^2/4$, so the condition is
$$
m^2 = -k^2 = - \frac{4}{\alpha'}~.
$$
Similarly, the tensor states at the first excited level of the closed string have the flat world-sheet vertex operators
$$
\frac{2g_c}{\alpha'} \int d^2 z :\partial X^\mu \bar \partial X^\nu e^{ik\cdot X}:
$$

## Strings in curved spacetime

$$
S_\sigma = \frac{1}{4\pi \alpha'} \int_M d^2 \sigma \sqrt{g} [(g^{ab} G_{\mu \nu}(X) + i \epsilon^{ab} B_{\mu \nu}(X)) \partial_a X^\mu \partial_b X^\nu + \alpha' R \Phi(X)]~.
$$

The field $B_{\mu \nu} (X)$ is the antisymmetric tensor, and the dilaton involves both $\Phi$ and the diagonal part of $G_{\mu \nu}$.

One can think of the fields $X^\mu$ as being coordinates on a manifold. This is called the **target space**, because the $X^\mu$ define an embedding,
$$
{\rm world~ sheet \to target}
$$
A field theory in which the kinetic term is field dependent and so field space is effectively a curved manifold, is known for historic reasons as a **nonlinear sigma model**.