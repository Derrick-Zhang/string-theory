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

