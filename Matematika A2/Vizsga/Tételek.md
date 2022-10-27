# Tételek 2022

1. (a) **Hatványsor**. Konvergencia tartomány, jellemzése. **Konvergenciasugár**, meghatározása (B). 2. (b) Hatványsor deriváltja, integrálja. 3. (c) Függvénysorozat. **Pontonkénti és egyenletes konvergencia**. Cauchy kritérium
2. (a) Függvénysor. **Pontonkénti és egyenletes konvergencia**. Cauchy kritérium.
   1. (b) Elégséges feltétel függvénysor egyenletes konvergenciára (B). Összegfüggvény folytonossága (B), deriváltja és integrálja.
   2. (c) Trigonometrikus sor. **Trigonometrikus függvényrendszer**, 'ortogonalitása' (B)
3. (a) **Fourier sor**. Derivált függvény Fourier sora (B).
   1. (b) **Fourier sor konvergenciája**. Parseval egyenlőség Fourier sorokra.
   2. (c) Fourier sor **komplex alakja**. Parseval egyenlet a komplex Fourier sorra.
4. (a) **Fourier transzformáció**. Alaptulajdonságok, idő- és frekvenciatartomány
   1. (b) A Fourier transzformáció valós fixpontja. (B)
   2. (c) **Inverz Fourier transzformáció**. Parseval egyenlet a FT-ra (B).
5. (a) **FT és deriválás** időtartományban ill. frekvenciatartományban.
   1. (b) Konvolúció, tulajdonságai. **Konvolúció és FT kapcsolata**.
   2. (c) Kétváltozós függvény értelmezése, ábrázolása. Polár-koordináták a síkon.
6. (a) **Folytonosság, sorozatfolytonosság**. Egyenletes folytonosság. Határérték.
   1. (b) Bolzano tétel két dimenzióban (B). **Weierstrass tételek.**
   2. (c) **Parciális deriváltak.** Geometriai jelentés. Kapcsolat a folytonossággal (B)
7. (a) Magasabb rendű parciális deriváltak, **deriválások sorrendje**.
   1. (b) **Teljes differenciálhatóság**. **Gradiens**. Folytonosság és differenciálhatóság (B)
   2. (c) Kétváltozós függvény **érintősíkja** adott pontban. (B)
8. (a) **Iránymenti derivált**, kiszámítása (B). Hesse mátrix.
   1. (b) Kétváltozós függvény lokális szélsőértéke. **Szükséges feltétel létezésre** (B). Stacionárius pont. Nyeregpont.
   2. (c) **Elégséges feltétel lokális szélsőértékre** kétváltozós függvény esetén.
9. (a) **Feltételes szélsőérték feladat**. Lagrange-féle multiplikátor szabály. (B vázlat)
   1. (b) Lagrange féle középérték tétel **kétváltozós** (B) ill. n változós függvényekre.
   2. (c) **Lánc-szabály** kétváltozós függvényre, speciális esetek.
10. (a) n-változós függvény: **gradiens, Hesse mátrix**, iránymenti derivált.
    1. (b) Lokális szélsőérték n-változós függvényekre. **Szükséges feltétel** (B).
    2. (c) **Másodrendű Taylor formula**, kétváltozós függvényre (B).
    3. (d) Implicit függvény tétel, implicit deriválás. (B)
11. (a) **Függvény rendszer** (koordináta-transzformáció). Folytonosság.
    1. (b) Deriválhatóság. **Jacobi mátrix**, Jacobi determináns.
    2. (c) Függvényrendszer invertálhatósága. **Inverz rendszer**, annak Jacobi mátrixa. Pl. lineáris transzformáció (B).
12. (a) Riemann integrál kétváltozós függvényre, szemléletes jelentés. Értelmezése.
    1. (b) Alaptulajdonságok. **Integrálás téglalap tartományon** (B).
    2. (c) Normáltartomány. **Integrálás síkbeli normáltartományon**.
13. (a) **Áttérés polár-koordinátákra kettős integrálban**. Koordináta transzformáció Jacobi determinánsa (B) 4. (b) Általános helyettesítés kettős integrálban. 5. (c) Háromváltozós függvény integrál. Spec: **intervallumon** és normál tartományon.
14. (a) **Gömbi polárkoordináták**, Jacobi determinánsa (B)
    1. (b) Improprius kettős integrál nem korlátos függvényre ill. nem korlátos tartományon.
    2. (c) Példa: harang-görbe integrálja a síkon.(B).
15. (a) Vonal $\mathbb{R}^2$-ben. **Valós kétváltozós függvény vonalintegrálja**.
    1. (b) Vektormező vonalintegrál. **Potenciálkeresés**.
    2. (c) Potenciál létezésének **szükséges** (B) és elégséges feltétele (vonalintegrállal).
16. (a) Magasabb rendű lineáris DE. **Homogén LDE: megoldások tere**
    1. (b) **Függvények függetlensége**. Wronsky determináns, alkalmazása (részben B)
    2. (c) Állandó együtthatós homogén LDE. **Karakterisztikus polinom, szerepe** (B).
17. (a) Inhomogén LDE: **megoldások struktúrája** (B). Partikuláris megoldás.
    1. (b) Differenciálegyenlet rendszer 3 dimenzióban.
    2. (c) Állandó együtthatós LDER megoldása (B). $e^A$ **értelmezése**
18. (a) Komplex függvény, "ábrázolás". **Kanonikus alak**. Határérték,folytonosság.
    1. (b) Komplex függvény deriválhatósága. **Cauchy-Riemann egyenletek**. (részben B)
    2. (c) **Harmonikus** függvény. Kapcsolat a komplex analitikus függvénnyel (B). Harmonikus társ.
    3. (d) Elemi komplex függvények: $e^z$ **alaptulajdonságok** (részben B). Logaritmus.

## Kidolgozott tételek 2022

### 1. Tétel

(a)
**Hatványsor**: $\sum^\infty_{n=0}c_n(x-x_0)^n ; c_n\in \mathbb{R} ; x_0\in\mathbb{R} fix$

Konvergencia tartomány, jellemzése: $\mathcal{H}=x\in \mathbb{R}: \sum^\infty_{n=0}c_nx^n<\infty$ ; ha $\xi \in \mathcal{H}$ akkor minden x-re ami kisebb, igaz hogy x is benne, fordítva meg hogy x nincs benne

**Konvergenciasugár**: tfh $\exists \xi \neq 0 ; \xi \in \mathcal{H} ; \exists \eta \notin \mathcal{H}$ ; ekkor sugár $\rho \coloneqq \sup\{|x|:x\in\mathcal{H}\}$
$\mathcal{H}={0} \to p:=0$
$\mathcal{H}=\mathbb{R} \to p:= \inf$

Konvergenciasugár meghatározása (B) $x_0=0$ esetben gyökkritériummal $\lim_{n\to \infty}\sqrt[n]{|a_n|}=\gamma$, ahol $a_n=c_nx^n$

(b) Hatványsor deriváltja, integrálja.
deriválás: vegyünk egy hatványsort, amire teljesül a gyökkrit, $\gamma$ innen "$p=\frac{1}{\gamma}$"
ekkor $f$ akárhányszor diffható, éspedig $f^{(k)}(x)=\sum_{n=k}^\infty \frac{n!}{(n-k)!}a_n(x-x_0)^{n-k}$
integrálás: $\int f(x) \,\,dx = \sum^\infty_{n=0}\frac{a_n(x-x_0)^{n+1}}{n+1}+C$
(c) Függvénysorozat: adott $f_1,f_2,f_n, : D \to \mathbb{R}$ fvk, ÉT közös. ezek sorozatát fvsorozatnak nevezzük, jele $f_n$

Cauchy kritérium: az $f_n$ pontosan akkor konvergens, ha $\forall \epsilon \gt 0$-hoz és minden $x \in D$-hez $\exists N = N(\epsilon, x)$ küszöbindex, amire $\forall m,n \gt N$ esetén $|f_n(x)-f(x)|\lt \epsilon$

**Pontonkénti és egyenletes konvergencia:**
Pontonkénti konvergencia: $f_n$ pontonként konvergens $f$-hez ha $\forall x \in D$ és $\forall \epsilon \gt 0$-hoz $\exists N = N(\epsilon, x)$, melyre $\forall n \gt N$ esetén $|f_n(x)-f(x)|\lt \epsilon$
Egyenletes konvergencia: $f_n$ egyenletesen konvergens $f$-hez ha $\forall \epsilon \gt 0$-hoz $\exists N = N(\epsilon, x)$, melyre $\forall n \gt N$ esetén $|f_n(x)-f(x)|\lt \epsilon, \forall x \in D$-re
Következmény: ha konv egyenletes, akkor pontonkénti is

Elégséges feltétel konvergenciára:
Adottak $f_n, f: D \to \mathbb{R}$ függvények. Tfh $\lim_{n\to \infty}f_n(x)=f(x)$ pontonkénti határérték. Tfh a függvények korlátosak, és $|f_n(x)-f(x)|\gt a_n, \forall x \in D$. Ekkor $\lim_{n\to \infty}a_n=0$ esetén a fenti konvergencia egyenletes.

### 2. Tétel

(a)
Függvénysor: adott $f_1,f_2,f_n, : D \to \mathbb{R}$ fvk, ÉT közös. Ezen függvények végtelen összegét nevezzük függvénysornak. $\sum_{k=0}^\infty f_n=f_0+f_1+\ldots+f_k+\ldots$

**Pontonkénti és egyenletes konvergencia:**
Cauchy kritérium: $\sum f_n$ pontosan akkor konvergens, ha $\forall x \in D$ és $\forall \epsilon \gt 0$-hoz $\exists N = N(\epsilon, x)$, melyre $|\sum_{k=m}^n f_k(x)| \lt \epsilon, \forall n>m>N$
Egyenletes konvergencia: függvénysor konvergenciája egyenletes, ha a részletösszegek sorozata egyenletesen konvergens, azaz $F_n(x) := \sum_{k=1}^n f_k(x)$ jelöléssel $F_n$ egyenletesen konvergál $f$-hez

(b)
Elégséges feltétel függvénysor egyenletes konvergenciára (B):
Adottak az $f_n:D\to \mathbb{R}$ függvények, ÉT közös, tfh a $\sum f_n$ függvénysor tagjai korlátosak, és $f_n$ korlátja $|f_n(x)|<a_n, \forall x \in D$. Tfh $\sum_{n=1}^\infty a_n \lt \infty$. Ekkor a konvergencia egyenletes.

Összegfüggvény folytonossága (B), deriváltja és integrálja.
Összegfv tulajdonság megállapítására: Tfh $f_n:D\to \mathbb{R}$ függvények folytonosak. Tfh soruk egyenletesen konvergens $D$-ben. Ekkor $f=\sum f_n$ is folytonos.

Integrálhatóság: Adottak az $f_n:D\to \mathbb{R}$ integrálható függvények és $f:D\to \mathbb{R}$ függvény. Tfh $\sum_{n=1}^\infty f_n(x)=f(x)$ és a konvergencia egyenletes. Legyen $[\alpha, \beta] \subset D$. Ekkor az összegfüggvény is integrálható: $\int^\beta_\alpha f(x) \,\,dx = \sum_{n=1}^\infty \int^\beta_\alpha f_n(x) \,\,dx$

Deriválhatóság: Adottak az $f_n:D\to \mathbb{R}$ differenciálható függvények és $f:D\to \mathbb{R}$ függvény. Tfh $\sum_{n=1}^\infty f_n(x)=f(x)$ pontonként konvergens $D$-ben. Tfh a deriváltakból álló függvénysor is egyenletesen konvergens: $\sum_{n=1}^\infty f'_n(x)=g(x)$ és $g(x)$ folytonos. Ekkor $f$ diffható, és $f'(x)=g(x)$
(c)
Trigonometrikus sor: adott $a_0, a_1, a_2, \ldots$ illetve $b_0, b_1, b_2,\ldots$ konstansok esetén a formális $a_0+\sum(a_k\cos{kx}+b_k\sin{kx}$ alakú függvénysort.
**Trigonometrikus függvényrendszer**
'ortogonalitása' (B): bármely két függvény skaláris szorzata egyenlő 0-val
