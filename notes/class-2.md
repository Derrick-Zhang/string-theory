# Conformal field theory

## Massless scalars in two dimension

The complex coordinates are
$$
z = \sigma^1 + i \sigma^2, \quad \bar z = \sigma^1 - i \sigma^2~.
$$
Define also
$$
\part_z = \frac12 (\part_1 - i\part_2), \quad \part_{\bar z} = \frac12 (\part_1 + i \part_2)~.
$$
Then
$$
\part z = 1, \quad \part \bar z = 0, \quad \bar \part z = 0, \quad \bar \part \bar z = 0~.
$$
For a general vector $v^a$,
$$
v^z = v^1 + i v^2, \quad v^{\bar z} = v^1 - i v^2,\quad  v_z = \frac12(v^1 - i v^2), \quad v_{\bar z} = \frac12 (v^1+iv^2)~.
$$
Therefore,
$$
g_{z\bar z} = g_{\bar z z} = \frac12, \quad g^{z\bar z} = g^{\bar z z} = 2~.
$$
Note that also
$$
d^2 z = 2 d\sigma^1 d\sigma^2
$$
We define
$$
\int d^2 z \delta (z,\bar z) = 1
$$
so that $\delta^2(z,\bar z) = \frac12  \delta (\sigma^1) \delta(\sigma^2)$. Now we are only considering Euclidean metric, for Minkowski metric, use $\sigma^2 = i \sigma^0$.

---

Expectation values are defined by
$$
\lang f[X]\rang = \int [dX] \exp(-S) f[X]~,
$$
where $f[x]$ is any functional of $X$.

Since
$$
0 = \int [dX] \frac{\delta}{\delta X_\mu(z,\bar z)} \exp(-S)... = \frac{1}{\pi \alpha'} \lang\part \bar \part X^\mu(z,\bar z)...\rang
$$
Thus
$$
\lang \part \bar \part X^\mu(z,\bar z)...\rang = 0~, {\rm with~insertions~away~from~}z
$$

---

What if insertions are coincident with $z$?
$$
\begin{align}
0 &= \int [dX] \frac{\delta}{\delta X_\mu(z, \bar z)} [\exp(-S) X^\nu(z', \bar z')]\\
  &= \int [dX] \exp(-S) [\eta^{\mu \nu} \delta^2(z-z', \bar z - \bar z') + \frac{1}{\pi \alpha'} \part \bar \part X^\mu(z, \bar z) X^\nu(z',\bar z')]\\
  &= \eta^{\mu \nu} \lang \delta^2(z - z', \bar z - \bar z')\rang + \frac{1}{\pi \alpha'} \part \bar \part \lang X^\mu(z,\bar z) X^\nu(z', \bar z') \rang~.
\end{align}
$$
Thus
$$
\frac{1}{\pi \alpha'} \part \bar \part X^\mu(z, \bar z) X^\nu(z', \bar z') = - \eta^{\mu \nu} \delta^2(z-z', \bar z - \bar z')~.
$$

---

Now we introduce normal ordering.
$$
\begin{align}
:X^\mu(z, \bar z): &= X^\mu(z, \bar z)\\
:X^\mu(z_1, \bar z_1)X^\nu(z_2, \bar z_2): &= X^\mu(z_1, \bar z_1) X^\nu(z_2, \bar z_2) + \frac{\alpha'}{2}\eta^{\mu \nu} \ln|z_1 - z_2|^2 
\end{align}
$$
 Notice that under this definition, we have
$$
\part \bar \part :X^\mu(z_1, \bar z_1)X^\nu(z_2, \bar z_2): ~= 0
$$
This follows from
$$
\part \bar \part \ln|z|^2 = 2 \pi \delta^2(z, \bar z)~.
$$

> This is obvious for $z \neq 0$. And we integrate both sides using divergence theorem in complex coordinates.
> $$
> \int _R d^2 z (\part v + \bar \part \bar v) = i \int_{\part R}(v d\bar z - \bar v dz)~.
> $$
> where the contour integral circles the region $R$ counterclockwise.
>
> Then
> $$
> \frac 12 \int_R d^2 z ~[\part (\bar \part \ln|z|^2)+\bar \part (\part \ln|z|^2)]\\ 
> = \frac12 \int_R d^2 z \left(\part \frac{1}{\bar z} + \bar \part \frac1z\right)
> = \frac i2 \int_{\part R} \left(\frac{d \bar z}{\bar z} - \frac{d z}{z}\right) = 2\pi~.
> $$

## The operator product expansion

The basic object of interest in string perturbation theory will be the path integral expectation value of a product of local operators,
$$
\lang \mathscr A_{i_1} (z_1, \bar z_1) \mathscr{A}_{i_2}(z_2, \bar z_2) \cdots \mathscr A_{i_n} (z_n, \bar z_n) \rang~,
$$
where $\mathscr A_i$ is some basis for the set of local operators. What if two operators  are taken to approach each other? The description of this limit is the **operator product expansion**. It states that a product of two local operators close together can be approximated to arbitrary accuracy by a sum of local operators,
$$
\mathscr A_i(\sigma_1) \mathscr A_j(\sigma_2) = \sum_k c^k_{ij}(\sigma_1 - \sigma_2) \mathscr A_k(\sigma_2)
$$
We have seen that the normal ordered product satisfies the naive equation of motion. Thus
$$
\begin{align}
X^\mu (z) X^\nu(w) &= -\frac{\alpha'}{2} \eta^{\mu \nu} \ln|z - w|^2 + :X^\mu(z)X^\nu(w):\\
&= -\frac{\alpha'}{2} \eta^{\mu\nu}\ln|z-w|^2 + :X^\mu(w)X^\nu(w): + \sum_{k=1}^\infty\frac{1}{k!} [(z-w)^k:X^\nu\part^kX^\mu(w):] + (\bar z - \bar w)^k :X^\nu \bar \part ^k X^\mu(w):
\end{align}
$$
The definition of normal ordering for arbitrary numbers of fields can be given recursively as
$$
:X^{\mu_1}(z_1, \bar z_1) \cdots X^{\mu_n}(z_n, \bar z_n): =X^{\mu_1}(z_1, \bar z_1) \cdots X^{\mu_n}(z_n, \bar z_n) + \sum {\rm subtractions}
$$
The subtraction between two pairs gives
$$
\frac{\alpha'}{2} \eta^{\mu_i \mu_j} \ln|z_{ij}|^2~.
$$
The OPE for any pair of operators can be generated from
$$
:\mathscr F: \,:\mathscr G: = :\mathscr F \mathscr G: + \sum {\rm cross~contractions}
$$

> Example
> $$
> \begin{align}
> &:\part X^\mu(z) \part X_\mu(z):\, :\part' X^\nu(z') \part' X_\nu(z'):\\
> &\sim 2 \left[\part \part' \left(-\frac{\alpha'}{2}\eta^{\mu \nu} \ln|z-z'|^2\right)\right]^2
> + 4 \left[\part \part' \left(-\frac{\alpha'}{2}\eta^{\mu \nu} \ln|z-z'|^2\right)\right]:\part X_\mu(z) \part' X_\nu(z'):\\
> &\sim \frac{D \alpha'^2}{2(z-z')^4}-\frac{2\alpha'}{(z-z')^2}:\part X_\mu(z) \part' X^\mu(z'):\\
> &\sim  \frac{D \alpha'^2}{2(z-z')^4}-\frac{2\alpha'}{(z-z')^2}:\part' X_\mu(z') \part' X^\mu(z'): - \frac{2\alpha'}{z-z'}:\part'^2 X_\mu(z') \part' X^\mu(z'):~.
> \end{align}
> $$
> Another example
> $$
> \begin{align}
> :e^{ik_1 X(z,\bar z)}:\,:e^{ik_2 X(0,0)}:~ &= \exp\left(-\frac{\alpha'}{2} \int d^2 z_1 d^2 z_2 \ln|z_{12}|^2 \frac{\delta}{\delta X^\mu(z_1, \bar z_1)}\frac{\delta}{\delta X_\mu(z_2, \bar z_2)}\right) :e^{ik_1 X(z,\bar z)} e^{ik_2 X(0,0)}:\\
> &= \exp\left(\frac{\alpha'}{2} k_1 k_2 \ln|z|^2\right) :e^{ik_1 X(z,\bar z)} e^{ik_2 X(0,0)}: = |z|^{\alpha' k_1 k_2} :e^{ik_1 X(z,\bar z)} e^{ik_2 X(0,0)}:~.
> \end{align}
> $$
> To get OPE, Taylor expand inside the normal ordering to give
> $$
> :e^{ik_1 X(z,\bar z)}:\,:e^{ik_2 X(0,0)}:~ =~|z|^{\alpha' k_1 k_2} :e^{i (k_1 + k_2) X(0,0)} [1+ O(z,\bar z)]:
> $$

## Ward identities and Nother's theorem

Let there be a symmetry
$$
\phi'_\alpha(\sigma) = \phi_\alpha(\sigma) + \delta \phi_\alpha(\sigma),
$$
where $\delta \phi_\alpha$ is proportional to an infinitesimal parameter $\varepsilon$. The product of the path integral measure and the weight $\exp(-S)$ is invariant,
$$
[d \phi'] \exp(-S[\phi']) = [d \phi] \exp(-S[\phi])~.
$$




