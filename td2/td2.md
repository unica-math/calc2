![UniCA](https://github.com/unica-math/calc2/raw/main/logo-unica.png)

## L1
# Calculus 2
# 2025-26

# TD 2 - Équations différentielles linéaires

## Exercice 1

Résoudre les équations différentielles :

a) $x y' + \log x = 0$

b) $(2x + 1) y' + x^2 + x - 2 = 0$

c) $y' - \exp y = 0$

---

## Exercice 2

Résoudre les équations différentielles :

a) $2y' - y = 2$

b) $y' - 2y + 1 = 0$

c) $y' + 2y = 2x$

d) $2y' + y = e^x$

---

## Exercice 3

Résoudre les équations différentielles :

a) $y'' + 9y = 0$

b) $y'' - 4y = 0$

c) $y'' + y = 4$

d) $y'' - y = e^{2x}$

---

## Exercice 4

On considère l'équation différentielle $(E_4)$ :

$$y'' + y = 2 \cos x \quad (E_4)$$

a) Trouver une solution particulière de $(E_4)$ sous la forme $y_0 = \beta x \sin \alpha x$, avec $\beta$ et $\alpha$ deux constantes à déterminer.

b) On pose maintenant $y = u + y_0$. Trouver l'équation $(F_4)$ vérifiée par $u$ ; la résoudre. En déduire la solution générale de $(E_4)$.

c) Déterminer la solution $y$ du problème aux CI suivant :  
$y$ vérifie $(E_4)$ ; $y$ et $y'$ s'annulent en $x = \pi/2$.  
On précisera l'intervalle de définition de la solution.

---

## Exercice 5

On considère l'équation différentielle $(E_5)$ :

$$y'' + y'^2 = 1 \quad (E_5)$$

a) On pose $z = \exp y$. Écrire l'EDO $(F_5)$ vérifiée par $z$.

b) Résoudre $(F_5)$ et en déduire la solution de $(E_5)$ telle que $y(x = 0) = 0$ et $y'(x = 0) = 0$.

---

## Exercice 6

Résoudre l'équation différentielle

$$y' = y \tan(x) + x$$

par la méthode de variation de la constante. On précisera l'intervalle de définition de la solution.

---

## Exercice 7

On se propose d'intégrer sur l'intervalle le plus grand possible contenu dans $]0,\infty[$ l'équation différentielle :

$$(E) \quad y'(x) - \frac{y(x)}{x} - \frac{y(x)}{2} = 9x^2$$

1. Déterminer $a \in ]0,\infty[$ tel que $y(x) = ax$ soit une solution particulière $y_0$ de $(E)$.

2. Montrer que le changement de fonction inconnue : $y(x) = y_0(x) - \frac{1}{z(x)}$ transforme l'équation $(E)$ en l'équation différentielle

$$(E_1) \quad z'(x) + \left(6x + \frac{1}{x}\right)z(x) = 1$$

3. Intégrer $(E_1)$ sur $]0,\infty[$.

4. Donner les solutions de $(E)$ définies sur $]0,\infty[$ entier.

---

## Exercice 8

Résoudre l'équation suivante :

$$y'' - 3y' + 2y = e^x$$

---

## Exercice 9

Résoudre l'équation suivante :

$$y'' - y = 6 \cos x + 2x \sin x$$

---

## Exercice 10

Résoudre l'équation suivante :

$$4y'' + 4y' + 5y = \sin x \, e^{x/2}$$

---

## Exercice 11

On considère l'équation différentielle suivante :

$$(ED) \quad y'' - 4y' + 4y = d(x)$$

où $d$ est une fonction qui sera précisée plus loin.

1. Résoudre l'équation différentielle homogène (i.e. sans le second membre $d(x)$) associée à $(ED)$.

2. Trouver une solution particulière de $(ED)$ lorsque $d(x) = e^{2x}$ et lorsque $d(x) = e^{-2x}$ respectivement.

3. Donner la forme générale des solutions de $(ED)$ lorsque $d(x) = \frac{e^{2x} + e^{-2x}}{4}$.

---

## Exercice 12

Résoudre l'équation suivante, sur l'intervalle $]-\frac{\pi}{2}, +\frac{\pi}{2}[$ :

$$y'' + y = \frac{1}{\cos x}$$

---

## Exercice 13

Déterminer les $f \in C^2(\mathbb{R}, \mathbb{R})$ telles que :

$$\forall x \in \mathbb{R}, \quad f''(x) + f(x) = x \cos x$$

**Indications :** On pourra décomposer $f$ en partie paire $p(x) = \frac{1}{2}(f(x) + f(-x))$ et partie impaire $q(x) = \frac{1}{2}(f(x) - f(-x))$.

On donne en outre :

$$\int x \cos(x) \exp(x) \, dx = \frac{1}{2} \exp(x) [(x - 1) \sin(x) + x \cos(x)]$$

et (en posant $x = -u$ dans l'expression précédente)

$$\int x \cos(x) \exp(-x) \, dx = \frac{1}{2} \exp(-x) [(1 + x) \sin(x) - x \cos(x)]$$
