![UniCA](https://github.com/unica-math/calc2/raw/main/logo-unica.png)

## L1
# Calculus 2
# 2025-26

# TD 2 - Équations différentielles linéaires (corrigé)

## Solution 1

Ce sont des équations à variables séparables.

a) $y = -\frac{1}{2}[\log(x)]^2 + \text{Cte}$, soit sur $I = ]-\infty,0[$, soit sur $I = ]0,\infty[$ (la cte dépendant de l'intervalle, sans possibilité de prolonger à $\mathbb{R}$.

b) Supposons $x \neq -\frac{1}{2}$. Alors $y' = -\frac{x^2+x-2}{2x+1}$ et donc $y' = -\frac{x}{2} - \frac{1}{4} + \frac{9}{4(2x+1)}$, ce qui donne $y = -\frac{x^2}{4} - \frac{x}{4} + \frac{9}{8}\log|2x + 1| + C$. Attention, la constante $C$ dépend de l'intervalle : $C = C_1$ sur $]-\infty,-\frac{1}{2}[$ et $C = C_2$ sur $]-\frac{1}{2},\infty[$.

c) $y = Ce^{e^x}$ sur $\mathbb{R}$.

---

## Solution 2

a) La solution générale de l'équation homogène (SGEH) est $y = Ce^{\frac{x}{2}}$. Or $y_0 = -2$ est une solution particulière de l'équation non homogène (SPENH). D'où la solution générale de l'équation non homogène (SGENH) $y = -2 + Ce^{\frac{x}{2}}$.

b) Idem. On trouve $y = Ce^{2x} + \frac{1}{2}$.

c) La SGEH est $y = Ce^{-2x}$. On cherche une SPENH sous la forme $y_0 = ax + b$. On trouve par identification $a = 1$ et $b = -\frac{1}{2}$. La SGENH est donc $y = Ce^{-2x} + x - \frac{1}{2}$.

d) La SGEH est $y = Ce^{-\frac{x}{2}}$. On cherche une SPENH sous la forme $y_0 = ke^x$ et on trouve $k = 1$. D'où $y_{\text{SGENH}} = Ce^{-\frac{x}{2}} - e^x$.

---

## Solution 3

a) $y = A\cos(3x) + B\sin(3x)$, sur $\mathbb{R}$

b) $y = Ae^{2x} + Be^{-2x}$, sur $\mathbb{R}$

c) $y = A\cos(x) + B\sin(x) + 4$, sur $\mathbb{R}$

d) $y = Ae^x + Be^{-x} + \frac{1}{3}e^{2x}$, sur $\mathbb{R}$

---

## Solution 4

a) La forme $y_0 = \alpha x \sin(\beta x)$ est SPENH si l'on a $y_0'' + y_0 = 2\cos x$, ce qui donne

$$-2\alpha\beta\cos(\beta x) + (1 - \beta^2)\sin(\beta x) = 2\cos x$$

En identifiant (puisque sin et cos sont linéairement indépendants), on peut choisir $\alpha = \beta = 1$ et on vérifie que $y_0 = x\sin x$ est bien solution de $(E_4)$.

b) En posant $y = u + x\sin x$, on trouve pour $(F_4)$ l'équation $u'' + u = 0$, équation homogène dont la solution générale est $u = A\cos x + B\sin x$ avec $A$ et $B$ deux constantes réelles.

La solution générale de $(E_4)$ est donc $y = A\cos x + B\sin x + x\sin x$.

On remarque que $y' = (1 - A)\sin x + (B + x)\cos x$.

c) Avec les conditions imposées, on cherche $A$ et $B$ telles que $A\cos\frac{\pi}{2} + B\sin\frac{\pi}{2} + \frac{\pi}{2}\sin\frac{\pi}{2} = 0$ et $(1 - A)\sin\frac{\pi}{2} + (B + x)\cos\frac{\pi}{2} = 0$. On trouve $A = 1$ et $B = -\frac{\pi}{2}$.

La solution est donc $\cos x - \frac{\pi}{2}\sin x + x\sin x$, définie sur $\mathbb{R}$ entier.

---

## Solution 5

On trouve

$$z'' = z \quad (F_5)$$

et $z = Ae^x + Be^{-x}$. D'où $y$ de la forme $y = \log|Ae^x + Be^{-x}|$.

On remarque que $y' = \frac{Ae^x - Be^{-x}}{Ae^x + Be^{-x}}$.

On cherche $A$ et $B$ telles que $y(0) = \log|A + B| = 0$ et $y'(0) = \frac{A - B}{A + B} = 0$, soit $A = B$ et $|2A| = 1$. Ce qui donne par exemple $A = B = \frac{1}{2}$ et $y = \log(\cosh x)$, $x \in \mathbb{R}$.

On peut vérifier que $y' = \tanh(x)$; $y'' = 1 - \tanh^2(x)$ et $y'' + y'^2 = 1$, avec $y(0) = 0$ et $y'(0) = 0$.

---
## Solution 6

L'équation $y' = \tan(x)y + x$ est une EDO linéaire non homogène (ENH) du premier ordre. On résout d'abord l'équation homogène (EH) associée $y' = \tan(x)y$. On va ensuite traiter le cas non homogène par la méthode de variation de la constante. La fonction tan est définie sur $\mathbb{R} \setminus (\frac{\pi}{2} + \pi\mathbb{Z})$. Fixons un entier $k \in \mathbb{Z}$ et l'on travaille sur l'intervalle ouvert $I_k = ]-\frac{\pi}{2} + k\pi, \frac{\pi}{2} + (k + 1)\pi[$. On peut vérifier aisément que la fonction $x \mapsto \log|\cos(x)|$ est une primitive de la fonction tan sur $I_k$. La solution générale de l'EH est alors $y_{\text{SGEH}} = \frac{C}{\cos(x)}$ avec $C$ une constante réelle (qui dépend de $I_k$, donc de $k$).

On cherche ensuite une solution particulière de l'ENH sous la forme $y_{\text{SPENH}} = \frac{C(x)}{\cos(x)}$. L'équation NH devient alors

$$\frac{C'(x)}{\cos(x)} + \frac{C(x)\sin(x)}{[\cos(x)]^2} = \tan(x)\frac{C(x)}{\cos(x)} + x$$

Les termes en $C(x)$ s'éliminent (on a tout fait pour !) et l'équation ci-dessus se réduit à une quadrature

$$\frac{C'(x)}{\cos(x)} = x$$

Une intégration par parties de $C'(x) = x\cos(x)$ conduit à $C(x) = x\sin(x) + \cos(x)$ et une solution particulière de l'ENH $y_{\text{SPENH}} = \frac{C(x)}{\cos(x)}$ s'écrit :

$$y_{\text{SPENH}} = x\tan(x) + 1$$

On peut revenir à la solution générale de l'ENH en ajoutant la solution générale de l'équation homogène (avec la constante !) à cette solution particulière :

$$y_{\text{SGENH}} = y_{\text{SPENH}} + y_{\text{SGEH}} = x\tan(x) + 1 + \frac{C}{\cos(x)}$$

avec $C \in \mathbb{R}$, $x \in I_k$. Il convient de noter que la constante $C$ peut être différente d'un $I_k$ sur l'autre.

**Nota :** on retrouve bien la structure en droite affine de la solution générale de l'ENH. On ajoute à un "point" $y_{\text{SPENH}} = x\tan(x) + 1$ un "vecteur" quelconque colinéaire à $\frac{1}{\cos(x)}$.

---

## Solution 7

1. On cherche une solution particulière de $(E)$, de la forme $y(x) = ax$ pour $x \in ]0,\infty[$. En injectant $y(x) = ax$ dans $(E)$, il vient

$$a - \frac{ax}{x} - a^2 x^2 = -9x^2$$

donc $a^2 = 9$. On peut prendre $y_0(x) = 3x$ comme solution particulière de $(E)$ définie sur $]0,\infty[$.

2. Effectuons le changement de fonction inconnue suivant : $y(x) = y_0(x) - \frac{1}{z(x)}$ où $z$ est une fonction définie sur $]0,\infty[$ à trouver. Ici $y_0(x) = 3x$ donc $y(x) = 3x - \frac{1}{z(x)}$. On calcule la dérivée et le carré de $y(x)$ pour l'injecter dans $(E)$ :

$$y'(x) = 3 + \frac{z'(x)}{z^2(x)} \quad \text{et} \quad y^2(x) = 9x^2 - \frac{6x}{z(x)} + \frac{1}{z^2(x)}$$

En injectant dans $(E)$ il vient

$$ 3 + \frac{z'(x)}{z^2(x)} - 3 + \frac{1}{xz(x)} - 9x^2 + \frac{6x}{z(x)} - \frac{1}{z^2(x)} = -9x^2 $$

d'où en simplifiant et arrangeant, il vient :

$$(E_1) \quad z'(x) + \left(6x + \frac{1}{x}\right)z(x) = 1$$

3. L'équation $(E_1)$ est une EDO linéaire non homogène. On cherche d'abord la solution générale de l'équation homogène :

$$(EH) \quad z'(x) + \left(6x + \frac{1}{x}\right)z(x) = 0$$

c'est-à-dire $z'/z = -(6x + 1/x)$ ce qui s'intègre en $\log|z| = -6x^2/2 - \log x + K$, avec $K$ constante. Il vient in fine que la solution générale de l'équation homogène est

$$z(x) = \frac{Ke^{-3x^2}}{x}$$

Il reste à trouver une solution particulière de l'équation non homogène $(E_1)$, $z_{\text{SPENH}}$. On applique la méthode de variation de la constante et on cherche $z_{\text{SPENH}}$ sous la forme $z_{\text{SPENH}} = \frac{C(x)e^{-3x^2}}{x}$. Sa dérivée vaut

$$z'_{\text{SPENH}}(x) = \frac{C'(x)e^{-3x^2}}{x} - \frac{6C(x)xe^{-3x^2}}{x} - \frac{C(x)e^{-3x^2}}{x^2}$$

et le second terme vaut

$$\left(6x + \frac{1}{x}\right)z_{\text{SPENH}}(x) = \left(6x + \frac{1}{x}\right)\frac{C(x)e^{-3x^2}}{x}$$

En additionnant ces deux expressions, les termes en $C(x)$ disparaissent et on obtient

$$C'(x)\frac{e^{-3x^2}}{x} = 1 \quad \text{ou encore} \quad C'(x) = xe^{3x^2} = \frac{1}{6}(6xe^{3x^2})$$

Ce qui donne $C(x) = \frac{1}{6}e^{3x^2}$ (on peut prendre la constante d'intégration à 0, puisque l'on cherche UNE solution particulière). Il vient enfin en remplaçant $C(x)$ :

$$z_{\text{SPENH}} = \frac{1}{6}e^{3x^2} \cdot \frac{e^{-3x^2}}{x} = \frac{1}{6x}$$

On vérifie que la fonction $z_{\text{SPENH}} = \frac{1}{6x}$ est bien solution particulière de $(E_1)$. La solution générale de $(E_1)$ est donc la somme de $\frac{1}{6x}$ et de $\frac{Ke^{-3x^2}}{x}$ :

$$z_{\text{SGENH}} = \frac{1}{6x} + \frac{Ke^{-3x^2}}{x}$$

Les solutions de $(E)$ sont ainsi de la forme

$$y(x) = y_0(x) - \frac{1}{z(x)} = 3x - \frac{1}{\frac{1}{6x} + \frac{Ke^{-3x^2}}{x}} = 3x - \frac{6x}{1 + Ae^{-3x^2}}$$

avec $A$ une constante réelle. Si $A > -1$, le dénominateur reste $> 0$ pour tout $x > 0$ et la solution est définie pour tout $x > 0$. Si $A < -1$, $\log(-A) > 0$ et le dénominateur peut s'annuler en $x_A = \sqrt{\log(-A)/3} > 0$ : d'après l'énoncé, on écarte ces dernières solutions.

## Solution 8

On considère l'équation $y'' - 3y' + 2y = e^x$. D'après le cours (section 3.2), le polynôme caractéristique est $f(r) = r^2 - 3r + 2 = (r - 1)(r - 2)$ et les solutions de l'équation homogène sont toutes les fonctions de la forme :

$$y(x) = c_1 e^x + c_2 e^{2x} \quad \text{avec } c_1, c_2 \in \mathbb{R}$$

Toujours d'après le cours (section 3.4), on est dans le cas où le second membre $e^x$ est de la forme $e^{\alpha x}P(x)$, avec $\alpha$ (ici $= 1$) racine simple de l'équation caractéristique, et $P(x) = 1$, polynôme de degré 0. On cherche une solution de la forme $y_p(x) = xQ(x)e^x$ avec $Q(x) = K$ constante (polynôme de même degré 0 que $P(x)$).

Il vient $y_p(x) = Kx\exp(x)$, $y_p'(x) = K\exp(x) + Kx\exp(x)$, $y_p''(x) = 2K\exp(x) + Kx\exp(x)$.

Soit

$$y_p'' - 3y_p' + 2y_p = 2K\exp(x) + Kx\exp(x) - 3K\exp(x) - 3Kx\exp(x) + 2Kx\exp(x) = -K\exp(x)$$

et on trouve $K = -1$.

Une solution particulière de l'ENH est donc $y_p(x) = -x\exp(x)$ (comme on peut le vérifier). Les solutions générales de l'équation non homogène sont les fonctions :

$$y(x) = (c_1 - x)e^x + c_2 e^{2x} \quad \text{avec } c_1, c_2 \in \mathbb{R}$$

---

## Solution 9

On cherche les solutions de $y'' - y = 6\cos x + 2x\sin x$.

L'équation caractéristique est $f(r) = r^2 - 1 = (r - 1)(r + 1)$ et l'équation homogène a pour solutions :

$$y(x) = c_1 e^x + c_2 e^{-x} \quad \text{avec } c_1, c_2 \in \mathbb{R}$$

Pour trouver une solution particulière de l'ENH, on peut ou bien utiliser la méthode de variation de la constante (telle que décrite en cours, pour les équations du second degré à coefficients constants), ou bien encore se référer au cours section 3.4, avec le second membre de la forme

$$e^{\alpha x}\left[P_1(x)\cos(\beta x) + P_2(x)\sin(\beta x)\right]$$

Ici, $\alpha = 0$, $P_1(x) = 6$, $\beta = 1$, $P_2(x) = 2x$. Comme $\alpha + i\beta = i$ n'est pas une racine de l'équation caractéristique, que le max des degrés des polynômes $P_1$ et $P_2$ est 1, on peut chercher une SP sous la forme $y_p(x) = (a_1 x + b_1)\cos(x) + (a_2 x + b_2)\sin(x)$. Il vient

$$y_p'(x) = (a_2 x + a_1 + b_2)\cos(x) - (a_1 x - a_2 + b_1)\sin(x)$$

et

$$y_p''(x) = -(a_1 x + 2a_2 - b_1)\cos(x) - (a_2 x + 2a_1 + b_2)\sin(x)$$

Soit $y_p'' - y_p = -2(a_1 x + a_2 - b_1)\cos(x) - 2(a_2 x + a_1 + b_2)\sin(x)$.

On trouve $a_1 = 0$, $a_2 - b_1 = -3$, $2a_2 = -2$, $a_1 + b_2 = 0$. Soit $a_1 = 0$, $b_2 = 0$, $a_2 = -1$ et $b_1 = 2$.

Et donc $y_p(x) = 2\cos(x) - x\sin(x)$ (et on peut vérifier que $y_p$ convient).

Les solutions sont les fonctions :

$$y(x) = c_1 e^x + c_2 e^{-x} + 2\cos x - x\sin x \quad \text{avec } c_1, c_2 \in \mathbb{R}$$

---

## Solution 10

On cherche les solutions de $4y'' + 4y' + 5y = \sin(x)e^{-x/2}$.

L'équation caractéristique est $f(r) = 4r^2 + 4r + 5$ a 2 racines complexes $r_1 = -1/2 + i$ et $r_2 = -1/2 - i = \overline{r_1}$.

Les solutions générales de l'équation homogène sont donc (cours, section 3.2 : $\alpha = -1/2$, $\beta = 1$) :

$$y_{\text{SGEH}} = e^{-x/2}(c_1\cos x + c_2\sin x) \quad \text{avec } c_1, c_2 \in \mathbb{R}$$

Encore une fois, le second membre est de la forme

$$e^{\alpha x}\left[P_1(x)\cos(\beta x) + P_2(x)\sin(\beta x)\right]$$

avec $\alpha = -1/2$ et $\beta = 1$ (et donc ici $\alpha + i\beta$ racine de l'équation caractéristique), $P_1(x) = 0$, $P_2(x) = 1$.

On cherche une SP sous la forme $y_p(x) = xe^{-x/2}\left[Q_1(x)\cos(x) + Q_2(x)\sin(x)\right]$, avec $Q_1$ et $Q_2$ deux polynômes de degré 0 donc deux constantes notées $q_1$ et $q_2$.

Il vient

$$y_p'(x) = \frac{1}{2}\exp(-x/2)\left[((q_1 - 2q_2)x - 2q_1)\cos(x) + 2((q_1 + q_2/2)x - q_2)\sin(x)\right]$$

et

$$y_p''(x) = \frac{3}{4}\exp(-x/2)\left(((x + 4/3)q_1 + \frac{4q_2(x - 2)}{3})\cos(x) - \frac{4}{3}\sin(x)((x - 2)q_1 + q_2(1 - 3x/4))\right)$$

et enfin

$$4y'' + 4y' + 5y = -8\exp(-x/2)(q_1\sin(x) - q_2\cos(x)) = \sin(x)e^{-x/2}$$

On en déduit $q_1 = -1/8$ et $q_2 = 0$. On vérifie que $y_p(x) = -\frac{1}{8}x\cos(x)e^{-x/2}$ est bien SP de l'ENH.

La solution générale de l'ENH est donc $y_p(x) + y_{\text{SGEH}}$, soit

$$y_{\text{SGENH}} = -\frac{1}{8}x\cos x e^{-x/2} + e^{-x/2}(c_1\cos x + c_2\sin x)$$

---

## Solution 11

On cherche d'abord les solutions de $y'' - 4y' + 4y = 0$.

1. L'équation caractéristique $r^2 - 4r + 4 = 0$ a une racine (double) $r = 2$ donc les solutions de l'équation homogène sont les fonctions :

$$y(x) = (c_1 x + c_2)e^{2x} \quad \text{où } c_1, c_2 \in \mathbb{R}$$

2. Pour $d(x) = e^{-2x}$, le second membre est de la forme $P(x)\exp(\alpha x)$ avec $\alpha = -2$ qui n'est pas racine de l'équation caractéristique. Le polynôme $P(x)$ est réduit à une constante. D'après le cours, on peut chercher une solution particulière de la forme : $y_p(x) = Ke^{-2x}$. Il vient $y_p'(x) = -2Ke^{-2x}$ et $y_p''(x) = 4Ke^{-2x}$. On substitue dans (ED) (avec second membre) pour trouver

$$y_p''(x) - 4y_p'(x) + 4y_p(x) = 4Ke^{-2x} - 4 \times (-2Ke^{-2x}) + 4 \times Ke^{-2x} = e^{-2x}$$

Soit $4K + 8K + 4K = 1$ et $K = \frac{1}{16}$ (et on vérifie bien que $y_p(x) = \frac{e^{-2x}}{16}$ est solution de (ED)).

Pour $d(x) = e^{2x}$, on cherche une solution de la forme $y_q(x) = ax^2 e^{2x}$ ($a \in \mathbb{R}$) car 2 est racine double de l'équation caractéristique. On a $y_q'(x) = (2ax + 2ax^2)e^{2x}$ et $y_q''(x) = (2a + 4ax + 4ax + 4ax^2)e^{2x} = (4ax^2 + 8ax + 2a)e^{2x}$. On trouve

$$(4ax^2 + 8ax + 2a - 4(2ax + 2ax^2) + 4ax^2)e^{2x} = e^{2x}$$

et donc $a = \frac{1}{2}$.

3. On déduit du principe de superposition (du fait de la linéarité) que la fonction

$$y_0(x) = \frac{1}{4}(-y_p(x) + y_q(x)) = -\frac{1}{64}e^{-2x} + \frac{1}{8}x^2 e^{2x}$$

est solution de l'équation pour le second membre donné dans cette question (on peut le vérifier directement). La forme générale des solutions est alors :

$$y_{\text{SGENH}}(x) = (c_1 x + c_2)e^{2x} - \frac{1}{64}e^{-2x} + \frac{1}{8}x^2 e^{2x} \quad \text{où } c_1, c_2 \in \mathbb{R}$$

---

## Solution 12

Les solutions de l'équation homogène $y'' + y = 0$ sont $\lambda\cos x + \mu\sin x$ où $\lambda, \mu \in \mathbb{R}$.

On cherche une solution particulière de l'équation avec second membre sous la forme

$$y_0(x) = \lambda(x)\cos x + \mu(x)\sin x$$

où cette fois $\lambda(x), \mu(x)$ sont des fonctions à trouver et qui vérifient (S) :

$$\begin{cases}
\lambda'y_1 + \mu'y_2 = 0 \\
\lambda'y_1' + \mu'y_2' = \frac{g(x)}{a}
\end{cases}$$

donc 

$$\begin{cases}
\lambda'\cos x + \mu'\sin x = 0 \\
-\lambda'\sin x + \mu'\cos x = \frac{1}{\cos x}
\end{cases}$$

En multipliant la première ligne par $\sin x$ et la seconde par $\cos x$, on obtient

$$\begin{cases}
\lambda'\cos x\sin x + \mu'(\sin x)^2 = 0 \\
-\lambda'\cos x\sin x + \mu'(\cos x)^2 = 1
\end{cases}$$

donc par somme $\mu' = 1$.

Ainsi $\mu(x) = x$ et la première ligne des équations devient $\lambda' = -\frac{\sin x}{\cos x}$ donc $\lambda(x) = \ln(\cos x)$.

On vérifie pour se rassurer que $y_0(x) = \ln(\cos x)\cos x + x\sin x$ est une solution de l'équation. Ainsi les fonctions solutions sont de la forme :

$$\lambda\cos x + \mu\sin x + \ln(\cos x)\cos x + x\sin x$$

quels que soient $\lambda, \mu \in \mathbb{R}$.

---

## Solution 13

On a que $f(x) = p(x) + q(x)$, avec $p(-x) = p(x)$ et $q(-x) = -q(x)$.

En dérivant $p$ et $q$, $\frac{dp}{dx} = \frac{1}{2}(f'(x) - f'(-x))$ et $\frac{dq}{dx} = \frac{1}{2}(f'(x) + f'(-x))$.

Si on dérive encore une fois, il vient $\frac{d^2p}{dx^2} = \frac{1}{2}(f''(x) + f''(-x))$ et $\frac{d^2q}{dx^2} = \frac{1}{2}(f''(x) - f''(-x))$.

On remarque que $\frac{d^2p}{dx^2}$ est paire et $\frac{d^2q}{dx^2}$ est impaire et que $f''(x) = \frac{d^2p}{dx^2} + \frac{d^2q}{dx^2}$.

En ré-injectant dans l'équation, il vient, puisque $f(-x) = p(x) - q(x)$, que

$$\frac{d^2p}{dx^2}(x) + \frac{d^2q}{dx^2}(x) + p(x) - q(x) = x\cos(x)$$

Evaluons cette équation en $(-x)$, il vient (en tenant compte des parités)

$$\frac{d^2p}{dx^2}(x) - \frac{d^2q}{dx^2}(x) + p(x) + q(x) = -x\cos(x)$$

En prenant la demi-somme et la demi-différence des deux équations ci-dessus (i.e. en distinguant partie paire et partie impaire), il vient le système :

$$\begin{cases}
p'' + p = 0 \\
q'' - q = x\cos(x)
\end{cases}$$

La première équation admet comme équation caractéristique $r^2 + 1 = 0$, dont les racines sont $\pm i$.

Les solutions de cette équation homogène sont donc $A\cos(x) + B\sin(x)$, avec $A$ et $B \in \mathbb{R}$. Il convient toutefois de faire attention au fait que l'on ne cherche pour cette équation que des solutions paires ! et donc $B = 0$.

La seconde équation admet comme équation caractéristique $r^2 - 1 = 0$, dont les racines sont $\pm 1$.

Les solutions de cette équation homogène sont donc $\alpha\exp(x) + \beta\exp(-x)$, avec $\alpha$ et $\beta \in \mathbb{R}$. (Nota : nous imposerons l'imparité à la fin des calculs). D'après le cours (section 3.4), on cherche donc une solution particulière par la méthode de variation des constantes, sous la forme $q_{sp} = \lambda(x)\exp(x) + \mu(x)\exp(-x)$, avec $\lambda$ et $\mu$ telles que (cf. cours système (S), page xxxiii)

$$\begin{cases}
\lambda'\exp(x) + \mu'\exp(-x) = 0 \\
\lambda'\exp(x) - \mu'\exp(-x) = x\cos(x)
\end{cases}$$

En prenant la demi-somme, il vient

$$\lambda' = \frac{1}{2}x\cos(x)\exp(-x)$$

et la demi-différence donne

$$\mu' = -\frac{1}{2}x\cos(x)\exp(x)$$

Les indications fournies dans l'énoncé permettent d'une part de déterminer $\lambda$ et $\mu$ selon

$$\lambda = \frac{1}{2}\int x\cos(x)\exp(-x)dx = \frac{1}{4}\exp(-x)[(1 + x)\sin(x) - x\cos(x)]$$

et

$$\mu = -\frac{1}{2}\int x\cos(x)\exp(x)dx = -\frac{1}{4}\exp(x)[(x - 1)\sin(x) + x\cos(x)]$$

Une solution particulière pour $q_{sp}$ est $\lambda(x)\exp(x) + \mu(x)\exp(-x)$, ce qui donne

$$q_{sp} = \frac{1}{4}[(1 + x)\sin(x) - x\cos(x)] - \frac{1}{4}[(x - 1)\sin(x) + x\cos(x)] = \frac{1}{2}(\sin(x) - x\cos(x))$$

On vérifie bien à posteriori que cette solution particulière proposée est bien impaire comme somme de deux fonctions impaires. La solution générale de l'équation pour la partie impaire est donc $\frac{1}{2}(\sin(x) - x\cos(x)) + \alpha\exp(x) + \beta\exp(-x)$. Mais il faut imposer que cette solution soit impaire ! Ce qui est OK si $\beta = -\alpha$ et que $\alpha\exp(x) + \beta\exp(-x)$ corresponde en fait à une fonction de type $K\sinh(x)$. In fine, en regroupant termes pairs et impairs pour les solutions générales, on obtient

$$f(x) = K\sinh(x) + A\cos(x) + \frac{1}{2}(\sin(x) - x\cos(x))$$

avec $K$ et $A \in \mathbb{R}$ et $x \in \mathbb{R}$.

On peut aisément vérifier directement que $f''(x) + f(x) = x\cos x$.
