![UniCA](https://github.com/unica-math/calc2/raw/main/logo-unica.png)

## L1
# Calculus 2
# 2025-26

# TD 1 - Nombres complexes (corrigé)

## Solution 1

Puisque $a$ et $b$ sont positifs ou nuls, $\sqrt{a}$ et $\sqrt{b}$ sont bien définis (dans $\mathbb{R}$) et $(\sqrt{a})^2 = a$, $(\sqrt{b})^2 = b$.

Considérons $(\sqrt{a} - \sqrt{b})^2$ qui est $\geq 0$. Il vient :

$$(\sqrt{a} - \sqrt{b})^2 \geq 0$$

et donc 

$$a - 2\sqrt{ab} + b \geq 0$$

et le résultat 

$$\frac{1}{2}(a + b) \geq \sqrt{ab}$$

Réciproquement, on a égalité lorsque $a - 2\sqrt{ab} + b = 0$, i.e. $(\sqrt{a} - \sqrt{b})^2 = 0$, et donc $a = b$.

La moyenne arithmétique de deux nombres positifs distincts est toujours plus grande que leur moyenne géométrique.

---

## Solution 2

Remarquons d'abord que pour $z \in \mathbb{C}$, $z\bar{z} = |z|^2$ est un nombre réel, ce qui fait qu'en multipliant le dénominateur par son conjugué, nous obtenons un nombre réel.

$$\frac{3 + 6i}{3 - 4i} = \frac{(3 + 6i)(3 + 4i)}{(3 - 4i)(3 + 4i)} = \frac{9 - 24 + 12i + 18i}{9 + 16} = \frac{-15 + 30i}{25} = -\frac{3}{5} + \frac{6}{5}i$$

Calculons

$$\frac{1 + i}{2 - i} = \frac{(1 + i)(2 + i)}{5} = \frac{1 + 3i}{5}$$

et

$$\left(\frac{1 + i}{2 - i}\right)^2 = \left(\frac{1 + 3i}{5}\right)^2 = \frac{-8 + 6i}{25} = -\frac{8}{25} + \frac{6}{25}i$$

Donc

$$\left(\frac{1 + i}{2 - i}\right)^2 + \frac{3 + 6i}{3 - 4i} = -\frac{8}{25} + \frac{6}{25}i - \frac{3}{5} + \frac{6}{5}i = -\frac{23}{25} + \frac{36}{25}i$$

Soit $z = \frac{2+5i}{1-i}$. Calculons $z + \bar{z}$, nous savons déjà que c'est un nombre réel, plus précisément : $z = \frac{-3}{2} + \frac{7}{2}i$ et donc $z + \bar{z} = -3$.

---

## Solution 3

Remarquons tout d'abord que pour tout complexe $z$ non nul, $z\bar{z} = |z|^2$. Aussi, $\forall z \in \mathbb{C}$, $|z| = |\bar{z}|$ et $\forall z \in \mathbb{C}$ et $\forall z' \in \mathbb{C}^*$, $|z/z'| = |z|/|z'|$.

Enfin, le complexe conjugué d'une somme de complexes est la somme des complexes conjugués. (idem pour le produit). Ces deux points à démontrer, si besoin.

Puisque $a$, $b$ et $c$ sont de module 1, ils ne peuvent être nuls (propriété d'intégrité).

Puisque $|a| = 1$, $|a|^2 = 1$ et donc $\bar{a} = 1/a$. Idem pour $b$ et $c$.

En outre $|abc| = |a||b||c| = 1$.

Calculons 

$$|ab + bc + ca| = \frac{|ab+bc+ca|}{|abc|} = \left|\frac{ab+bc+ca}{abc}\right| = \left|\frac{1}{c} + \frac{1}{a} + \frac{1}{b}\right| = |\bar{c} + \bar{a} + \bar{b}| = |\overline{a + b + c}| = |a + b + c|$$

et le résultat.

---

## Solution 4

On calcule

1. $z_1 = 2e^{i\frac{\pi}{3}} = 2(\cos\frac{\pi}{3} + i\sin\frac{\pi}{3}) = 2(\frac{1}{2} + i\frac{\sqrt{3}}{2}) = 1 + i\sqrt{3}$.

2. $z_2 = 3e^{-i\frac{\pi}{4}} = 3\cos\frac{\pi}{4} - 3i\sin\frac{\pi}{4} = 3\sqrt{2}/2 - 3i\sqrt{2}/2$.

---

## Solution 5

Cf. cours...

---

## Solution 6

1. On cherche d'abord le module du nombre complexe $z = x + iy$, qui est $r = \sqrt{x^2 + y^2} > 0$. On cherche ensuite un argument de $z$, qui est l'angle $\theta$ tel que $\cos\theta = x/r$, $\sin\theta = y/r$, avec en outre par exemple $\theta \in ]-\pi;\pi]$ ou $\theta \in [0; 2\pi[$.

Pour $z_1$, on trouve $r_1 = \sqrt{18} = 3\sqrt{2}$ et $\theta_1 \in ]-\pi;\pi]$ tel que $\cos\theta_1 = \sin\theta_1 = 1/\sqrt{2}$, soit $\theta_1 = \frac{\pi}{4}$.

Pour $z_2$, on trouve $r_2 = \sqrt{4} = 2$ ; $\theta_2 \in ]-\pi;\pi]$ tel que $\cos\theta_2 = -1/2$, $\sin\theta_2 = -\sqrt{3}/2$, soit $\theta_2 = -\frac{2\pi}{3}$.

$z_3 = \frac{4}{3}\exp(i\frac{\pi}{2})$ ; $z_4 = 2\exp(i\pi)$ (attention $r > 0$ et $\theta \in ]-\pi;\pi]$ !).

Pour $z_5$, une première méthode (frontale :(, à éviter ! ! !)

$$e^{i\alpha} + e^{2i\alpha} = (\cos\alpha + \cos 2\alpha) + i(\sin\alpha + \sin 2\alpha)$$

On utilise les identités (cf. exercice plus loin) :

$$\cos p + \cos q = 2\cos\frac{p+q}{2} \times \cos\frac{p-q}{2} \text{ et } \sin p + \sin q = 2\sin\frac{p+q}{2} \times \cos\frac{p-q}{2}$$

On trouve

$$\cos\alpha + \cos 2\alpha = 2\cos(3\alpha/2) \times \cos(\alpha/2) \text{ (cos est paire)}$$
$$\sin\alpha + \sin 2\alpha = 2\sin(3\alpha/2) \times \cos(\alpha/2)$$

Soit $e^{i\alpha} + e^{2i\alpha} = 2\cos(\alpha/2) \times (\cos(3\alpha/2) + i\sin(3\alpha/2))$.

Puisque l'on a supposé $\alpha \in [0;\pi]$, $\alpha/2 \in [0;\pi/2]$, et $\cos(\alpha/2) \in [0; 1]$ et est donc $> 0$. Il vient que $r_5 = 2\cos(\alpha/2) > 0$.

Si l'on adopte (pour simplifier !) la convention $\theta_5 = \arg(z_5) \in [0; 2\pi[$, alors on peut prendre $\theta_5 = 3\alpha/2$ qui est bien dans cet intervalle ($\alpha \in [0;\pi] \Rightarrow 3\alpha/2 \in [0; 3\pi/2]$).

**Deuxième méthode (qui est celle à privilégier...)**

$$e^{i\alpha} + e^{2i\alpha} = e^{i\alpha}(1 + e^{i\alpha})$$

Or $1 + e^{i\alpha} = e^{i\alpha/2}(e^{-i\alpha/2} + e^{i\alpha/2})$ ;

et comme $e^{i\alpha/2} + e^{-i\alpha/2} = 2\cos(\alpha/2)$, il vient $e^{i\alpha} + e^{2i\alpha} = 2\cos(\alpha/2)e^{3i\alpha/2}$ et le résultat.

2. On reconnaît tout d'abord le nombre complexe $\frac{-1+i\sqrt{3}}{2} = e^{i\frac{\pi}{3}}$ (complexe de module 1 et d'argument $\frac{\pi}{3} \in ]-\pi;\pi]$, car $\cos\frac{\pi}{3} = -\frac{1}{2}$ et $\sin\frac{\pi}{3} = \frac{\sqrt{3}}{2}$).

Ensuite, on forme $\left(\frac{-1+i\sqrt{3}}{2}\right)^{2025} = e^{i\frac{2025\pi}{3}} = e^{i675\pi} = e^{i\pi} = -1$.

---

## Solution 7

1. Pour $z = x + iy$, le module de $e^z = e^{x+iy} = e^x e^{iy}$ est $e^x$ et un argument est $y$, modulo $2\pi$.

2. Il vient directement $\overline{e^z} = e^{\bar{z}}$, $e^{-z} = (e^z)^{-1}$, $(e^z)^n = e^{nz}$.

3. La fonction exp n'est pas surjective car $|e^z| = e^x > 0$ et donc $e^z$ ne vaut jamais 0. La fonction exp n'est pas non plus injective car pour $z \in \mathbb{C}$, $e^z = e^{z+2i\pi}$.

---

## Solution 8

On peut écrire

$$e^{i\alpha} - e^{i\beta} = e^{i\frac{\alpha+\beta}{2}}(e^{i\frac{\alpha-\beta}{2}} - e^{-i\frac{\alpha-\beta}{2}}) = e^{i\frac{\alpha+\beta}{2}}(2i\sin\frac{\alpha-\beta}{2})$$

---

## Solution 9

1. cf. Cours ; on a directement $z_1 = \cos a + i\sin a$ et $z_2 = \cos b + i\sin b$.

2. On calcule directement le produit

$$z_1z_2 = (\cos a + i\sin a)(\cos b + i\sin b) = (\cos a\cos b - \sin a\sin b) + i(\cos a\sin b + \sin a\cos b)$$

3. On calcule le produit sous forme exponentielle

$$z_1z_2 = e^{ia}e^{ib} = e^{i(a+b)} = \cos(a + b) + i\sin(a + b)$$

4. En identifiant les formules de $z_1z_2$ des deux questions précédentes, on obtient les formules d'addition :

$$\cos(a + b) = \cos a\cos b - \sin a\sin b$$
$$\sin(a + b) = \cos a\sin b + \sin a\cos b$$

---

## Solution 10

1. On calcule :

$$e^{ia} + e^{ib} = e^{i\frac{a+b}{2}}(e^{i\frac{a-b}{2}} + e^{-i\frac{a-b}{2}}) = 2e^{i\frac{a+b}{2}}\cos\left(\frac{a-b}{2}\right)$$

2. On en déduit

$$\cos p + \cos q = \text{Re}(e^{ip} + e^{iq}) = \text{Re}\left(e^{i\frac{p+q}{2}}(e^{i\frac{p-q}{2}} + e^{-i\frac{p-q}{2}})\right) = 2\text{Re}\left(e^{i\frac{p+q}{2}}\cos\left(\frac{p-q}{2}\right)\right) = 2\cos\left(\frac{p+q}{2}\right)\cos\left(\frac{p-q}{2}\right)$$

---

## Solution 11

Comme $1 + i = \sqrt{2}\exp i\frac{\pi}{4}$, $(1 + i)^n$ a pour module $2^{n/2}$ et pour argument $n\frac{\pi}{4}$ (modulo $2\pi$).

---

## Solution 12

Par la méthode vue en cours, on peut calculer directement les racines carrées $\omega_1$, $\omega_2$ de $z = \frac{1+i}{\sqrt{2}}$.

On écrit $(a + ib)^2 = \frac{1+i}{\sqrt{2}}$ et donc $a^2 + 2iab - b^2 = \frac{1}{\sqrt{2}} + i\frac{1}{\sqrt{2}}$.

Soit $2ab = \frac{1}{\sqrt{2}}$ et $a^2 - b^2 = \frac{1}{\sqrt{2}}$.

On rajoute classiquement l'équation sur le module : $a^2 + b^2 = \sqrt{1/2 + 1/2} = 1$.

Soit encore $a^2 = \frac{1}{2}(1 + \frac{1}{\sqrt{2}})$ et $b^2 = \frac{1}{2}(1 - \frac{1}{\sqrt{2}})$.

Comme $ab > 0$, $a$ et $b$ sont de même signe, et les racines sont opposées l'une de l'autre ($\omega_1 = -\omega_2 = \omega$).

On obtient

$$\omega = \sqrt{\frac{\sqrt{2} + 1}{2\sqrt{2}}} + i\sqrt{\frac{\sqrt{2} - 1}{2\sqrt{2}}}$$

qui peut aussi s'écrire :

$$\omega = \frac{1}{2}\sqrt{2 + \sqrt{2}} + i\frac{1}{2}\sqrt{2 - \sqrt{2}}$$

On peut également remarquer que $z$ s'écrit sous forme trigonométrique

$$z = e^{i\frac{\pi}{4}}$$

et que $e^{i\frac{\pi}{8}}$ vérifie

$$(e^{i\frac{\pi}{8}})^2 = e^{\frac{2i\pi}{8}} = e^{i\frac{\pi}{4}}$$

Cela signifie que $e^{i\frac{\pi}{8}}$ est une racine carrée de $z$, donc $e^{i\frac{\pi}{8}} = \cos\frac{\pi}{8} + i\sin\frac{\pi}{8}$ est égal à $\omega$ ou $-\omega$. Comme $\cos\frac{\pi}{8} > 0$ alors $e^{i\frac{\pi}{8}} = \omega$ et donc par identification des parties réelles et imaginaires :

$$\cos\frac{\pi}{8} = \frac{1}{2}\sqrt{2 + \sqrt{2}} \text{ et } \sin\frac{\pi}{8} = \frac{1}{2}\sqrt{2 - \sqrt{2}}$$

---

## Solution 13

On va utiliser l'identité $\forall\theta \in \mathbb{R}$, $\sin(2\theta) = 2\sin(\theta)\cos(\theta)$.

Pour tout $k$ entier relatif, puisque $x/2^k$ n'est pas un multiple de $\pi$ par hypothèse, on a donc

$$\cos\left(\frac{x}{2^k}\right) = \frac{\sin\frac{x}{2^{k-1}}}{2\sin\frac{x}{2^k}}$$

En substituant, il vient

$$P_n = \prod_{k=0}^n \frac{\sin\frac{x}{2^{k-1}}}{2\sin\frac{x}{2^k}} = \frac{1}{2^{n+1}}\prod_{k=0}^n \sin\left(\frac{x}{2^{k-1}}\right)\prod_{k=0}^n \frac{1}{\sin\frac{x}{2^k}} = \frac{\sin(2x)}{2^{n+1}}\prod_{k=0}^{n-1}\sin\left(\frac{x}{2^k}\right)\prod_{k=0}^n \frac{1}{\sin\frac{x}{2^k}} = \frac{1}{2^{n+1}}\frac{\sin(2x)}{\sin(2^{-n}x)}$$

---

## Solution 14

Soit $P(z) = az^2 + bz + c$, et $\Delta = b^2 - 4ac$. Si $\Delta > 0$, alors les racines sont réelles : seul le cas où $\Delta < 0$ nous intéresse.

**Première méthode :** il suffit de déterminer les deux solutions et de vérifier qu'elles sont conjuguées...

**Seconde méthode :** si $z$ est une racine de $P$ i.e. $P(z) = 0$, alors

$$\overline{P(z)} = \overline{az^2 + bz + c} = a\bar{z}^2 + b\bar{z} + c = P(\bar{z}) = \overline{0} = 0$$

Donc $\bar{z}$ est aussi une racine de $P$. Or $z$ n'est pas un nombre réel (car $\Delta < 0$) donc $z \neq \bar{z}$. Sachant que le polynôme $P$ de degré 2 a exactement 2 racines, ce sont $z$ et $\bar{z}$ et elles sont conjuguées.

---

## Solution 15

On pose d'abord $u = z^2$. On résout l'équation $u^2 + 10u + 169 = 0$.

Le discriminant vaut $\Delta = 10 \times 10 - 4 \times 1 \times 169 = -576 = (24i)^2$.

Les racines sont complexes conjuguées et valent

$$u_1 = \frac{-10 + 24i}{2} = -5 + 12i \text{ et } u_2 = \bar{u_1} = \frac{-10 - 24i}{2} = -5 - 12i$$

Il reste à trouver les racines (complexes) de $u_1$ et $u_2$.

Leur module vaut $\sqrt{25 + 144} = \sqrt{169} = 13$.

Si on cherche par exemple $a$ et $b$ réels tels que $(a+ib)^2 = u_1 = -5+12i$, il vient $a^2+2iab-b^2 = -5+12i$ et $a^2 - b^2 = -5$, $2ab = 12$. Le carré du module des racines vaut $a^2 + b^2 = |u_1| = 13$ et donc $2a^2 = 8$ et $a = \pm 2$ ; $2b^2 = 18$ et $b = \pm 3$.

Dans le cas où $ab > 0$ ($u_1$), on trouve $2 + 3i$ et $-2 - 3i$.

Dans le cas où $ab < 0$ ($u_2$), on trouve $2 - 3i$ et $-2 + 3i$ (qui sont évidemment les conjuguées des 2 précédentes).

L'équation en $z$ a donc pour solutions : $2 + 3i$, $-2 - 3i$, $2 - 3i$, $-2 + 3i$ (ce que l'on peut vérifier).

---

## Solution 16

1. La fonction polynomiale $P(z)$ a tous ses coefficients réels. Si on prend l'expression conjuguée de $P(\alpha)$, tous les coefficients réels sont conjugués d'eux-mêmes : on trouve directement $\overline{P(\alpha)} = P(\bar{\alpha})$. (je ne détaille pas les calculs...)

On en déduit directement que si $\alpha \in \mathbb{C}$ est racine de $P(z)$, alors $\bar{\alpha} \in \mathbb{C}$ l'est aussi.

2. On calcule $(1 + i)^2 = 1 + 2i - 1 = 2i$ ; $(1 + i)^3 = 2i(1 + i) = -2 + 2i$ et $(1 + i)^4 = (2i)^2 = -4$

donc

$$P(1 + i) = -4 - 6(-2 + 2i) + 23 \times 2i - 34(1 + i) + 26 = -4 + 12 - 34 + 26 + i(-12 + 46 - 34) = 0$$

Ainsi, $1 + i$ et donc son conjugué $1 - i$ sont solutions de l'équation $P(z) = 0$.

3. On cherche $R(z)$ sous la forme $R(z) = az^2 + bz + c$. On calcule

$$[z - (1 + i)][z - (1 - i)][az^2 + bz + c]$$
$$= [z^2 - (1 - i)z - (1 + i)z + (1 - i^2)][az^2 + bz + c]$$
$$= az^4 + bz^3 + cz^2 - 2az^3 - 2bz^2 - 2cz + 2az^2 + 2bz + 2c$$
$$= az^4 + (b - 2a)z^3 + (c - 2b + 2a)z^2 + (-2c + 2b)z + 2c$$

En identifiant les coefficients, on trouve $a = 1$, $b - 2a = -6$, $c - 2b + 2a = 23$, $2b - 2c = -34$ et $2c = 26$.

D'où, $c = 13$, $b = -6 + 2 = -4$.

On retrouve bien aussi

$$c - 2b + 2a = 13 + 8 + 2 = 23 \text{ et } 2b - 2c = -8 - 26 = -34$$

Ainsi, $P(z) = [z^2 - (1 - i)z - (1 + i)z + (1 - i^2)][z^2 - 4z + 13] = Q(z) \times R(z)$

Le discriminant de $R(z) = z^2 - 4z + 13$ vaut $\Delta = 16 - 4 \times 13 = -36$ donc $R(z)$ a pour racines $2 \pm 3i$ et les solutions de l'équation $P(z) = 0$ sont in fine $1 + i$, $1 - i$, $2 + 3i$ et $2 - 3i$.

---

## Solution 17

**i) Calcul algébrique.**

Pour un quotient du type $z_1/z_2$, on multiplie numérateur et dénominateur par $\bar{z_2}$. On trouve

$$\frac{\frac{1+i\sqrt{3}}{2}}{\frac{\sqrt{2}(1+i)}{2}} = \frac{\frac{1+i\sqrt{3}}{2} \times \frac{\sqrt{2}(1-i)}{2}}{\frac{\sqrt{2}(1+i)}{2} \times \frac{\sqrt{2}(1-i)}{2}} = \frac{(-\frac{1}{2} + i\frac{\sqrt{3}}{2}) \times (\frac{1}{\sqrt{2}} - \frac{i}{\sqrt{2}})}{1} = \frac{1}{2\sqrt{2}}(\sqrt{3} + 1 + i(\sqrt{3} - 1))$$

**ii) Calcul trigonométrique.**

On reconnaît $\frac{1+i\sqrt{3}}{2} = e^{i\frac{\pi}{3}}$ et $\frac{\sqrt{2}(1+i)}{2} = e^{i\frac{\pi}{4}}$.

On en déduit

$$\frac{\frac{1 + i\sqrt{3}}{2}}{\frac{\sqrt{2}(1 + i)}{2}} = e^{i(\frac{\pi}{3} - \frac{\pi}{4})} = e^{i\frac{\pi}{12}}$$

On trouve ainsi 

$$\cos\frac{\pi}{12} = \frac{1 + \sqrt{3}}{2\sqrt{2}} \quad ; \quad \sin\frac{\pi}{12} = \frac{\sqrt{3} - 1}{2\sqrt{2}} \quad ; \quad \tan\frac{\pi}{12} = \sin\frac{\pi}{12}/\cos\frac{\pi}{12} = 2 - \sqrt{3}$$

Les racines de $z^{24} = 1$ sont données par $z_k = e^{2ki\pi/24}$ pour $k = 0,1,...,23$. Ce sont donc $1$, $\cos\frac{\pi}{12} + i\sin\frac{\pi}{12}$, $\cos\frac{2\pi}{12} + i\sin\frac{2\pi}{12}$, etc., que l'on peut déterminer par exemple de proche en proche grâce aux formules trigonométriques et à $\cos\frac{\pi}{12}$ et $\sin\frac{\pi}{12}$.

---

## Solution 18

1. On va calculer $\Sigma_n = \sum_{k=0}^n e^{ikt}$ et remarquer que $S_n = \text{Re}(\Sigma_n)$. Il vient, puisque $\Sigma_n$ est la somme d'une série géométrique de premier terme 1 et de raison $e^{it}$ :

$$\Sigma_n = \frac{e^{i(n+1)t} - 1}{e^{it} - 1}$$

Soit en factorisant par $e^{i(n+1)t/2}$ et en simplifiant par $2i$ (on utilise le fait que $2i\sin\theta = e^{i\theta} - e^{-i\theta}$) :

$$\Sigma_n = \frac{e^{i(n+1)t/2}\sin((n + 1)t/2)}{e^{it/2}\sin(t/2)}$$

il vient enfin

$$S_n = \text{Re}(\Sigma_n) = \frac{\cos(nt/2)\sin((n + 1)t/2)}{\sin(t/2)}$$

2. Puisque cos et sin sont toujours inférieurs à 1 en valeur absolue, et que $\sin(t/2)$ ne s'annule pas puisque $t \in ]0;\pi[$, il vient

$$|S_n| \leq \frac{1}{|\sin(t/2)|}$$

et le résultat.

---

## Solution 19

1. Pour développer $\cos(5\theta)$ et $\sin(5\theta)$, on écrit :

$$\cos(5\theta) + i\sin(5\theta) = e^{5i\theta} = (\cos(\theta) + i\sin(\theta))^5$$

La formule du binôme de Newton à l'ordre 5 s'écrit

$$(x + y)^5 = x^5 + 5x^4y + 10x^3y^2 + 10x^2y^3 + 5xy^4 + y^5$$

ce qui donne pour $e^{5i\theta} = (\cos(\theta) + i\sin(\theta))^5$

$$\cos(\theta)^5 + 5i\cos(\theta)^4\sin(\theta) - 10\cos(\theta)^3\sin(\theta)^2 - 10i\cos(\theta)^2\sin(\theta)^3 + 5\cos(\theta)\sin(\theta)^4 + i\sin(\theta)^5$$

En identifiant parties réelles et parties imaginaires, il vient :

$$\cos(5\theta) = 5\cos(\theta)\sin(\theta)^4 - 10\cos(\theta)^3\sin(\theta)^2 + \cos(\theta)^5$$

et

$$\sin(5\theta) = 5\cos(\theta)^4\sin(\theta) - 10\cos(\theta)^2\sin(\theta)^3 + \sin(\theta)^5$$

ce qui s'écrit également (à l'aide de $\cos^2\theta + \sin^2\theta = 1$)

$$\cos(5\theta) = 16\cos^5\theta - 20\cos^3\theta + 5\cos\theta$$

et

$$\sin(5\theta) = 16\cos(\theta)^4\sin(\theta) - 12\sin(\theta)\cos(\theta)^2 + \sin(\theta)$$

2. On utilise les formules d'Euler :

$$\cos\theta = \frac{e^{i\theta} + e^{-i\theta}}{2}, \quad \sin\theta = \frac{e^{i\theta} - e^{-i\theta}}{2i} = -i\frac{e^{i\theta} - e^{-i\theta}}{2}$$

afin de développer $\cos^5\theta$ et $\sin^5\theta$ à l'aide de la formule du binôme de Newton. On trouve pour le cosinus :

$$\cos^5\theta = \frac{e^{5i\theta}}{32} + \frac{5e^{3i\theta}}{32} + \frac{5e^{i\theta}}{16} + \frac{5e^{-i\theta}}{16} + \frac{5e^{-3i\theta}}{32} + \frac{e^{-5i\theta}}{32}$$

ce qui se regroupe en

$$\cos^5\theta = \frac{\cos(5\theta)}{16} + \frac{5\cos(3\theta)}{16} + \frac{5\cos(\theta)}{8}$$

Pour le sinus

$$\sin^5\theta = \frac{ie^{5i\theta}}{32} + \frac{5ie^{3i\theta}}{32} - \frac{5ie^{i\theta}}{16} + \frac{5ie^{-i\theta}}{16} - \frac{5ie^{-3i\theta}}{32} + \frac{ie^{-5i\theta}}{32}$$

ce qui se regroupe en

$$\sin^5\theta = \frac{\sin(5\theta)}{16} - \frac{5\sin(3\theta)}{16} + \frac{5\sin(\theta)}{8}$$

---

## Solution 20

Écrivons $z = x + iy \in \mathbb{C}$, alors

$$x = \frac{z + \bar{z}}{2}, \quad y = \frac{z - \bar{z}}{2i}$$

donc $D$ a aussi pour équation $a(z + \bar{z}) - ib(z - \bar{z}) = 2c$ ou encore $(a - ib)z + (a + ib)\bar{z} = 2c$.

Posons $\omega = a + ib \in \mathbb{C}^*$ et $k = 2c \in \mathbb{R}$ alors l'équation complexe d'une droite est :

$$\bar{\omega}z + \omega\bar{z} = k$$

où $\omega \in \mathbb{C}^*$ et $k \in \mathbb{R}$.

---

## Solution 21

Le cercle $\mathcal{C}(\Omega,r)$ est l'ensemble des points $M$ tels que distance$(\Omega, M) = r$. Si l'on note $\omega$ l'affixe de $\Omega$ et $z$ l'affixe de $M$, il vient :

$$\text{distance}(\Omega, M) = r \Leftrightarrow |z - \omega| = r \Leftrightarrow |z - \omega|^2 = r^2 \Leftrightarrow (z - \omega)(\bar{z} - \bar{\omega}) = r^2$$

et en développant nous trouvons que l'équation complexe du cercle centré en un point d'affixe $\omega$ et de rayon $r$ est :

$$z\bar{z} - \bar{\omega}z - \omega\bar{z} = r^2 - |\omega|^2$$

où $\omega \in \mathbb{C}$ et $r \in \mathbb{R}_+^*$.

---

## Solution 22

Si les affixes de $A$, $B$, $M$ sont respectivement $a$, $b$, $z$, cela revient à résoudre l'équation $\frac{|z-a|}{|z-b|} = k$.

$$\frac{|z - a|}{|z - b|} = k \Leftrightarrow |z - a|^2 = k^2|z - b|^2$$
$$\Leftrightarrow (z - a)(\bar{z} - \bar{a}) = k^2(z - b)(\bar{z} - \bar{b})$$
$$\Leftrightarrow (1 - k^2)z\bar{z} - z(\bar{a} - k^2\bar{b}) - \bar{z}(a - k^2b) + |a|^2 - k^2|b|^2 = 0$$

Donc si $k = 1$, on pose $\omega = a - k^2b$ et l'équation obtenue $z\bar{\omega} + \bar{z}\omega = |a|^2 - k^2|b|^2$ est bien celle d'une droite. Et bien sûr l'ensemble des points qui vérifient $MA = MB$ est la médiatrice de $[AB]$. 

Si $k \neq 1$ on pose $\omega = \frac{a - k^2b}{1 - k^2}$ alors l'équation obtenue est $z\bar{z} - z\bar{\omega} - \bar{z}\omega = \frac{|a|^2 + k^2|b|^2}{1 - k^2}$. C'est l'équation d'un cercle de centre $\omega$ et de rayon $r$ satisfaisant $r^2 - |\omega|^2 = \frac{|a|^2 + k^2|b|^2}{1 - k^2}$, soit $r^2 = \frac{|a - k^2b|^2}{(1 - k^2)^2} + \frac{|a|^2 + k^2|b|^2}{1 - k^2}$.

---

## Solution 23

1. Si l'on note $z_k = r_k e^{i\theta_k}$, avec $k = 1$ ou 2, il vient directement

$$\frac{z_2}{z_1} = \frac{r_2}{r_1}e^{i(\theta_2-\theta_1)}$$

$\theta_2 - \theta_1$ est un argument de $\frac{z_2}{z_1}$ et est bien une mesure (i.e. modulo $2\pi$) de l'angle orienté formé par les vecteurs $(\overrightarrow{OA_1}, \overrightarrow{OA_2})$.

2. Un argument de $\overrightarrow{\Omega A_1}$, d'affixe $z_1 - \omega$, est une mesure de l'angle orienté entre $Ox$ et le vecteur $\overrightarrow{\Omega A_1}$. Idem pour $A_2$. Un argument du rapport $\frac{z_2-\omega}{z_1-\omega}$ est une mesure de l'angle orienté entre les vecteurs $\overrightarrow{\Omega A_1}$ et $\overrightarrow{\Omega A_2}$.

---

## Solution 24

1. Puisque $a$, $b$ et $c$ sont de module unité, on a directement $a = e^{i\alpha}$, $b = e^{i\beta}$, $c = e^{i\gamma}$.

Formons le rapport

$$\frac{a - c}{b - c} = \frac{e^{i\alpha} - e^{i\gamma}}{e^{i\beta} - e^{i\gamma}} = \frac{\sin\frac{\alpha-\gamma}{2}e^{i\frac{\alpha+\gamma}{2}}}{\sin\frac{\beta-\gamma}{2}e^{i\frac{\beta+\gamma}{2}}} = \frac{\sin\frac{\alpha-\gamma}{2}}{\sin\frac{\beta-\gamma}{2}}e^{i\frac{\alpha-\beta}{2}}$$

où l'on a utilisé le résultat d'un exercice précédent. Et donc

$$\left(\frac{a - c}{b - c}\right)^2 = \left(\frac{\sin\frac{\alpha-\gamma}{2}}{\sin\frac{\beta-\gamma}{2}}\right)^2 e^{i(\alpha-\beta)} = \left(\frac{\sin\frac{\alpha-\gamma}{2}}{\sin\frac{\beta-\gamma}{2}}\right)^2 \frac{a}{b} = \lambda\frac{a}{b}$$

2. D'après un exercice précédent (ou le cours !), un argument de $\frac{a}{b}$ est une mesure de l'angle orienté formé par les vecteurs $(\overrightarrow{OB}, \overrightarrow{OA})$. De même, un argument de $\frac{a-c}{b-c}$ est une mesure de l'angle orienté formé par les vecteurs $(\overrightarrow{CB}, \overrightarrow{CA})$. Le carré dans la formule ci-dessus (et la positivité de $\lambda$) indique qu'une mesure du double de l'angle orienté $(\overrightarrow{CB}, \overrightarrow{CA})$ est égale à une mesure de l'angle orienté $(\overrightarrow{OB}, \overrightarrow{OA})$.

On retrouve le résultat géométrique (théorème de l'angle inscrit) qui stipule que, pour un cercle, l'angle au centre (ici, $(\overrightarrow{OB}, \overrightarrow{OA})$) est le double de l'angle inscrit (ici, $(\overrightarrow{CB}, \overrightarrow{CA})$).
