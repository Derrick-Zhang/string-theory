## Problem 1

### Problem 1.1

The two-form field strength
$$
F_2 = \frac12 F_{\mu \nu}\, dx^\mu \wedge dx^\nu~.
$$
Its Hodge dual is
$$
* F_2 = \frac{\sqrt{|G|}}{2!(D-2)!} {\epsilon_{\mu_1\cdots\mu_{D-2}}}^{\mu_{D-1}\mu_D} F_{\mu_{D-1}\mu_D}\, dx^{\mu_1} \wedge \cdots \wedge dx^{\mu_{D-2}}~.
$$
Their Wedge product is then
$$
\begin{align}
F_2 \wedge * F_2 &= \frac{\sqrt{|G|}}{4} \frac{1}{(D-2)!}{\epsilon_{\mu_1\cdots\mu_{D-2}}}^{\mu_{D-1}\mu_D} F_{\mu_{D-1}\mu_D}F_{\mu \nu}\, dx^\mu \wedge dx^\nu \wedge dx^{\mu_1} \wedge \cdots \wedge dx^{\mu_{D-2}}\\
& = \frac{\sqrt{|G|}}{4} \frac{1}{(D-2)!}\epsilon_{\mu_1\cdots\mu_D} F^{\mu_{D-1}\mu_D}F_{\mu \nu}\, \epsilon^{\mu \nu \mu_1 \cdots \mu_{D-2}} d^Dx
\end{align}
$$
The contraction of two totally antisymmetric tensor is
$$
\epsilon_{\mu_1 \cdots \mu_{D-2}\mu_{D-1}\mu_D}\cdot  \epsilon^{ \mu \nu\mu_1 \cdots \mu_{D-2}} = (D-2)! (\delta^\mu_{\mu_{D-1}} \delta^\nu_{\mu_{D}} - \delta^\mu_{\mu_{D}}\delta^\nu_{\mu_{D-1}})
$$
Therefore,
$$
F_2 \wedge * F_2 = \frac{\sqrt{|G|}}{4} (\delta^\mu_{\mu_{D-1}} \delta^\nu_{\mu_D} - \delta^\mu_{\mu_D} \delta^\nu_{\mu_{D-1}}) F^{\mu_{D-1}\mu_D} F_{\mu\nu}\,  d^D x= \frac{\sqrt{|G|}}{2} F^{\mu \nu}F_{\mu \nu}\,d^Dx~.
$$
So
$$
\frac{1}{2g^2} \int F_2^2 \equiv \frac{1}{2g^2} \int F_2 \wedge * F_2 = \frac{1}{4 g^2} \int \sqrt{|G|}\, d^D x\, F_{\mu \nu } F^{\mu \nu}~. 
$$

 ### Problem 1.2

Consider only the variation of $f_{D-n-1}$, then the variation of the action
$$
0 = \delta S = - \int \delta f_{D-n -1} \wedge (F_{n+1} - dA_n)~,
$$
for arbitrary $\delta f_{D-n-1}$. Therefore, the equation of motion is
$$
F_{n+1}  = d A_n~.
$$
Then $F_{n+1}$ is the curvature and $S$ is the kinetic term action.

---

Consider only the variation of $F_{n+1}$, then the variation of the action
$$
\begin{align}
0 &= \delta S = - \frac{1}{2g^2} \int \delta F_{n+1} \wedge * F_{n+1}- \frac{1}{2g^2} \int F_{n+1} \wedge * \delta F_{n+1} - \int f_{D-n-1} \wedge \delta F_{n+1} \cr
& = -\frac{1}{g^2} \int \delta F_{n+1} \wedge * F_{n+1} - (-1)^{(n+1)(D-n-1)} \int \delta F_{n+1} \wedge f_{D-n-1}~,
\end{align}
$$
where we have used $\omega \wedge * \eta = \eta \wedge * \omega$. Then the equation of motion is
$$
f_{D-n-1} = (-1)^{(n+1)(D-n-1)} \left(-\frac{1}{g^2} * F_{n+1}\right)
$$
Therefore, the action is
$$
\begin{align}
S &= - \frac{1}{2g^2} \int F_{n+1} \wedge *F_{n+1} + \frac{1}{g^2} \int (F_{n+1} - d A_n) \wedge * F_{n+1}\\
&= \frac{1}{2g^2} \int F_{n+1} \wedge * F_{n+1} - \frac{1}{g^2} \int d A_n \wedge * F_{n+1}
\end{align}
$$

---

Consider the variation of $A_n$,
$$
\delta S = - \frac{1}{g^2} \int (d \delta A_n) \wedge * F_{n+1} = \frac{1}{g^2} \int (-1)^n \delta A_n \wedge d* F_{n+1}~,
$$
where we have used
$$
d(\delta A_n \wedge * F_{n+1}) = (d \delta A_n) \wedge * F_{n+1} + (-1)^n \delta A_n \wedge d * F_{n+1}
$$
so
$$
(d \delta A_n) \wedge * F_{n+1}=d(\delta A_n \wedge * F_{n+1}) - (-1)^n \delta A_n \wedge d * F_{n+1}
$$
and we dropped the total derivative. The equation of motion is
$$
d * F_{n+1} = 0~.
$$


## Problem 2

### Problem 2.1

$$
\nabla \cdot {\bf B} = q_m \delta^3({\bf r}).
$$

Recall $\nabla \cdot {\bf r}/r^3 = 4\pi \delta^3({\bf r})$, we can get the solution
$$
{\bf B} = \frac{q_m}{4\pi} \frac{\bf r}{r^3}.
$$
It is defined on $\mathbb R^3 - \{0\}$, which is homotopic to $S^2$. Therefore, $\bf B$ cannot be expressed by space components of a gauge field $\bf A$ globally. 

---

Consider
$$
{\bf A}^N = \frac{q_m (1- \cos \theta)}{4 \pi r \sin \theta} {\bf e}_\phi, \quad {\bf A}^S = - \frac{q_m (1 + \cos \theta)}{4\pi r \sin \theta}{\bf e}_\phi~.
$$
In the polar coordinate, we have
$$
\nabla f = \frac{\partial f}{\partial r} {\bf e}_r + \frac1 r \frac{\partial f}{\partial \theta} {\bf e}_\theta + \frac{1}{r \sin \theta} \frac{\partial f}{\partial \phi} {\bf e}_\phi.
$$
Therefore
$$
{\bf A}^N - {\bf A}^S = \frac{q_m}{2\pi r \sin \theta} {\bf e}_\phi = \nabla\left(\frac{q_m \phi}{2\pi}\right),
$$
and they are related by a gauge transformation.

---

$$
\begin{align}
\nabla \times {\bf A}^N &= \frac{1}{r \sin \theta} \frac{\partial}{\partial \theta} \left(\sin \theta\cdot \frac{q_m (1- \cos \theta)}{4\pi r \sin \theta}\right){\bf e}_r - \frac 1r \frac{\partial }{\partial r} \left(r \cdot \frac{q_m (1- \cos \theta)}{4\pi r \sin \theta}\right){\bf e}_\theta\\
&=\frac{q_m }{4\pi r^2} {\bf e}_r = \frac{q_m }{4\pi} \frac{\bf r}{r^3} = {\bf B}~.
\end{align}
$$

Similarly,
$$
\begin{align}
\nabla \times {\bf A}^S &= \frac{1}{r \sin \theta} \frac{\partial}{\partial \theta} \left(\sin \theta\cdot \frac{-q_m (1+ \cos \theta)}{4\pi r \sin \theta}\right){\bf e}_r - \frac 1r \frac{\partial }{\partial r} \left(r \cdot \frac{-q_m (1+ \cos \theta)}{4\pi r \sin \theta}\right){\bf e}_\theta\\
&=\frac{q_m }{4\pi r^2} {\bf e}_r = \frac{q_m }{4\pi} \frac{\bf r}{r^3} = {\bf B}~.
\end{align}
$$

---

The total magnetic flux is
$$
\Phi = \int_{S^2} \nabla \times {\bf A} \cdot d{\bf S} = \int_{U_N} \nabla \times {\bf A}^N \cdot d {\bf S} + \int_{N_S} \nabla \times {\bf A}^S \cdot d{\bf S}~,
$$
where $U_N$ is the northern hemisphere and $U_S$ is the southern hemisphere. Their boundary is the equator $S^1$. Using the Stokes theorem,
$$
\begin{align}
\Phi &= \int_{S^1} {\bf A}^N \cdot d{\bf l} - \int_{S^1} {\bf A}^S \cdot d{\bf l}
\\&= \int_{S^1}  \nabla\left(\frac{q_m \phi}{2\pi}\right) \cdot d{\bf l} = q_m~.
\end{align}
$$

---

$$
d F_2 = q_m \delta_3({\bf r}), \quad \delta_3({\bf r}) = \delta(x)\delta(y)\delta(z) dx \wedge dy \wedge dz
$$

$$
d F_2 = d\left(\frac12 F_{\mu \nu} \,dx^\mu \wedge dx^\nu\right) = \frac 12 \partial_\rho F_{\mu \nu} \, dx^\rho \wedge dx^\mu \wedge dx^\nu
$$

Therefore, we have
$$
\frac12 (\partial_1 F_{23} - \partial_1 F_{32} + \partial_2 F_{31} - \partial_2 F_{13} + \partial_3 F_{12} - \partial_3 F_{21}) = q_m\delta(x) \delta(y) \delta(z)
$$
Since
$$
F_{\mu \nu} = \begin{pmatrix}0 & E_1 & E_2 & E_3 \\
-E_1 & 0 & -B_3 & B_2 \\
-E_2 & B_3 & 0 & -B_1\\
-E_3 & -B_2 & B_1 & 0\end{pmatrix}
$$
Therefore, we get
$$
- \nabla \cdot {\bf B} = q_m \delta^3({\bf r})
$$

---

$$
\begin{align}
A_N &= {\bf A}^N \cdot d{\bf l}=  \frac{q_m (1- \cos \theta)}{4 \pi r \sin \theta} r \sin \theta d\phi = \frac{q_m}{4 \pi }(1- \cos \theta) d\phi~, 
\\ A_S &= {\bf A}^S \cdot d{\bf l} = - \frac{q_m (1 + \cos \theta)}{4\pi r \sin \theta} r\sin \theta d\phi = - \frac{q_m}{4\pi} (1+ \cos \theta) d\phi~.
\end{align}
$$

$$
A_N - A_S = \frac{q_m}{2\pi} d\phi~.
$$

$$
\Phi = \int_{S^1} (A_N - A_S) = \int_{S^1} \frac{q_m}{2\pi} d\phi = q_m~.
$$

### Problem 2.2

$\kappa$ is the gravitational coupling constant. Using Stokes theorem, it is easy to calculate
$$
\int_{S^{p+2}} G_{p+2} = \int_{D^{p+3}} d G_{p+2} = 2\kappa^2 q_m\int_{D^{p+3}} \delta_{p+3}(M_{D-p-3}) = 2 \kappa^2 q_m~.
$$
Consider an object that is electrically coupled to $C_{p+1}$,
$$
S_E = q_e \int_{E_{p+1}} C_{p+1} = q_e \int_{\widehat E_{p+2}} G_{p+2} \equiv S_E(\delta\widehat E_{p+2})~.
$$
Consider a deformation of $\widehat E_{p+2}$, 
$$
\delta \widehat E_{p+2} = \widehat E_{p+2}^N - \widehat E^S_{p+2}~.
$$
From $e^{iS_E(\delta \widehat E_{p+2})} = 1$, we have
$$
q_e \int_{\widehat E_{p+2}^N} G_{p+2} - q_e \int_{\widehat E^S_{p+2}} G_{p+2} = 2\kappa^2 q_m q_3 \in 2\pi \mathbb Z~.
$$

## Problem 3

The action is given by
$$
S = \frac{1}{2\kappa^2} \int d^{10}x \sqrt{-G_E} \left[R_E - \frac{\nabla_\mu \tau \nabla^\mu \bar \tau}{2({\rm Im} \,\tau)^2} - \frac 12 {\mathbb F}^T_{(3)} \cdot \mathbb M \cdot \mathbb F_{(3)} - \frac14 \widetilde G^2_{(5)}\right] - \frac{1}{4\kappa^2} \int C_{(4)} \wedge \mathbb F_{(3)}^T \wedge \epsilon \,\mathbb F_{(3)}~.
$$
The $SL(2, \mathbb R)$ transformation is given by
$$
\tau \to \frac{a\tau + b}{c \tau + d},\quad \mathbb M \to (\Lambda^{-1})^T \mathbb M \Lambda^{-1}, \quad \mathbb F_{(3)} \to \Lambda \mathbb F_{(3)}, \quad \Lambda = \begin{pmatrix}d & c\\ b & a\end{pmatrix} \in SL(2, \mathbb R)~.
$$
Then
$$
\mathbb F_{(3)}^T \cdot \mathbb M\cdot \mathbb F_{(3)} \to \mathbb F_{(3)}^T \Lambda^T (\Lambda^{-1})^T\mathbb M \Lambda^{-1} \Lambda \mathbb F_{(3)} = \mathbb F_{(3)}^T \cdot \mathbb M\cdot \mathbb F_{(3)}~.
$$
Since
$$
\Lambda^T \epsilon \Lambda = \begin{pmatrix}d & b\\ c & a\end{pmatrix}\begin{pmatrix}0 & 1\\ -1 & 0\end{pmatrix}\begin{pmatrix}d & c\\ b & a\end{pmatrix} = \begin{pmatrix}0 & 1\\ -1 & 0\end{pmatrix} = \epsilon~,
$$
we can obtain
$$
C_{(4)} \wedge \mathbb F_{(3)}^T \wedge \epsilon \, \mathbb F_{(3)} \to C_{(4)} \wedge \mathbb F_{(3)}^T \wedge (\Lambda^T \epsilon\, \Lambda)\mathbb F_{(3)}= C_{(4)} \wedge \mathbb F_{(3)}^T \wedge \epsilon \, \mathbb F_{(3)}~.
$$
Last, consider $\frac{\nabla_\mu \tau \nabla^\mu \bar \tau}{2 (\rm Im\, \tau)^2}$, the numerator transforms as
$$
\nabla_\mu \tau \nabla^\mu \bar \tau \to \nabla_\mu \left(\frac{a\tau + b}{c \tau + d}\right) \nabla^\mu \left(\frac{a \bar \tau + b}{c \bar \tau + d}\right) = \frac{1}{(c \tau + d)^2 (c \bar \tau + d)^2} \nabla_\mu \tau \nabla^\mu \bar \tau~.
$$
The numerator $2 ({\rm Im \, \tau})^2 = - \frac 12 (\tau - \bar \tau)^2$,
$$
-\frac 12 (\tau - \bar \tau)^2 \to - \frac 12 \left(\frac{a \tau + b}{c \tau + d} - \frac{a \bar \tau + b}{c \bar \tau + d}\right)^2 = -\frac 12 \frac{1}{(c\tau + d)^2 (c \bar \tau + d)^2} \left((a\tau + b)(c \bar \tau + d) - (a \bar \tau + b)(c \tau + d)\right)^2\\
= - \frac 12 \frac{1}{(c\tau + d)^2 (c \bar \tau + d)^2}(\tau - \bar \tau )^2~.
$$
Therefore, this term is also $SL(2, \mathbb R)$ invariant. So type IIB SUGRA is $SL(2, \mathbb R)$ invariant.

## Problem 4

The metric is 
$$
ds^2 = G_{MN} dx^M dx^N = g_{\mu \nu} dx^\mu dx^\nu + e^{2\sigma} (dy + A_\mu dx^\mu)^2~.
$$
We have, for $\mu, \nu$ run from $0$ to $D-1$,
$$
G_{\mu \nu} = g_{\mu \nu} + e^{2\sigma} A_\mu A_\nu~.
$$
Also,
$$
G_{\mu D} = G_{D \mu} = e^{2\sigma} A_\mu, \quad G_{DD} = e^{2\sigma}~.
$$
We have
$$
G_{MN} = \begin{pmatrix}g_{\mu \nu} + e^{2\sigma} A_\mu A_\nu & e^{2\sigma } A_\mu\\
e^{2\sigma} A_\nu& e^{2\sigma}\end{pmatrix}, \quad G^{MN} = \begin{pmatrix}g^{\mu \nu} & -A^\mu \\ -A^\nu & A^2 + e^{-2\sigma}\end{pmatrix}~.
$$
Therefore, we can rewrite the action
$$
\mathcal L^{(D+1)} = - \frac 12 G^{MN} \partial_M \phi \partial _N \phi = -\frac12 G^{\mu \nu } \partial_\mu \phi \partial_\nu \phi - G^{\mu D} \partial_\mu \phi \frac{\partial\phi}{\partial y}-\frac 12 G^{DD} \left(\frac{\partial \phi}{\partial y}\right)^2\\
= - \frac 12 g^{\mu \nu} \partial_\mu \phi\partial_\nu \phi+ A^\mu \partial_\mu \phi \frac{\partial \phi}{\partial y} - \frac12 (A^2 + e^{-2\sigma}) \left(\frac{\partial \phi}{\partial y}\right)^2~.
$$

---

The determinant is
$$
G = e^{2\sigma} g~.
$$

---

We can expand the filed $\phi$ as
$$
\phi = \sum_{n \in \mathbb Z} \phi_n e^{iny/r}~.
$$
Then
$$
\partial \phi / \partial y = \sum_{n \in \mathbb Z} \phi_n \frac{in}{r} e^{iny/r}~.
$$
The effective Lagrangian of $D$-dimensional theory is
$$
\sqrt{-g} \mathcal L^{(D)} = \int dy \sqrt{-G} \mathcal L ^{(D+1)} = \int dy \,e^\sigma \sqrt{-g} \,\mathcal L ^{(D+1)}\\
= -e^\sigma \sqrt{-g}\, 2 \pi r \cdot \frac 12\sum_n\left( \partial_\mu \phi_n^* \partial^\mu \phi_n - \frac{n^2}{r^2} (A^2 +e^{-2\sigma}) |\phi_n|^2 - i \frac{n}{r} A^\mu (\phi_n \partial_\mu \phi_n^* -\phi_n^* \partial_\mu \phi_n)\right)~.
$$
Therefore, the mass of the field $\phi_n$ is $\frac{n^2}{r^2}e^{-2\sigma}$, its coupling to KK-gauge field is $n/r$.

---

We have
$$
\frac{2\pi r e^\sigma}{2 \kappa^2} e^{-2\langle \Phi\rangle} = \frac{2\pi \frac{\alpha'}{r}e^\sigma}{2\kappa^2} e^{-2\langle\widetilde \Phi\rangle},
$$
then
$$
\langle \widetilde \Phi\rangle = \langle \Phi\rangle - \frac 12 \ln \frac{r^2}{\alpha'}~.
$$


