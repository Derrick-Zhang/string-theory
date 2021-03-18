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
A continuous symmetry in field theory implies the existense of a conserved current (**Nother's theorem**) and also **Ward identities**, which constrain the operator products of the current. To derive these results consider the change of variables,
$$
\phi'_\alpha(\sigma) = \phi_\alpha(\sigma) + \rho(\sigma) \delta \phi_\alpha(\sigma)~.
$$
This is not a symmetry. The path integral measure times $\exp(-S)$ would be invariant if $\rho$ were a constant, so its variation must be proportional to the gradient $\part_a \rho$,
$$
[d\phi']\exp(-S[\phi']) = [d\phi] \exp(-S[\phi])\left[1 + \frac{i\epsilon}{2\pi}\int d^d \sigma \sqrt{g} j^a(\sigma) \part_a \rho(\sigma) + O(\epsilon^2) \right]
$$
The unknow coefficient $j^a(\sigma)$ comes from the variation of the measure and the action, both of which are local, and so it must be a local function of the fields and their derivatives. Take the function $\rho$ to be nonzero only in a small region, and consider a path integral with general insertions '...' _outside_ this region. The insertions are therefore invariant under the change of $\phi_\alpha$. Invariance of the path integral under change of variables gives
$$
0 = \int [d\phi']\exp(-S[\phi'])\,... - \int [d\phi] \exp(-S[\phi])\,... = \frac{\epsilon}{2\pi i} \int d^d \sigma\sqrt{g}\, \rho(\sigma) \lang \nabla_a j^a(\sigma)\,...\rang,
$$
Thus we have $\nabla_a j^a = 0$ as an operator equation. This is Nother's theorem.

To derive the Ward identity, let $\rho(\sigma)$ be 1 in some region $R$ and 0 outside $R$. Also, include in the path integral some general local operator $\mathscr A(\sigma_0)$ at a point $\sigma_0$ inside $R$, and the usual arbitrary insertions '...' outside. Proceeding as above we obtain the operator relation
$$
\delta \mathscr A(\sigma_0) + \frac{\epsilon}{2\pi i} \int_R d^d \sigma \sqrt{g}\, \nabla_a j^a(\sigma) \mathscr A(\sigma_0) = 0.
$$
Equivalently,
$$
\nabla_a j^a(\sigma) \mathscr A (\sigma_0) = \frac{1}{\sqrt{g}} \delta^d(\sigma-\sigma_0) \frac{2\pi}{i \epsilon} \delta \mathscr A(\sigma_0) + {\rm total~}\sigma{\rm -derivative}~.
$$
The divergence theorem gives
$$
\int _{\part R} d A n_a j^a \mathscr A(\sigma_0) = \frac{2\pi}{i \epsilon} \delta \mathscr{A}(\sigma_0)
$$
This relates the integral of the current around the operator to the variation of the operator. Going to two flat dimensions this becomes
$$
\int_{\part R}(j dz - \bar jd\bar z)  \mathscr A(z_0, \bar z_0) = \frac{2\pi}{\epsilon}\delta \mathscr A(z_0, \bar z_0)~,
$$
where on the current the omitted indices are implicitly lower.

---

It is important that Noether's theorem and the Ward identity are local properties, which do not depend on whatever boundary conditions we might have far away, nor even on whether these are invariant under the symmetry. In particular, since the function $\rho(\sigma)$ is nonzero only inside $R$, the symmetry transformation need only be defined there.

In conformally invariant theories it is usually the case that $j_z$ is holomorphic and $j_{\bar z}$ antiholomorphic, except for singluarities at the other fields. In this case, the currents $(j_z,0)$ and $(0, j_{\bar z})$ are separately conserved. The integral then picks out the residues in the OPE,
$$
{\rm Res}_{z\to z_0} j(z) \mathscr A(z_0, \bar z_0) + \overline{\rm Res}_{\bar z \to \bar z_0} \bar j(\bar z) \mathscr A(z_0, \bar z_0) = \frac{1}{i\epsilon} \delta \mathscr{A}(z_0, \bar z_0)~.
$$
This form of the Ward identity is particularly convenient.

---

As an example, return to the free massless scalar and consider the **spacetime** translation $\delta X^\mu = \epsilon a^\mu$. Under $\delta X^\mu(\sigma) = \epsilon\rho(\sigma) a^\mu$,
$$
\delta S = \frac{\epsilon a_\mu}{2\pi \alpha'} \int d^2\sigma\, \part^aX^\mu \part_a \rho~.
$$
We have Noether current $a_\mu j^\mu_a$, where
$$
j^\mu_a = \frac{i}{\alpha'} \part_a X^\mu~.
$$
For the OPE of this current with the exponential operator one finds
$$
j^\mu(z) :e^{ik X(0,0)}: ~\sim \frac{k^\mu}{2z} :e^{ikX(0,0)}:,\quad \bar j^\mu(\bar z):e^{ikX(0,0)}:~\sim \frac{k^\mu}{2\bar z} :e^{ikX(0,0)}:
$$
This OPE is in agreement with the Ward identity.

---

Another example is the **world-sheet** translation $\delta \sigma^a = \epsilon v^a$, under which $\delta X^\mu = -\epsilon v^a \part_a X^\mu$. The Nother current is
$$
j_a = i v^b T_{ab}, \quad T_{ab} = - \frac{1}{\alpha'} :\left(\part_a X^\mu \part_b X_\mu - \frac{1}{2} \delta_{ab} \part_c X^\mu \part^c X_\mu\right):
$$

## Conformal invariance

The energy-momentum tensor is traceless, $T_a^{~a} = 0$. In complex coordinates this is
$$
T_{z \bar z} = 0.
$$
The conservation $\part^a T_{ab} = 0$ then implies that in any theory with $T_a^{~a} = 0$,
$$
\bar \part T_{zz} = \part T_{\bar z\bar z} = 0~.
$$
Thus,
$$
T(z) \equiv T_{zz}(z), \quad \bar T (\bar z) \equiv T_{\bar z\bar z} (\bar z)~.
$$
are respectively holomorphic and antiholomorphic. For the free massless scalar,
$$
T(z) = -\frac{1}{\alpha'} :\part X^\mu \part X_\mu:~, \quad \bar T(\bar z) = -\frac{1}{\alpha'} :\bar \part X^\mu \bar \part X_\mu: ~.
$$
The tracelessness of $T_{ab}$ implies a much larger symmetry. The currents
$$
j(z) = i v(z) T(z), \quad \bar j (\bar z) = i v(z)^* \bar T(\bar z)~.
$$
are conserved for any holomorphic $v(z)$. For the free scalar theory, one finds the OPE
$$
T(z) X^\mu(0) \sim \frac1 z\part X^\mu(0), \quad \bar T(\bar z) X^\mu(0) \sim \frac{1}{\bar z} \bar \part X^\mu(0)~.
$$
The Ward identity then gives the transformation
$$
\delta X^\mu = - \epsilon v(z) \part X^\mu - \epsilon v(z)^* \bar \part X^\mu~.
$$
This is an infinitesimal coordinate transformation $z'= z + \epsilon v(z)$. The finite transformation is
$$
X'^\mu(z', \bar z') = X^\mu(z,\bar z), \quad z' = f(z)
$$
for any holomorphic $f(z)$. This is known as a **conformal transformation**.

---

Consider the special case
$$
z' = \zeta z
$$
for complex $\zeta$. Then
$$
ds'^2 = dz' d\bar z' = \frac{\part z'}{\part z} \frac{\part \bar z'}{\part \bar z}dz d\bar z~.
$$

### Conformal invariance and the OPE

Consider the OPE of $T$ with the general operator $\mathscr A$. The OPE would be a Laurent expansion. All the singular terms are determined by the conformal transformation of $\mathscr A$.
$$
T(z) \mathscr A(0,0) \sim \sum_{n=0}^\infty \frac{1}{z^{n+1}} \mathscr A^{(n)}(0,0)
$$
The operator coefficients $\mathscr A^{(n)}$ remain to be determined.

It is convenient to take a basis of local operators that are eigenstates under rigid transformation
$$
\mathscr A'(z', \bar z') = \zeta^{-h} \bar \zeta^{-\bar h} \mathscr A(z,\bar z).
$$
The $(h,\bar h)$ are known as the **weights** of $\mathscr A$. The sum $h + \bar h$ is the dimension of $\mathscr A$, determine its behavior under scaling, while $h-\bar h$ is the spin, determining its behavior under rotations. The derivative $\part$ increases $h$ by one, and the derivative $\bar \part$ increases $\bar h$ by one.

An important special case is a **tensor operator** or **primary field** $\mathscr O$, on which a general conformal transformation acts as
$$
\mathscr O'(z', \bar z') = (\part z')^{-h}(\bar \part \bar z')^{-\bar h} \mathscr O(z,\bar z)~.
$$
The OPE  is 
$$
T(z) \mathscr O(0,0) = \frac{h}{z^2} \mathscr O(0,0) + \frac{1}{z} \part \mathscr O(0,0)+...
$$

---

Take the example of the free $X^\mu$ CFT, the weights of some typical operators are
$$
X^\mu \quad (0,0);\qquad \part X^\mu\quad (1,0);\qquad \bar \part X^\mu\quad (0,1);\qquad :e^{ikX}:\quad (\alpha'k^2/4, \alpha'k^2/4)
$$
For any pair of operators, applying rigid translations, scale transformations, and rotations to both sides of the OPE determines the $z$-dependence of the coefficient functions completely,
$$
\mathscr A_i(z_1, \bar z_1) \mathscr A_j(z_2,\bar z_2) = \sum_k z_{12}^{h_k-h_i-h_j}\bar z_{12}^{\bar h_k - \bar h_i - \bar h_j} c^k_{~ij} \mathscr A_k(z_2, \bar z_2)
$$

### Conformal properties of the energy-momentum tensor

The OPE of the energy-momentum tensor with itself was obtained by
$$
T(z) T(0) \sim \frac{D}{2 z^4} + \frac{2}{z^2} T(0) + \frac 1 z \part T(0)
$$
This OPE combined with the Ward identity, gives the transformation law
$$
\epsilon^{-1} \delta T(z) = -\frac{D}{12}\part^3 v(z)- 2\part v(z) T(z) - v(z) \part T(z)
$$
In a general CFT, $T(z)$ transforms as
$$
\epsilon^{-1} \delta T(z) = -\frac{c}{12}\part^3 v(z)- 2\part v(z) T(z) - v(z) \part T(z)~,
$$
with $c$ a constant known as the **central charge**. The central charge of a free scalar is $1$, for $D$ free scalars it is $D$.

The finite form of the transformation law is
$$
(\part z')^2 T'(z') = T(z) - \frac{c}{12}\{z',z\}~,
$$
where $\{f,z\}$ denoted the **Schwarzian derivative**
$$
\{f,z\} = \frac{2\part^3_z f \part_z f- 3\part_z^2 f\part^2_z f}{2\part_z f \part_zf}
$$

## Free CFTs

We will introduce three families of free-field CFTs, the linear dilaton, $bc$, and $\beta \gamma$ theories.

### Linear dilaton CFT

The energy-momentum tensor is given by
$$
T(z) = -\frac{1}{\alpha'} :\part X^\mu \part X_\mu: + V_\mu \part^2 X^\mu~,\\
\bar T(\bar z)= -\frac{1}{\alpha'} :\bar\part X^\mu \bar\part X_\mu: + V_\mu \bar\part^2 X^\mu~,
$$
where $V_\mu$ is some fixed $D$-vector. Working out the $TT$ OPE, one finds that it is of the form
$$
T(z)T(0) \sim \frac{c}{2z^4} + \frac{2}{z^2} T(0) + \frac 1z \part T(0)~,
$$
but with $c = D + 6\alpha' V^\mu V_\mu$.

The $T X^\mu$ OPE gives
$$
T(z) X^\mu(0) \sim \frac{\alpha' V^\mu}{2 z^2} + \frac{\part X^\mu}{z}
$$
and the Ward identity gives the transformation law of $X^\mu$
$$
\delta X^\mu = - \epsilon v \part X^\mu - \epsilon v^* \bar \part X^\mu - \frac{\epsilon}{2}\alpha' V^\mu [\part v + (\part v)^*]~.
$$
Different values of $V^\mu$ are to be regarded as different CFTs. The vector $V^\mu$ picks out a direction in spacetime. This CFT is therefore not Lorentz-invariant and not of immediate interest to us.

### $bc$ CFT

The second family of CFTs has **anticommuting** fields $b$ and $c$ with action
$$
S = \frac{1}{2\pi} \int d^2z b \bar \part c~.
$$
This is conformally invariant for $b$ and $c$ transforming as tensors of weights $(h_b, 0)$ and $(h_c,0)$ such that
$$
h_b = \lambda,\quad h_c = 1-\lambda~,
$$
for any given constant $\lambda$. This is secretly the same as the linear dilaton family as we will see later.

The operator equations of motion are
$$
\bar \part c(z) = \bar \part b(z) = 0,\quad \bar \part b(z) c(0) = 2\pi \delta^2(z, \bar z)~.
$$
The $bb$ and $cc$ OPE satisfy the equation of motion withou source. The normal ordered $bc$ product is
$$
:b(z_1) c(z_2): = b(z_1) c(z_2) - \frac{1}{z_{12}}~.
$$
This is because
$$
\bar \part \frac 1 z= \part\frac{1}{\bar z} = 2\pi \delta^2(z,\bar z).
$$
The operator products are
$$
b(z_1) c(z_2) \sim \frac{1}{z_{12}},\quad c(z_1) b(z_2) \sim \frac{1}{z_{12}}~.
$$
Noether's theorem gives the energy-momentum tensor
$$
T(z) = :(\part b)c: - \lambda \part(:bc:),\quad \overline T(\bar z)  = 0.
$$
The $TT$ OPE is
$$
T(z)T(0) \sim \frac{c}{2z^4} + \frac{2}{z^2} T(0) + \frac 1z \part T(0)~,
$$
with $c = -3(2\lambda-1)^2 + 1$. Moreover, $\bar c = 0$. This is a purely holomorphic CFT, and is an example where $c \neq \bar c$. There is of course a corresponding antiholomorphic theory
$$
S = \frac{1}{2\pi} \int d^z \bar b \part \bar c~.
$$
The $bc$ theory has a **ghost number** symmetry $\delta b = -i\epsilon b, \delta c = i \epsilon c$.