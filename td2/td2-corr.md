![UniCA](https://github.com/unica-math/calc2/raw/main/logo-unica.png)

## L1
# Calculus 2
# 2025-26

# TD 2 - Équations différentielles linéaires (corrigé ordre 1)

## Solution 1

Ce sont des équations à variables séparables.

a) $y = \frac{1}{2}[\log(x)]^2 + \text{Cte}$ ;

b) Supposons $x \neq -\frac{1}{2}$. Alors $y' = -\frac{x^2+x-2}{2x+1}$ et donc $y' = -\frac{x}{2} - \frac{1}{4} + \frac{9}{4(2x+1)}$, ce qui donne $y = -\frac{x^2}{4} - \frac{x}{4} + \frac{9}{8}\log|2x + 1| + C$. Attention, la constante $C$ dépend de l'intervalle : $C = C_1$ sur $]-\infty,-\frac{1}{2}[$ et $C = C_2$ sur $]-\frac{1}{2},\infty[$.

c) $y = \frac{1}{4}(e^x + C)^2$ sur $\mathbb{R}$.

---

## Solution 2

a) La solution générale de l'équation homogène (SGEH) est $y = Ce^{\frac{x}{2}}$. Or $y_0 = 2$ est une solution particulière de l'équation non homogène (SPENH). D'où la solution générale de l'équation non homogène (SGENH) $y = 2 + Ce^{\frac{x}{2}}$.

b) Idem. On trouve $y = Ce^{2x} + \frac{1}{2}$.

c) La SGEH est $y = Ce^{-2x}$. On cherche une SPENH sous la forme $y_0 = ax + b$. On trouve par identification $a = 1$ et $b = -\frac{1}{2}$. La SGENH est donc $y = Ce^{-2x} + x - \frac{1}{2}$.

d) La SGEH est $y = Ce^{-\frac{x}{2}}$. On cherche une SPENH sous la forme $y_0 = ke^x$ et on trouve $k = 1$. D'où $y_{\text{SGENH}} = Ce^{-\frac{x}{2}} - e^x$.

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

$$a - \frac{ax}{x} - \frac{a}{2}x = 9x^2$$

donc $\frac{a}{2} = 9$. On peut prendre $y_0(x) = 3x$ comme solution particulière de $(E)$ définie sur $]0,\infty[$.

2. Effectuons le changement de fonction inconnue suivant : $y(x) = y_0(x) - \frac{1}{z(x)}$ où $z$ est une fonction définie sur $]0,\infty[$ à trouver. Ici $y_0(x) = 3x$ donc $y(x) = 3x - \frac{1}{z(x)}$. On calcule la dérivée et le carré de $y(x)$ pour l'injecter dans $(E)$ :

$$y'(x) = 3 + \frac{z'(x)}{z^2(x)} \quad \text{et} \quad y^2(x) = 9x^2 - \frac{6x}{z(x)} + \frac{1}{z^2(x)}$$

En injectant dans $(E)$ il vient

$$3 + \frac{z'(x)}{z^2(x)} - \frac{3}{x} + \frac{1}{xz(x)} - \frac{9x^2}{2} + \frac{6x}{2z(x)} - \frac{1}{2z^2(x)} = 9x^2$$

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
