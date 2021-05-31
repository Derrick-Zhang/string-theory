# Bosonic string theory

We study the closed oritented bosonic strings in 26 dimensional Euclidean space. The Polyakov action
$$
S= \frac{1}{2\pi} \int_{\Sigma_g} d^2 \sigma \sqrt{\gamma} \gamma^{\alpha \beta} \partial_\alpha X^\mu \partial_\beta X_\mu - \frac{\lambda}{4\pi} \int_{\Sigma_g} d^2 \sigma \sqrt{\gamma} R
$$
where $\Sigma_g$ is a Riemann surface with genus $g$. The second term it proportional to the Euler characteristic $\chi = 2- 2g$ and, hence, determines the relative ratio of multi-loop amplitudes. The $g$-loop amplitude is proportional to $\exp(-\lambda g)$

## Differential geometry on Riemann surfaces

### Metric and complex structure

Let $\Sigma_g$ be a Riemann surface of genus $g$. We may introduce, in any chart $U$, the **isothermal coordinates** $(\sigma^1, \sigma^2)$ in which the metric is conformally flat,
$$
g = e^{2 \omega(\sigma)} (d\sigma^1 \otimes d\sigma^1 + d\sigma^2 \otimes d\sigma^2)~.
$$
Introduce the complex coordinates
$$
z = \sigma^1 + i \sigma^2, \quad \bar z = \sigma^1 - i \sigma^2~.
$$
Forms and vectors are spanned by
$$
dz = d\sigma^1 + i d\sigma^2, \quad d\bar z = d\sigma^1 - i d\sigma^2
$$

$$
\partial_z = \frac{1}{2} (\partial_{\sigma^1} - i \partial_{\sigma^2}), \quad \partial_{\bar z} = \frac12(\partial_{\sigma^1} + i \partial_{\sigma^2})~.
$$

In terms of the complex coordinates, the metric takes the form
$$
g = \frac12 e^{2 \omega(z, \bar z)} (dz \otimes d\bar z + d \bar z\otimes dz)
$$
Let $V$ be another chart on $\Sigma_g$ such that $U \cap V \neq \emptyset$. The metric in $V$ is
$$
g = e^{2\omega'(u, \bar u)} d u \otimes d\bar u
$$
We should have
$$
e^{2\omega(z,\bar z)} dz \otimes d\bar z = e^{2\omega'(u,\bar u)} du \otimes d\bar u
$$
Since
$$
du \otimes d \bar u = \left(\frac{\partial u}{\partial z}dz + \frac{\partial u}{\partial \bar z} d\bar z\right) \otimes \left(\frac{\partial \bar u}{\partial z} dz + \frac{\partial \bar u}{\partial \bar z} d\bar z\right)
$$
We must have 
$$
\frac{\partial u}{\partial \bar z} = \frac{\partial \bar u}{\partial z} = 0
$$
Therefore,
$$
u = u(z), \quad \bar u = \bar u(\bar z)
$$
which verfies that $\Sigma_g$ is a complex manifold. We also have
$$
e^{2 \omega(z, \bar z)} = e^{2 \omega'(u, \bar u)} |\partial u / \partial z|^2
$$

### Vectors, forms and tensors

We only need to consider tensors with pure $z$-indeices. The tensor transforms under $z \to u$ as
$$
T \to \left(\frac{\partial u}{\partial z}\right)^n T
$$
where $n$ is called the **helicity** and is defined as the number of upper $z$-indices minus the number of lower $z$-indices. Therefore, the tensor $T^z_{~z}$ is left invariant and is regarded as a scalar.

In real indices, the helicity $\pm 1$ vectors are given by $V^1 \pm i V^2$. This follows since
$$
V^1 \partial_{\sigma_1} + V^2 \partial_{\sigma^2} = (V^1 + i V^2) \partial_z + (V^1 - i V^2)\partial_{\bar z}~.
$$
We put $V^z = V^1 + i V^2$ and $V^{\bar z} = V^1 - i V^2 \simeq V_z$. The helicity $\pm 2$ tensors are $T^{11}\pm iT^{12}$, where $T$ is a symmetric traceless tensor of rank two.
$$
T^{11}(\partial_{\sigma^1} \otimes \partial_{\sigma^1} - \partial_{\sigma^2} \otimes \partial_{\sigma^2}) + T^{12}(\partial_{\sigma^1} \otimes \partial_{\sigma^2}+ \partial_{\sigma^2} \otimes \partial_{\sigma^1}) = 2(T^{11}+i T^{12})\partial_z \otimes \partial _z + 2(T^{11}- i T^{12}) \partial_{\bar z} \otimes \partial_{\bar z}~.
$$

### Covariant derivatives

