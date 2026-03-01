![UniCA](https://github.com/unica-math/calc2/raw/main/logo-unica.png)

## L1
# Calculus 2
# 2025-26

# TD 3 - Fonctions de plusieurs variables

## Exercice 1

Étudier la continuité sur ℝ² des fonctions suivantes :

1. $f(x, y) = \frac{x^{1/2} y^{3/2}}{x^2 + y^2}$ et $f(0, 0) = 0$

2. $g(x, y) = \frac{x^2 y^2}{x^2 + y^2}$ et $g(0, 0) = 0$

---

## Exercice 2

Soit $f : \mathbb{R}^2 \setminus \{(0, 0)\} \to \mathbb{R}$ la fonction définie par :

$$f(x, y) = \frac{x^2 y^2}{x^2 y^2 + (x - y)^2}$$

Montrer que :

$$\lim_{x \to 0, x \neq 0} f(x, 0) = \lim_{y \to 0, y \neq 0} f(0, y) = 0$$

mais que $\lim_{(x, y) \to (0,0), (x, y) \neq (0, 0)} f(x, y)$ n'existe pas.

---

## Exercice 3

Déterminer, pour chacune des fonctions suivantes, le domaine de définition $D_f$. Pour chacune des fonctions, calculer ensuite les dérivées partielles en chaque point du domaine de définition lorsqu'elles existent :

1. $f(x, y) = x^2 e^{xy}$

2. $f(x, y) = \ln(x + \sqrt{x^2 + y^2})$

3. $f(x, y) = \sin^2 x + \cos^2 y$

4. $f(x, y, z) = x^2 y^2 \sqrt{z}$

---

## Exercice 4

1. Étudier la continuité en $(0, 0)$ de la fonction $f(x, y) = \frac{x^2 y}{x^2 + y^2}$ et $f(0, 0) = 0$.

2. La fonction $f$ est-elle de classe $C^1$ sur ℝ² entier ?

---

## Exercice 5

On considère $f : \mathbb{R}^2 \to \mathbb{R}$ la fonction définie par :

$$f(x, y) = \frac{x^2 y + 3y^3}{x^2 + y^2} \text{ pour } (x, y) \neq (0, 0)$$

$$f(0, 0) = 0$$

1. La fonction $f$ est-elle continue en $(0, 0)$ ?

2. La fonction $f$ admet-elle des dérivées partielles par rapport à $x$, à $y$ en $(0, 0)$ ?

3. Déterminer les dérivées partielles de $f$ en un point $(x, y) \neq (0, 0)$.

4. La fonction $f$ est-elle de classe $C^1$ ?

5. Déterminer l'équation du plan tangent au graphe de $f$ au point $(1, 1, 2)$.

**Rappel :** Le plan tangent au point $(x_0, y_0, f(x_0, y_0))$ du graphe $z = f(x, y)$ de $f$ est donné par l'équation :

$$z - f(x_0, y_0) = \frac{\partial f}{\partial x}(x_0, y_0)(x - x_0) + \frac{\partial f}{\partial y}(x_0, y_0)(y - y_0)$$

---

## Exercice 6

Soit $f : \mathbb{R}^3 \to \mathbb{R}$ une fonction de classe $C^1$ et soit $g : \mathbb{R}^3 \to \mathbb{R}$ la fonction définie par :

$$g(x, y, z) = f(x - y, y - z, z - x)$$

Montrer que la somme des coordonnées de $\nabla g$ est nulle.

---

## Exercice 7

Soit la fonction $f : \mathbb{R}^2 \to \mathbb{R}$ définie par :

$$f(x, y) = xy \frac{x^2 - y^2}{x^2 + y^2} \text{ si } (x, y) \neq (0, 0)$$

$$f(0, 0) = 0$$

a) Montrer que $\left|\frac{x^2 - y^2}{x^2 + y^2}\right|$ reste borné, pour tout $(x, y) \neq (0, 0)$.

b) Étudier la continuité de $f$.

c) Montrer que $f$ est de classe $C^1$ sur ℝ².

d) Justifier que $f$ est de classe $C^2$ sur tout ouvert de ℝ² ne contenant pas $(0, 0)$. Que peut-on en déduire sur les deux fonctions $\frac{\partial^2 f}{\partial x \partial y}$ et $\frac{\partial^2 f}{\partial y \partial x}$ ?

e) Déterminer $\frac{\partial^2 f}{\partial x \partial y}(0, 0)$ et $\frac{\partial^2 f}{\partial y \partial x}(0, 0)$. Que peut-on en déduire ?

---

## Exercice 8

Étudier les extrema de la fonction $f$ de ℝ² dans ℝ définie par :

$$\forall (x, y) \in \mathbb{R}^2, \quad f(x, y) = (x - y)^2(x + y) + 16x^2$$

---

## Exercice 9

Étudier les extrema des fonctions suivantes :

1. $f(x, y) = x^3 + 3x^2 y - 15x - 12y$

2. $g(x, y) = 2(x - y)^2 + x^4 + y^4$

---

## Exercice 10

Déterminer l'équation du plan tangent à la surface de niveau :

$$\sin(\pi xy) + \sin(\pi yz) = 1$$

au point de coordonnées $(1, \frac{1}{6}, 1)$.

Identifier, en ce point, un vecteur perpendiculaire à la surface.

---

## Exercice 11

Soit $f$ la fonction définie sur ℝ² par $f(x, y) = x^2 - 2y^3$.

1. Déterminer l'équation du plan tangent $P_{M_0}$ au graphe $G_f$ de $f$ en un point quelconque $M_0$ de $G_f$.

2. Pour le point $M_0$ de coordonnées $(2, 1, 2)$, déterminer tous les points $M$ tels que le plan tangent en $M$ soit parallèle à $P_{M_0}$.

---

## Exercice 12

Soit $A \in \mathbb{R}^3$ fixé et soient :

$$f_A : \mathbb{R}^3 \to \mathbb{R}$$
$$M \mapsto AM^2$$

1. Calculer le gradient de $f_A$ en un point $M$.

2. Soient $A$, $B$, $C$ trois points distincts de ℝ³. Trouver les points $M$ réalisant le minimum de $AM^2 + BM^2 + CM^2$.
