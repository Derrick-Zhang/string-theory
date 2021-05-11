## Problem 1

Write $\Lambda$ as
$$
\Lambda = \begin{pmatrix} A & B\\ C & D \end{pmatrix}, \quad 
\Lambda^T = \begin{pmatrix} A^T & C^T\\ B^T & D^T\end{pmatrix}~,
$$
where $A, B, C, D$ are $k\times k$ matrices.

- From $P \Lambda^T P = \Lambda$, we can obtain
  $$
  A = D^T, \quad B = -B^T, \quad C = -C^T~.
  $$
  The degree of freedom is
  $$
  k^2 + \frac{k(k-1)}{2} + \frac{k(k-1)}{2} = 2k^2 -k = \frac12 n(n-1)~.
  $$

- From $P \Lambda^T P = - \Lambda$, we can obtain
  $$
  A = - D^T, \quad B = B^T, \quad C = C^T~.
  $$
  The degree of freedom is
  $$
  k^2 + \frac{k(k+1)}{2} + \frac{k(k+1)}{2} = 2k^2 + k = \frac12 n(n+1)~.
  $$

---

We have
$$
\Omega_\Lambda = P \Lambda^T P \Lambda^{-1} = \begin{cases}+1, & P\Lambda^TP = \Lambda \\
-1, & P \Lambda^T P = - \Lambda\end{cases}~.
$$
 Therefore,
$$
{\rm tr}[\Omega_\Lambda] = \frac 12 n(n-1) - \frac12 n(n+1) = -n~.
$$

## Problem 2

In the NS sector
$$
\Omega: \psi^\mu(t, \sigma) \to - \bar \psi^\mu(t, 2\pi - \sigma),\quad \bar \psi^\mu(t, \sigma) \to - \psi^\mu(t, 2\pi - \sigma)~.
$$
In the R sector
$$
\Omega: \psi^\mu(t, \sigma) \to \bar \psi^\mu(t, 2\pi - \sigma), \quad \bar\psi(t, \sigma) \to \psi^\mu(t, 2\pi - \sigma)~.
$$
Define the action of the orientation operator on the fermions $\psi^\mu(t, \sigma)$, $\bar \psi^\mu (t, \sigma)$ in NS-sector and R-sector respectively, and derive the action on their modes

---

Show that only the 2-form IIB RR-field survives under the $\Omega$ projection $(1+ \Omega)/2$

## Problem 3

## Problem 4

