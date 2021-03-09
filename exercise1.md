## Problem 1

The mode expansion for bosonic closed string is
$$
X^\mu = x^\mu + \alpha' p^\mu \tau + i\sqrt{\alpha'/2} \sum_{n\neq 0}\{\frac1n \alpha^\mu_n \exp\left[-in(\tau-\sigma)\right]+\frac1n\tilde \alpha^\mu_n\exp[-in(\tau + \sigma)]\}~.
$$
Then
$$
\part_\tau X^\mu = \alpha' p^\mu +\sqrt{\alpha'/2} \sum_{n\neq 0}\{\alpha^\mu_n \exp\left[-in(\tau-\sigma)\right]+\tilde \alpha^\mu_n\exp[-in(\tau + \sigma)]\}~.
$$
The center-of-mass position and momenta are given by
$$
\begin{align}
x^\mu = \frac{1}{2\pi}\int_0^{2\pi} d\sigma X^\mu, \quad p_\mu = \int_0^{2\pi} d\sigma \,\Pi_\mu~.
\end{align}
$$
Therefore, when $\tau$ is fixed
$$
\begin{align}
[x^\mu, p_\nu] = \frac{1}{2\pi} \int_0^{2\pi}d\sigma \int_0^{2\pi} d\sigma' \,[X^\mu(\sigma), \Pi_\nu(\sigma')] = \frac{1}{2\pi} \int_0^{2\pi}d\sigma \int_0^{2\pi} d\sigma' \, i\delta(\sigma-\sigma') \delta^\mu_{~\nu} = i \delta^\mu_{~\nu}~.
\end{align}
$$
Now we would like to solve $\alpha_m^\mu$ and $\tilde \alpha^\mu_m$ ($m\neq0$) in terms of $X^\mu$ and $\partial_\tau X^\mu$ . Note that
$$
\begin{align}
\frac{1}{2\pi} \int_0^{2\pi} d\sigma\, X^\mu e^{im\sigma} &= i\sqrt{\alpha'/2}\frac1m\left(- \alpha^\mu_{-m} e^{im\tau} + \tilde \alpha_m^\mu e^{-im\tau}\right)~,\\
\frac{1}{2\pi} \int_0^{2\pi} d\sigma\, \part_\tau X^\mu e^{im\sigma} &= \sqrt{\alpha'/2}(\alpha_{-m}^\mu e^{im\tau} + \tilde\alpha_m^\mu e^{-im\tau})~.
\end{align}
$$
Therefore
$$
\begin{align}
\alpha_m^\mu = \sqrt{\alpha'/2} \int_0^{2\pi} d\sigma \,\left(\Pi^\mu - \frac{im}{2\alpha'\pi}X^\mu\right) e^{im(\tau - \sigma)}~,\\
\tilde\alpha_m^\mu = \sqrt{\alpha'/2} \int_0^{2\pi} d\sigma \,\left(\Pi^\mu - \frac{im}{2\alpha'\pi}X^\mu\right) e^{im(\tau + \sigma)}~.\\
\end{align}
$$
The commutation relations are
$$
\begin{align}
[\alpha^\mu_n, \alpha^\nu_m]&= \alpha'/2\int_{0}^{2\pi}d\sigma \int_{0}^{2\pi} d\sigma' e^{in(\tau - \sigma) +im(\tau-\sigma')} \left\{-\frac{im}{2\alpha'\pi}[\Pi^\mu(\sigma), X^\nu(\sigma')]-\frac{in}{2\alpha'\pi}[X^\mu(\sigma), \Pi^\nu(\sigma')]\right\}\\
&=\alpha'/2 \int_{0}^{2\pi}d\sigma \int_{0}^{2\pi} d\sigma' e^{in(\tau - \sigma) +im(\tau-\sigma')}
\left\{-\frac{m}{2\alpha'\pi}\eta^{\mu \nu}\delta(\sigma-\sigma')+\frac{n}{2\alpha'\pi}\eta^{\mu \nu}\delta(\sigma-\sigma')\right\}\\
&=\alpha'/2\int_0^{2\pi} d\sigma e^{i(m+n)(\tau-\sigma)} \eta^{\mu \nu} \frac{1}{2\pi \alpha'} (n-m) = \frac12 e^{i(m+n)\tau}\eta^{\mu \nu} (n-m)\delta_{m,-n} = n\eta^{\mu \nu} \delta_{m,-n}~.
\end{align}
$$
Similarly,
$$
[\tilde \alpha^\mu_n, \tilde\alpha_m^\mu] = n \eta^{\mu \nu} \delta_{m,-n}~.
$$

## Problem 2

We will conisder open string with length $\ell = 2\pi$. The equation of motion is
$$
\part^2_\tau X^\mu = \part^2_\sigma X^\mu~.
$$

- For $i=0,\cdots,24$, conisdering Neumann boundary condition
  $$
  \partial^\sigma X^i(\tau,\sigma) = 0 ~{\rm at} ~\sigma=0, 2\pi~.
  $$

​	The solution is 
$$
X^i(\tau, \sigma) = x^i + p^i\alpha'\tau+ i\sqrt{2\alpha'} \sum_{n\neq 0} \frac{1}{n} \alpha_n^i \exp\left(-i n \tau/2\right) \cos\left(n \sigma/2\right)~.
$$

- For $i=25$, if both ends satisfy Dirichlet boundary conditions
  $$
  X^i(\tau,0) = X_0, \quad X^i(\tau, 2\pi) = X_{2\pi}~.
  $$
  Intepretation: both ends of the open string are fixed in certain one direction which breaks the Poincaré invariance.

  We can solve that
  $$
  X^i(\tau, \sigma) = X_0+\frac{X_{2\pi}-X_0}{2\pi} \sigma+ \sqrt{2\alpha'}\sum_{n\neq 0} \frac1n \alpha_n^i \exp(-in\tau/2)\sin(n\sigma/2)~.
  $$
  Then, the conjugate momentum
  $$
  p_i = \frac{\part L}{\part(\part_\tau X^i)} = \frac{1}{2\pi \alpha'}\part_\tau X^i = \frac{-i}{2\pi \sqrt{2\alpha'}} \sum_{n\neq0} \alpha^i_n \exp(-in\tau/2)\sin(n\sigma/2)~.
  $$
  And the momentum is not conserved.

- For $i = 25$, if one end satisfies Dirichlet boundary condition and the other satisfies Neumann boundary condition
  $$
  X^i(\tau,0) = X_0, \quad \part_\sigma X^i(\tau, 2\pi) = 0.
  $$
  One end of the open string is fixed in this direction, and one end is perpendicular to the boundary $\sigma = 2\pi$.

  The solution is
  $$
  X^i(\tau, \sigma) = X_0 + \sqrt{2\alpha'}\sum_{n\neq 0} \frac{1}{n+1/2} \alpha_n^i \exp(-i(n+1/2)\tau/2)\sin((n+1/2)\sigma/2)~.
  $$

## Problem 3

The mode expansion for open string is
$$
X^\mu = x^\mu + 2\alpha'p^\mu \tau + i\sqrt{\alpha'/2}\sum_{n\neq0} \frac1n\left(\tilde \alpha^\mu_n e^{-in(\tau + \sigma)}+ \alpha_n^\mu e^{-in(\tau -\sigma)}\right)~.
$$
Then 
$$
\part_\sigma X^\mu = i\sqrt{\alpha'/2}\sum_{n\neq0} \left(-i\tilde \alpha^\mu_n e^{-in(\tau + \sigma)}+ i\alpha_n^\mu e^{-in(\tau -\sigma)}\right)~,
$$
and
$$
\part_\sigma X^\mu\big|_{\sigma = 0} = \sqrt{\alpha'/2}\sum_{n\neq0} e^{-in\tau }\left(\tilde \alpha^\mu_n - \alpha_n^\mu \right)=0~,
$$
Therefore, for Neumann boundary conditions,
$$
\tilde \alpha^\mu_n = \alpha^\mu_n~.
$$
On the other hand
$$
\begin{align}
X^\mu\big|_{\sigma = 0} &= x^\mu + 2\alpha'p^\mu \tau + i\sqrt{\alpha'/2}\sum_{n\neq 0} \frac1n\left(\tilde \alpha_n^\mu + \alpha_n^\mu\right) e^{-in\tau} = c^\mu~,\\
X^\mu\big|_{\sigma = \pi} &= x^\mu + 2\alpha'p^\mu \tau + i\sqrt{\alpha'/2}\sum_{n\neq 0} \frac1n\left(\tilde \alpha_n^\mu  + \alpha_n^\mu  \right)e^{-in\tau}(-1)^n  = c^\mu~,
\end{align}
$$
holds for arbitrary $\tau$. Therefore,
$$
x^\mu = c^\mu, \quad p^\mu = 0, \quad \alpha_n = -\tilde \alpha_n~.
$$


