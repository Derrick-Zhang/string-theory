## Problem 1

The stress-energy tensor for massless scalar field is give by
$$
T(z) = -\frac{1}{\alpha'} :\part X \part X:~, \quad \overline T(\bar z) = -\frac{1}{\alpha'} :\bar \part X \bar \part X:~.
$$
Therefore,
$$
\begin{align}
T(z) :e^{ikX(0)}:~ =&~ -\frac{1}{\alpha'} \sum_{m = 0}^\infty \frac{(ik)^m}{m!} :\part X \part X(z):~:(X(0))^m:\\
\sim&~-\frac{2}{\alpha'} \sum_{m=1}^\infty (ik) \frac{(ik)^{m-1}}{(m-1)!} :\part X(z)(X(0))^{m-1}: \left(-\frac{\alpha'}{2} \frac 1z\right)\\
&-\frac{1}{\alpha'}\sum_{m=2}^\infty(ik)^2 \frac{(ik)^{m-2}}{(m-2)!} :(X(0))^{m-2}:\left(\frac{\alpha'^2}{4 z^2}\right)\\
\sim&~\frac{\alpha' k^2}{4 z^2} :e^{ikX(0)}: + \frac{1}{z}:\part e^{ik X(0)}:
\end{align}
$$
Similarly, 
$$
\overline T(\bar z):e^{ikX(\bar 0)}:~ \sim \frac{\alpha' k^2}{4 \bar z^2} :e^{ikX(\bar 0)}: + \frac{1}{\bar z} :\bar \part e^{ikX(\bar0)}:
$$
Therefore, $:e^{ikX}:$ is a primary field with wieght $h = \bar h = \alpha' k^2/4$.

For $\part^n X$ with $n\ge 2$, the contraction between $\part X(z)$ in $T(z)$ and $\part^n X(w)$ would give a non-vanishing term
$$
- \frac{\alpha'}{2} \part_z \part^n_w \ln(z-w) \propto \frac{1}{(z-w)^{n+1}}, \quad n\ge 2
$$
Therefore, $\part^n X$ with $n \ge 2$ is not a primary.

## Problem 2

The OPE of the stress-energy tensor is 
$$
T(z)T(w) \sim \frac{c/2}{(z-w)^4} + \frac{2 T(w)}{(z-w)^2}+\frac{\part T(w)}{z-w}~.
$$
The mode expanson of the stress-energy tensor is given by
$$
T(z) = \sum_{n \in \mathbb Z} L_n z^{-n-2}~.
$$
Conversely, we can get the Laurent coefficient by
$$
L_m = \int \frac{dz}{2\pi i z} z^{m+2} T(z).
$$
Therefore, one can derive the Virasoro algebra
$$
\begin{align}
[L_m, L_n] &= \int \frac{dz}{2\pi i }\int \frac{dw}{2\pi i} z^{m+1} w^{n+1} \,[T(z), T(w)]\\
					 &= \int \frac{dw}{2\pi i} w^{n+1} \int_w \frac{dz}{2\pi i} z^{m+1} T(z)T(w)\\
					 & = \int \frac{dw}{2\pi i }w^{n+1}\left(\frac{1}{3!}(m+1)m(m-1)w^{m-2}\frac c 2+ 2(m+1) w^m T(w) + w^{m+1} \part T(w)\right)\\
					 & = \frac{c}{12}(m+1)m(m-1)\delta_{m+n,0} + 2(m+1)L_{m+n} - (m+n+2) L_{m+n}\\
					 & = \frac{c}{12}m(m^2-1)\delta_{m+n,0} + (m-n)L_{m+n}~,
\end{align}
$$
where in the next to the last step, we integrate by parts over the last term.

## Problem 3

A general infinitesimal hollomorphic map can be expressed as
$$
z' = z - \epsilon(z) = z- \sum_{n \in \mathbb Z}\epsilon_n z^{n+1}~,
$$
Generators of the transformation are
$$
\ell_n = -z^{n+1} \part_z~.
$$
Therefore,
$$
\begin{align}
[\ell_m, \ell_n]&= z^{m+1}\part(z^{n+1}\part)- z^{n+1}\part(z^{m+1} \part)\\
&=(n+1) z^{m+n+1}\part + z^{m+n+2}\part \part - (m+1)z^{m+n+1}\part - z^{m+n+2}\part\part\\
&=-(m-n)z^{m+n+1}\part = (m-n)\ell_{m+n}~.
\end{align}
$$

## Problem 4

We have
$$
\frac{a z_1 + b}{c z_1 + d} = 0, \quad \frac{a z_2 + b}{c z_2 + d} = 1, \quad \frac{a z_3 + b}{c z_3 + d} = \infty, \quad ad - bc = 1
$$
From the first equation we know that $b = -a z_1$, from the third we know that $d= -c z_3$. Plug these into the second and fouth equations, we are left with
$$
\frac{a}{c} \frac{z_2 - z_1}{z_2 - z_3} = 1, \quad ac(z_1 - z_3) = 1.
$$
Therefore
$$
a = \left (\frac{z_2 - z_3}{z_2 - z_1} \frac{1}{z_1-z_3}\right)^{\frac12},\quad c=\left (\frac{z_2 - z_1}{z_2 - z_3} \frac{1}{z_1-z_3}\right)^{\frac12}, \quad b = -z_1\left (\frac{z_2 - z_3}{z_2 - z_1} \frac{1}{z_1-z_3}\right)^{\frac12}, \quad d = -z_3\left (\frac{z_2 - z_1}{z_2 - z_3} \frac{1}{z_1-z_3}\right)^{\frac12}
$$

---

The cross-ration is defined by
$$
[z_1, z_2, z_3, z_4] = \frac{(z_1 - z_3)(z_2 - z_4)}{(z_2- z_3)(z_1 - z_4)}~.
$$
If $w_i = (a z_i +b)/(c z_i +d)$ with $ad-bc=1$, then
$$
\begin{align}
[w_1, w_2, w_3, w_4] =&~ \frac{(w_1 - w_3)(w_2 - w_4)}{(w_2 - w_3)(w_1 - w_4)} = \frac{(az_1 + b)(c z_3 + d) - (a z_3 + b)(c z_1 +d)}{(a z_2 +b)(c z_3 + d)- (a z_3 + b)(c z_2 +d)}\\
&\times\frac{(a z_2 +b)(c z_4 + d)-(az_4 +b)(c z_2 +d)}{(az_1 +b)(c z_4 +d)- (a z_4 + b)(c z_1 +d)}\\
=&~\frac{z_1 - z_3}{z_2 -z_3} \frac{z_2 - z_4}{z_1 -z_4} = [z_1, z_2, z_3, z_4].
\end{align}
$$
Therefore the cross ratio is invariant under any linear fractional transformation.