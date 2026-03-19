![UniCA](https://github.com/unica-math/calc2/raw/main/logo-unica.png)

## L1
# Calculus 2
# 2025-26

# TD 3 - Fonctions de plusieurs variables (corrigé)

## Solution 1

1. $f$ est définie pour $x > 0$ et $y > 0$ et est continue en tout point différent de $(0,0)$. Pour montrer qu'elle n'est pas continue en l'origine, il suffit par exemple de considérer l'image par $f$ de la suite $(x_n,y_n) = (1,1)/(n+1)$, laquelle ne tend pas vers $0 = f(0,0)$.

2. Pour la fonction $g(x, y) = \frac{x^2 y^2}{x^2 + y^2}$, $g$ est continue en tout point de $\mathbb{R}^2$ différent de $(0,0)$. Si on passe en coordonnées polaires il vient, avec $x = r\cos\theta$ et $y = r\sin\theta$, $x^2 + y^2 = r^2$,

$$g(x, y) = \frac{x^2 y^2}{x^2 + y^2} = \frac{r^4 \cos\theta \sin\theta}{r^2} = r^2 \cos\theta \sin\theta$$

Comme $\cos(\theta) \sin(\theta)$ reste borné ($\leq 1$ en valeur absolue), $r^2 \cos(\theta) \sin(\theta) \to 0 = g(0,0)$ lorsque $r \to 0$, \emph{i.e.} quand $(x,y) \to (0,0)$, d'où la continuité.

---

## Solution 2

Les deux limites existent et sont clairement nulles. On voit par contre que l'image (constante égale à $1$) par $f$ de la suite $(x_n,y_n) = (1,1)/(n+1)$ ne tend pas vers $0 = f(0,0)$.

---

## Solution 3

1. $D_f = \mathbb{R}^2$.
   - $\frac{\partial f}{\partial x} = 2x \exp(xy) + x^2 y \exp(xy)$
   - $\frac{\partial f}{\partial y} = x^3 \exp(xy)$

2. $D_f = \{x > 0 \text{ ou } y \neq 0\} \subset \mathbb{R}^2$
   - $\frac{\partial f}{\partial x} = \frac{1 + \frac{x}{\sqrt{x^2+y^2}}}{x + \sqrt{x^2 + y^2}} = \frac{1}{\sqrt{x^2 + y^2}}$
   - $\frac{\partial f}{\partial y} = \frac{\frac{y}{\sqrt{x^2+y^2}}}{x + \sqrt{x^2 + y^2}} = \frac{y}{x\sqrt{x^2 + y^2} + x^2 + y^2}$

3. $D_f = \mathbb{R}^2$
   - $\frac{\partial f}{\partial x} = 2\sin x \cos x$
   - $\frac{\partial f}{\partial y} = -2\sin y \cos y$

4. $D_f = \{z > 0\} \subset \mathbb{R}^3$ (la fonction est bien définie pour $z=0$ mais pas dérivable)
   - $\frac{\partial f}{\partial x} = 2xy^2\sqrt{z}$
   - $\frac{\partial f}{\partial y} = 2x^2 y\sqrt{z}$
   - $\frac{\partial f}{\partial z} = \frac{x^2 y^2}{2\sqrt{z}}$

---

## Solution 4

1. La fonction $f(x, y) = \frac{x^2 y}{x^2 + y^2}$ est définie, continue en dehors de l'origine (en tant que fonction fraction rationnelle dont le dénominateur ne s'annule pas). En passant en polaires,

$$f(x, y) = \frac{r^3\cos^2\theta\sin\theta}{r^2} = r \cos^2\theta \sin\theta \to 0 = f(0,0)$$

quand $r \to 0$ et on a continuité en $(0,0)$.

2. En $(0,0)$, les deux dérivées partielles existent et sont nulles. En dehors de $(0,0)$, les dérivées partielles existent et sont continues : 

$$\frac{\partial f}{\partial x}(x, y) = \frac{2xy}{x^2 + y^2} - \frac{2x^3 y}{(x^2 + y^2)^2}$$

$$\frac{\partial f}{\partial y}(x, y) = \frac{x^2}{x^2 + y^2} - \frac{2x^2 y^2}{(x^2 + y^2)^2}$$

On voit par contre (passer en polaires) qu'aucune des deux n'est continue en $(0,0)$ de sorte que la fonction est $C^1$ sur $\mathbb{R}^2 \backslash \{(0,0)\}$ mais pas sur tout $\mathbb{R}^2$.

---

## Solution 5

1. En polaires

$$f(x, y) = \frac{x^2 y + 3y^3}{x^2 + y^2} = r(\cos^2 \theta \sin\theta + 3\sin^3 \theta) \to 0 = f(0,0)$$

quand $r \to 0$, d'où la continuité en $(0,0)$.

2. Les dérivées partielles en $(0, 0)$ existent et valent

$$\frac{\partial f}{\partial x}(0, 0) = 0, $$

$$\frac{\partial f}{\partial y}(0, 0) = 3.$$

3. En dehors de l'origine, les dérivées partielles existent également et valent

$$\frac{\partial f}{\partial x}(x, y) = \frac{\partial}{\partial x}\frac{x^2 y + 3y^3}{x^2 + y^2} = \frac{2xy(x^2 + y^2) - 2x(x^2 y + 3y^3)}{(x^2 + y^2)^2} = \frac{-4xy^3}{(x^2 + y^2)^2}$$

$$\frac{\partial f}{\partial y}(x, y) = \frac{\partial}{\partial y}\frac{x^2 y + 3y^3}{x^2 + y^2} = \frac{(x^2 + 9y^2)(x^2 + y^2) - 2y(x^2 y + 3y^3)}{(x^2 + y^2)^2} = \frac{x^4 + 8x^2 y^2 + 3y^4}{(x^2 + y^2)^2}$$

Elles sont clairement continues en dehors de l'origine, en tant que fonctions fractions rationnelles dont le dénominateur ne s'annule pas.

4. On vérifie en passant en polaires qu'aucune des deux dérivées partielles n'est continue en $(0,0)$.

5. Cette équation s'écrit

$$z - 2 = \frac{\partial f}{\partial x}(1, 1)(x - 1) + \frac{\partial f}{\partial y}(1, 1)(y - 1) = -1 \cdot (x - 1) + 3(y - 1)$$

ou encore $z = 3y - x$.

---

## Solution 6

On calcule directement

$$\frac{\partial g}{\partial x} = \frac{\partial f}{\partial x} - \frac{\partial f}{\partial z}$$

$$\frac{\partial g}{\partial y} = -\frac{\partial f}{\partial x} + \frac{\partial f}{\partial y}$$

$$\frac{\partial g}{\partial z} = -\frac{\partial f}{\partial y} + \frac{\partial f}{\partial z}$$

d'où le résultat.

---

## Solution 7

a) En polaires, pour $(x,y) \neq (0,0)$,

$$\frac{x^2 - y^2}{x^2 + y^2} = \frac{r^2 \cos^2(\theta) - r^2 \sin^2(\theta)}{r^2} = \cos^2(\theta) - \sin^2(\theta) = \cos(2\theta)$$

qui reste inférieur à 1 en valeur absolue.

b) La continuité est claire en dehors de $(0,0)$. En ce point, puisque $\left|\frac{x^2-y^2}{x^2+y^2}\right|$ reste borné, il vient que

$$\lim_{(x, y) \to (0,0)} f(x, y) = 0$$

d'où la continuité en $(0,0)$.

c) Les deux dérivées partielles existent en $(0,0)$ et sont nulles. En dehors de l'origine, les dérivées partielles existnent et valent :

$$\frac{\partial f}{\partial x}(x, y) = y\frac{x^2 - y^2}{x^2 + y^2} + xy\frac{\partial}{\partial x}\frac{x^2 - y^2}{x^2 + y^2} = y\frac{x^2 - y^2}{x^2 + y^2} + \frac{4x^2 y^3}{(x^2 + y^2)^2}$$

$$\frac{\partial f}{\partial y}(x, y) = x\frac{x^2 - y^2}{x^2 + y^2} + xy\frac{\partial}{\partial y}\frac{x^2 - y^2}{x^2 + y^2} = x\frac{x^2 - y^2}{x^2 + y^2} - \frac{4x^3 y^2}{(x^2 + y^2)^2}$$

Elles sont clairement continues en dehors de l'origine, comme fonctions fractions rationnelles dont le dénominateur ne s'annule pas. En polaires,

$$\lim_{(x, y) \to (0,0)} \frac{x^2 y^3}{(x^2 + y^2)^2} = \lim_{r \to 0} \frac{r^5 \cos^2(\theta) \sin^3(\theta)}{r^4} = 0$$

$$\lim_{(x, y) \to (0,0)} \frac{x^3 y^2}{(x^2 + y^2)^2} = \lim_{r \to 0} \frac{r^5 \cos^3(\theta) \sin^2(\theta)}{r^4} = 0$$

d'où la continuité des deux dérivées partielles également en $(0,0)$ et le caractère $C^1$ de la fonction sur tout $\mathbb{R}^2$.

d) En dehors de l'origine, $f$ est clairement de classe $C^2$ comme fonction fraction rationnelle dont le dénominateur ne s'annule pas ; les dérivées partielles secondes croisées sont donc égales (théorème de Schwarz) : 

$$\frac{\partial^2 f}{\partial x \partial y} = \frac{\partial^2 f}{\partial y \partial x} = \frac{x^6 + 9x^4 y^2 - 9x^2 y^4 - y^6}{(x^2 + y^2)^3} = \frac{(x^4 + 10x^2 y^2 + y^4)(x^2 - y^2)}{(x^2 + y^2)^3}.$$

e) En $(0,0)$,
$$\frac{\partial^2 f}{\partial y \partial x}(0, 0) = -1,$$

$$\frac{\partial^2 f}{\partial x \partial y}(0, 0) = 1$$

ce qui indique (par contraposition) que les dérivées partielles secondes ne peuvent être continues en $(0,0)$.

---

## Solution 8

Les points critiques vérifient

$$
\begin{cases}
2(x-y)(x+y)+(x-y)^2+32x=0 \\
-(x-y)(x+3y)=0
\end{cases}
$$

La deuxième équation donne immédiatement

$$
(x-y)(x+3y)=0
$$

Donc

$$
x=y \quad \text{ou} \quad x=-3y.
$$

Cas 1 : $x=y$. La première équation donne directement $x=y=0$.

Cas 2 : $x=-3y$. On remplace dans la première équation, il vient
 
$$
32y(y-3)=0
$$

Ainsi

$$
y=0 \Rightarrow (0,0)
$$

ou

$$
y=3 \Rightarrow x=-9.
$$

Les points critiques sont donc

$$
(0,0) \quad \text{et} \quad (-9,3).
$$

En faisant $x=0$ et $y \to\pm\infty$, on voit néanmoins que $f$ ne peut avoir ni minimum ni maximum.

**NB.** De plus, au point $(0, 0)$, on remarque que $f(x, x) = 16x^2 > 0$, tandis que $f(0, y) = -y^3$, qui ne garde pas un signe constant : il n'y a donc pas d'extremum local en $(0, 0)$. Au point $(-9, 3)$, soit $u = (h, k) \in \mathbb{R}^2$. La valeur en $(-9, 3)$ est $f(-9, 3) = 432$ et

$$f(-9 + h, 3 + k) - 432 = 14h^2 + 12hk + 18k^2 + o(\|u\|^2)$$

Pour $k$ fixé, on peut remarquer que le trinôme en $h$, $T(h) = 14h^2 + 12hk + 18k^2$, a un discriminant strictement positif ($= 1152k^2$). Il ne garde donc pas un signe constant lorsque $h$ varie : il n'y a pas d'extremum local en $(-9, 3)$.

---

## Solution 9

1. La fonction $f$ est de classe $C^2$ sur $\mathbb{R}^2$, puisqu'elle est polynomiale en $x$ et $y$. Si $f$ admet un extremum en un point $(x_0, y_0)$ de $\mathbb{R}^2$, alors $(x_0, y_0)$ est nécessairement un point critique de $f$. On calcule le gradient :

$$\begin{cases}
\frac{\partial f}{\partial x} = 0 \\
\frac{\partial f}{\partial y} = 0
\end{cases}
\Leftrightarrow
\begin{cases}
3x^2 + 6xy - 15 = 0 \\
3x^2 - 12 = 0
\end{cases}
\Leftrightarrow
\begin{cases}
x = 2 \\
y = \frac{1}{4}
\end{cases}
\text{ ou }
\begin{cases}
x = -2 \\
y = -\frac{1}{4}
\end{cases}$$

qui sont donc les seuls candidats. En faisant $y=0$ et $x \to \pm\infty$, on voit que $f$ n'a ni minimum ni maximum.

**NB.** Pour étudier la nature de ces points critiques, on peut appliquer le critère de Monge (nécessité de la semi-définie positivité / négativité du Hessien en un minimum local / maximum local). On calcule $r = 6x + 6y$, $t = 0$ et $s = 6x$ puis $rt - s^2 = -36x^2$.

Ainsi, $(rt - s^2)\left(2, \frac{1}{4}\right) = (rt - s^2)\left(-2, \frac{1}{4}\right) = -144 < 0$.

Ceci implique que $f$ n'admet pas d'extremum local en $\left(2, \frac{1}{4}\right)$ ou $\left(-2, \frac{1}{4}\right)$.

2. La fonction $g$ est de classe $C^2$ sur $\mathbb{R}^2$ en tant que polynôme à plusieurs variables. Si $g$ admet un extremum  en $(x_0, y_0) \in \mathbb{R}^2$, alors $(x_0, y_0)$ est un point critique. Soit $(x, y) \in \mathbb{R}^2$.

$$\begin{cases}
\frac{\partial g}{\partial x}(x, y) = 0 \\
\frac{\partial g}{\partial y}(x, y) = 0
\end{cases}
\Leftrightarrow
\begin{cases}
4(x - y) + 4x^3 = 0 \\
-4(x - y) + 4y^3 = 0
\end{cases}
\Leftrightarrow
\begin{cases}
x^3 + y^3 = 0 \\
4(x - y) + 4x^3 = 0
\end{cases}
\Leftrightarrow
\begin{cases}
y = -x \\
x^3 - 2x = 0
\end{cases}$$

$$\Leftrightarrow (x, y) \in \left\{(0, 0), \left(\sqrt{2}, -\sqrt{2}\right), \left(-\sqrt{2}, \sqrt{2}\right)\right\}$$

De plus, pour tout $(x, y) \in \mathbb{R}^2$ (en utilisant $2|xy| \leq x^2 + y^2$),

$$g(x, y) - g\left(\sqrt{2}, -\sqrt{2}\right) = -2(x - y)^2 + x^4 + y^4 + 8 = x^4 + y^4 - 2x^2 - 2y^2 + 4xy + 8$$

$$\geq x^4 + y^4 - 2x^2 - 2y^2 - 2(x^2 + y^2) + 8$$

$$= (x^4 - 4x^2 + 4) + (y^4 - 4y^2 + 4) = (x^2 - 2)^2 + (y^2 - 2)^2$$

$$\geq 0$$

et $g\left(\sqrt{2}, -\sqrt{2}\right)$ est un minimum global, égal à $-8$. Idem en $\left(-\sqrt{2}, \sqrt{2}\right)$, par symétrie. Par ailleurs, $g(0, 0) = 0 > -8$ de sorte que $(0,0)$ ne peut ni minimiser, ni maximiser (évident !) la fonction.

**NB.** En évaluant d'une part $g(x,x)$, d'autre part $g(x,0)$ pour $x$ au voisinage de $0$, on voit que $g$ change de signe et que $(0,0)$ n'est pas même un extremum local.

## Solution 10

Le plan tangent à la surface d'équation $f(x, y, z) = 0$ au point $(x_0, y_0, z_0)$ est donné par l'équation

$$\frac{\partial f}{\partial x}(x_0, y_0, z_0)(x - x_0) + \frac{\partial f}{\partial y}(x_0, y_0, z_0)(y - y_0) + \frac{\partial f}{\partial z}(x_0, y_0, z_0)(z - z_0) = 0 \quad (1)$$

Soit $f : \mathbb{R}^3 \to \mathbb{R}$ la fonction définie par

$$f(x, y, z) = \sin(\pi xy) + \sin(\pi yz) - 1$$

Ses dérivées partielles sont

$$\frac{\partial f}{\partial x} = \pi y \cos(\pi xy), \quad \frac{\partial f}{\partial y} = \pi(x \cos(\pi xy) + z \cos(\pi yz)), \quad \frac{\partial f}{\partial z} = \pi y \cos(\pi yz)$$

et, après simplification, au point $\left(1, \frac{1}{6}, 1\right)$, l'équation (1) du plan tangent à la surface de niveau en discussion devient

$$(x - 1) + 12\left(y - \frac{1}{6}\right) + (z - 1) = 0$$

Ainsi, en ce point, le vecteur $(1, 12, 1)$ est perpendiculaire à la surface.

---

## Solution 11

1. Le plan tangent à la surface d'équation $z = f(x, y)$ au point $(x_0, y_0, z_0)$ est donné par l'équation

$$z - z_0 = \frac{\partial f}{\partial x}(x_0, y_0)(x - x_0) + \frac{\partial f}{\partial y}(x_0, y_0)(y - y_0)$$

On en déduit que l'équation du plan tangent au graphe $z = x^2 - 2y^3$ de la fonction $f$ au point $(x_0, y_0, z_0)$ est

$$z - z_0 = 2x_0(x - x_0) - 6y_0^2(y - y_0) = 2x_0 x - 6y_0^2 y - 2x_0^2 + 6y_0^3$$

2. Au point $(2, 1, 2)$, ce plan tangent est ainsi donné par l'équation

$$4x - 6y - z = 0$$

Pour que ce plan soit parallèle au plan tangent au point $(x_1, y_1, z_1)$ distinct de $(x_0, y_0, z_0)$ il faut et il suffit que $(4, -6, -1) = (2x_1, -6y_1^2, -1)$ et $y_1 \neq 1$, i.e. que $(x_1, y_1, z_1) = (2, -1, -6)$.

---

## Solution 12

Désignons respectivement par $(x_A, y_A, z_A)$ et $(x, y, z)$ les coordonnées de $A$ et de $M$ dans un repère orthonormé de $\mathbb{R}^3$. Alors

$$f_A(M) = AM^2 = (x - x_A)^2 + (y - y_A)^2 + (z - z_A)^2$$

1. Le gradient de $f_A$ est un vecteur de $\mathbb{R}^3$ qui a pour coordonnées

$$\text{grad}\,f_A = \begin{pmatrix}
\frac{\partial f_A}{\partial x} \\
\frac{\partial f_A}{\partial y} \\
\frac{\partial f_A}{\partial z}
\end{pmatrix}
= 2\begin{pmatrix}
x - x_A \\
y - y_A \\
z - z_A
\end{pmatrix}$$

2. La fonction $f(M) = AM^2 + BM^2 + CM^2$ admet comme gradient (avec des notations évidentes) :

$$\text{grad}\,f = \begin{pmatrix}
\frac{\partial f}{\partial x} \\
\frac{\partial f}{\partial y} \\
\frac{\partial f}{\partial z}
\end{pmatrix}
= 2\begin{pmatrix}
3x - x_A - x_B - x_C \\
3y - y_A - y_B - y_C \\
3z - z_A - z_B - z_C
\end{pmatrix}$$

Une condition nécessaire d'extremum est que le gradient soit nul, ce qui donne $x_i = (x_i^A + x_i^B + x_i^C)/3$ (avec la notation $(x_1, x_2, x_3) \equiv (x, y, z)$). Ces valeurs correspondent au barycentre $G$ de $(A, B, C)$. Ces valeurs ne peuvent correspondre à un maximum car on peut rendre $f(M)$ aussi grand que l'on souhaite en "éloignant" $M$ de chacun des 3 points.

Montrons qu'il s'agit bien d'un minimum. Pour cela on va s'éloigner du point $G$ et montrer que $f$ prend des valeurs supérieures à $f(G)$. On calcule par exemple $f(M) - f(G)$ avec (notations évidentes) $M = G + he_x + ke_y + le_z$, avec $h, k, l \in \mathbb{R}$ et non tous nuls. On trouve

$$f(G) = 2\left(\frac{x_A}{3} + \frac{x_B}{3} + \frac{x_C}{3}\right)^2 + \left(\frac{2y_A}{3} + \frac{y_B}{3} + \frac{y_C}{3}\right)^2 + \left(\frac{2z_A}{3} + \frac{z_B}{3} + \frac{z_C}{3}\right)^2$$

$$+ \left(\frac{-x_A}{3} + \frac{2x_B}{3} + \frac{x_C}{3}\right)^2 + \left(\frac{-y_A}{3} + \frac{2y_B}{3} + \frac{y_C}{3}\right)^2 + \left(\frac{-z_A}{3} + \frac{2z_B}{3} + \frac{z_C}{3}\right)^2$$

$$+ \left(\frac{x_A}{3} + \frac{x_B}{3} - \frac{2x_C}{3}\right)^2 + \left(\frac{y_A}{3} + \frac{y_B}{3} - \frac{2y_C}{3}\right)^2 + \left(\frac{z_A}{3} + \frac{z_B}{3} - \frac{2z_C}{3}\right)^2$$

et, tous calculs faits (...)

$$f(M) - f(G) = 3(h^2 + k^2 + l^2) > 0 \text{ puisque } h, k, l \text{ ne sont pas simultanément nuls}$$

Ce qui montre que $f(M)$ est toujours strictement supérieur à $f(G)$ pour $(h, k, l) \neq (0, 0, 0)$ et $f$ présente bien un minimum (global) en $G$.

Pour le détail des calculs, on peut par exemple voir ce qui se passe pour la coordonnée $x$.

On calcule

$$(2x_A/3 + x_B/3 + x_C/3 + h)^2 + (x_A/3 - 2x_B/3 + x_C/3 + h)^2 + (x_A/3 + x_B/3 - 2x_C/3 + h)^2$$

$$- (2x_A/3 + x_B/3 + x_C/3)^2 - (x_A/3 - 2x_B/3 + x_C/3)^2 - (x_A/3 + x_B/3 - 2x_C/3)^2$$

$$= 2h(2x_A/3 + x_B/3 + x_C/3 + x_A/3 - 2x_B/3 + x_C/3 + x_A/3 + x_B/3 - 2x_C/3) + 3h^2$$

$$= 3h^2$$
