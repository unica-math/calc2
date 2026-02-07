![UniCA](https://github.com/unica-math/calc2/raw/main/logo-unica.png)

## L1
# Calculus 2
# 2025-26

# TD 1 - Nombres complexes

---

### Exercice 1

Si $(a, b) \in \mathbf{R}^+ \times \mathbf{R}^+$, prouver que $\frac{1}{2}(a + b) \geq \sqrt{ab}$. Quand a-t-on égalité ?

---

### Exercice 2

Mettre sous la forme $a + ib$ $(a, b \in \mathbf{R})$ les nombres :

$$\frac{3 + 6i}{3 - 4i} \quad ; \quad \left(\frac{1 + i}{2 - i}\right)^2 + \frac{3 + 6i}{3 - 4i} \quad ; \quad \frac{2 + 5i}{1 - i} + \frac{2 - 5i}{1 + i}$$

---

### Exercice 3

On considère $a, b, c \in \mathbf{C}$, tels que $|a| = |b| = |c| = 1$.

Montrer que $|ab + bc + ac| = |a + b + c|$. (Indication : diviser le membre de gauche par $|abc|$.)

---

### Exercice 4

Écrire sous la forme $a + ib$ les nombres complexes suivants :

1. Nombre de module 2 et d'argument $\pi/3$.
2. Nombre de module 3 et d'argument $\pi/4$.

---

### Exercice 5

Placer dans le plan cartésien, les points d'affixes suivants :

$$z_1 = i, \quad z_2 = 1 + i, \quad z_3 = 2 + 2i, \quad z_4 = e^{i\frac{\pi}{3}}$$

---

### Exercice 6

1. Mettre sous forme trigonométrique les nombres complexes suivants :
   $$z_1 = 3 + 3i, \quad z_2 = 1 - \sqrt{3}i, \quad z_3 = \frac{4}{3}i, \quad z_4 = -2, \quad z_5 = e^{i\alpha} + e^{2i\alpha}

2. Calculer $\left(\frac{-1+i\sqrt{3}}{2}\right)^{2025}$.

---

### Exercice 7

Si $z = x + iy$, $(x, y) \in \mathbf{R}^2$,

1. Déterminer module et argument de $e^z$.
2. Déterminer $\overline{e^z}$, $e^{\overline{z}}$, $(e^z)^n$ pour $n \in \mathbf{Z}$.
3. L'application exponentielle
   $$\exp : \mathbf{C} \to \mathbf{C}, \quad z \mapsto e^z$$
   est-elle injective ? surjective ?

---

### Exercice 8

Soient $\alpha$ et $\beta$ deux nombres réels.

Mettre le nombre complexe $z = e^{i\alpha} - e^{i\beta}$ sous la forme $z = i\xi e^{i\mu}$ avec $\xi$ et $\mu$ deux réels.

**Indication :** on introduira $e^{i\frac{\alpha+\beta}{2}}$ et $e^{i\frac{\alpha-\beta}{2}}$.

---

### Exercice 9

On considère les nombres complexes $z_1 = e^{ia}$ et $z_2 = e^{ib}$ (avec $a$ et $b$ deux réels).

1. Donner la forme trigonométrique des nombres complexes $z_1$ et $z_2$.
2. En utilisant les résultats de la question précédente, calculer $z_1z_2$.
3. Déterminer la forme exponentielle de $z_1z_2$, puis en déduire sa forme trigonométrique.
4. En utilisant les questions précédentes, retrouver les formules d'addition de cosinus et sinus (i.e. $\cos(a + b)$ et $\sin(a + b)$).

---

### Exercice 10

On considère ici $a$ et $b$ deux nombres complexes.

1. Factoriser $e^{ia} + e^{ib}$ par $e^{i\frac{a+b}{2}}$. On simplifiera l'expression obtenue en utilisant les formules d'Euler.

2. En déduire que, pour tout couple $(p, q)$ de nombres réels, on a l'identité :
   $$\cos p + \cos q = 2\cos\left(\frac{p + q}{2}\right)\cos\left(\frac{p - q}{2}\right)$$

**Nota bene :** on pourra retrouver (et retenir...) de façon tout à fait analogue d'autres formules de trigonométrie :

$$\sin p + \sin q = 2\sin\left(\frac{p + q}{2}\right)\cos\left(\frac{p - q}{2}\right)$$

$$\sin p - \sin q = 2\cos\left(\frac{p + q}{2}\right)\sin\left(\frac{p - q}{2}\right)$$

$$\cos p - \cos q = -2\sin\left(\frac{p + q}{2}\right)\sin\left(\frac{p - q}{2}\right)$$

Il conviendra pour cela de factoriser $e^{ia} - e^{ib}$ par $e^{i\frac{a+b}{2}}$ (cf. exercice 7).

---

### Exercice 11

Calculer module et argument de $(1 + i)^n$.

---

### Exercice 12

Calculer les racines carrées de $\frac{1+i}{\sqrt{2}}$. En déduire les valeurs de $\cos(\pi/8)$ et $\sin(\pi/8)$.

---

### Exercice 13

Soient $n \in \mathbf{N}$ et $x \in \mathbf{R}$. On suppose que $\forall k \in \mathbf{Z}$, $x/2^k$ n'est pas un multiple de $\pi$.

Calculer $P_n = \prod_{k=0}^{n} \cos\left(\frac{x}{2^k}\right)$. (Indication : utiliser $\sin(2\alpha) = 2\sin\alpha\cos\alpha$.)

---

### Exercice 14

Montrer que les solutions de $ax^2 + bx + c = 0$ avec $a, b, c$ réels, sont réelles ou conjuguées.

---

### Exercice 15

Résoudre dans $\mathbf{C}$ l'équation $z^4 + 10z^2 + 169 = 0$.

---

### Exercice 16

On considère la fonction polynomiale en $z$

$$P(z) = z^4 - 6z^3 + 23z^2 - 34z + 26$$

1. Si $\alpha$ désigne un nombre complexe quelconque, démontrer que $P(\alpha) = \overline{P(\overline{\alpha})}$. En déduire que si $P(\alpha) = 0$, alors $P(\overline{\alpha}) = 0$.

2. Calculer $P(1 + i)$ puis indiquer deux solutions complexes de l'équation $P(z) = 0$.

3. On pose $Q(z) = [z - (1 + i)][z - (1 - i)]$.
   Vérifier que $P$ est le produit du polynôme $Q$ et d'un polynôme $R$ du second degré que l'on déterminera.
   Résoudre enfin dans $\mathbf{C}$ l'équation $P(z) = 0$.

---

### Exercice 17

1. Calculer $\frac{(1+i\sqrt{3})/2}{\sqrt{2}(1+i)/2}$ algébriquement, puis trigonométriquement. En déduire $\cos\frac{\pi}{12}$, $\sin\frac{\pi}{12}$, $\tan\frac{\pi}{12}$.

2. Résoudre dans $\mathbf{C}$ l'équation $z^{24} = 1$.

---

### Exercice 18

Soit $t \in ]0;\pi[$ et $n \in \mathbf{N}^*$. On définit $S_n$ telle que

$$S_n = \sum_{k=0}^{n} \cos(kt)$$

1. Déterminer $S_n$.
2. Montrer que $|S_n|$ est bornée indépendamment de $n$.

---

### Exercice 19

1. Développer $\cos(5\theta)$ et $\sin(5\theta)$.
2. Linéariser $\cos^5\theta$ et $\sin^5\theta$.

---

### Exercice 20 : Équation complexe d'une droite affine

On considère l'équation réelle d'une droite affine $D$ dans le plan (affine) :

$$ax + by = c$$

avec $a, b, c$ des nombres réels ($a$ et $b$ n'étant pas tous les deux nuls) et $(x, y) \in \mathbf{R}^2$.

Déterminer l'équation complexe d'une droite affine à partir de $a, b, c$ et des affixes $z = x + iy$ et $\overline{z} = x - iy$.

---

### Exercice 21

Trouver l'équation complexe du cercle de centre $\Omega$ et de rayon $r > 0$.

---

### Exercice 22

Considérons $A, B$ deux points du plan et $k > 0$ donné.

Montrer que l'ensemble des points $M$ tel que $\frac{MA}{MB} = k$ est

- une droite qui est la médiatrice de $[AB]$, si $k = 1$,
- un cercle, sinon.

---

### Exercice 23

1. Soient $A_1$ et $A_2$ deux points du plan $Oxy$ d'affixes respectifs $z_1$ et $z_2$. Montrer qu'un argument de $\frac{z_2}{z_1}$ est une mesure de l'angle orienté formé par les vecteurs $(\overrightarrow{OA_1}, \overrightarrow{OA_2})$. (Faire un dessin).

2. Soit $\Omega$ un point du plan $Oxy$ d'affixe $\omega$. Montrer qu'un argument de $\frac{z_2-\omega}{z_1-\omega}$ est une mesure de l'angle orienté formé par les vecteurs $(\overrightarrow{\Omega A_1}, \overrightarrow{\Omega A_2})$. (Faire un dessin, bis).

   **Indication :** on notera (cf. cours) que l'affixe de $\overrightarrow{\Omega A_1}$ (un vecteur) est $z_1 - \omega$.

---

### Exercice 24

Soient $a, b$ et $c$ trois nombres complexes de module 1 et d'arguments respectifs $\alpha, \beta, \gamma$. Les points $A, B, C$ d'affixes respectifs $a, b, c$ sont supposés distincts.

1. Établir la relation $\left(\frac{a - c}{b - c}\right)^2 = \lambda\frac{a}{b}$ avec $\lambda \in \mathbf{R}$ que l'on déterminera en fonction de $\alpha, \beta$ et $\gamma$.

2. Interprétation géométrique ? (Faire un dessin, bis).
