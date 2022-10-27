# LA II. fogalmak

## Lineáris leképezés

Legyenek $V$ és $W$ vektorterek, valamint $u, v \in V , k \in R$
Azt az $L : V \to W$ függvényt, amely a következő két tulajdonsággal rendelkezik, lineáris leképezésnek nevezzük.

1. Vektorok összegének képe a képvektorok összege: $L(u+v)=L(u)+L(v)$
2. Vektor számszorosának képe a vektor képének számszorosa: $L(λu)= λL(u)$
   Ha V=W akkor a leképezést lineáris transzformációnak hívjuk.

## Sajátérték, sajátvektor

A λ komplex szám sajátértéke az $L$ transzformációnak, ha van olyan nem 0 vektor, amelyre $L(x)=λx$
Ez a nem nulla $x$ vektor az $L$ transzformáció $λ$ sajátértékéhez tartozó sajátvektora.
$det(A-λE)=λ^2+1=0$
$Av=\lambda v$
$(A-\lambda E)v=0$

## Komplex konjugált

$a + bi \to a-2i$
A matematikában a **komplex konjugált** egy komplex szám képzetes része előjelének megváltoztatásával képződik.

## Ermitikus mátrix

> Hermitikus mátrix

$\underline{\underline{A}} = \overline{\underline{\underline{A}}}^T$ ha csak valós, $\underline{\underline{A}} =\underline{\underline{A}}^T$, szimmetriuks
Egyenlő a konjugált transzponált mátrixával

Sajátértékei valósak
$A\underline{x}=\lambda\underline{x}\hspace{2cm}|\hspace{1cm}\underline{\overline{x}}^T$ balról
$\underline{\overline{x}}^TA\underline{x}=\underline{\overline{x}}^T\lambda\underline{x}=\lambda\underline{\overline{x}}^T\underline{x}=\lambda\sum_{k=1}^{n}\underline{x}^2_k$

## Ferdén (h)ermitikus mátrix

$\underline{\underline{A}} = -\overline{\underline{\underline{A}}}^T$, ha csak valós $\underline{\underline{A}} = -\underline{\underline{A}}^T$, antiszimmetrikus
Hermitikus, de közben $a_{kk} = \overline{-a_{kk}}$
Főátló nulla, vagy csak komplex tagja van
Így $x_{kk}+y_{kk}i = -(x_{kk}-y_{kk}i)=-x_{kk}+y_{kk}i = 0$

**tétel:** sajátértékei vagy 0, vagy tisztán képzetesek

## Ferdén (h)ermitikus mátrix sajátértékei

A ferdén ermitikus mátrix sajátértékei vagy nullák, vagy (tisztán) képzetesek.

## Unitér mátrix

$\underline{\underline{A}}^{-1}=\overline{\underline{\underline{A}}}^T$, ha csak valós $\underline{\underline{A}}^T =\underline{\underline{A}}^{-1}$, ortogonális
A komplex U unitér mátrix négyzetes mátrix, melynek transzponált konjugáltja (\*-gal jelölve) egyben inverze is.
Az unitér mátrix speciális esete az ortogonális mátrix, melyben csak valós számok szerepelnek.

- $|\lambda|$ 1.
- U invertálható
- $|det(U)| = 1$
- skalárszorzattartó: $⟨Ux,Uy⟩=⟨x,y⟩$, ahol $⟨⋅,⋅⟩$ skalárszorzat
- normatartó: $||Ux||=||x||$
- U oszlopai ortonormált bázist alkotnak
- U sorai ortonormált bázist alkotnak
- a mátrixhoz tartozó lineáris leképezés izometria

## Transzponálás

A transzponálás egy argumentumú művelet. Egy mátrix transzponálása sorainak és oszlopainak a felcserélését jelenti.

## Norma

olyan vektortéren vagy függvénytéren értelmezett $d$ leképezés, ami a nullvektor kivételével a tér minden vektorához egy pozitív számot rendel.

- $d(x)\ge 0$
- $d(x)=0 \iff x=0$
- $d(x+y)\le d(x)+d(y)$
- $d(\lambda x)=|\lambda|d(x)$
  $d(x)$-et az $x$ normájának nevezzük

## Cauchy–Bunyakovszkij–Schwarz-egyenlőtlenség

$|\langle x,y \rangle|^2\le \langle x,x \rangle \cdot \langle y,y \rangle$

**biz**:
$||x||=\sqrt{\langle x,x \rangle}$ norma vezethető be euklideszi terekben
$y=0$ esetben egyenlőség áll fenn, így feltehetően $\langle y,y \rangle$ nem 0
Legyen $\lambda$ tetszőleges valós, vagy komplex szám. Ekkor
$\lambda=\langle x,y \rangle \cdot \langle y,y \rangle^{-1}$

## Hasonló mátrixok

**def:** Az $A$ mátrix hasonló a $D$ mátrixhoz, ha létezik egy olyan $P$ mátrix, amelyre: $D = P^{-1}AP$.
**def:** Az A kvadratikus mátrix diagonalizálható, ha hasonló egy diagonális mátrixhoz.
**def:** Ha az A mátrixra fennáll, hogy $A=S^{-1}BS$ , akkor azt mondjuk, hogy az A mátrix hasonló a B mátrixhoz.
**Tétel:** Hasonló mátrixok sajátértékei megegyeznek.  
**Tétel:** Ha valamely A kvadratikus mátrix sajátértékei mind különbözők, akkor a mátrix diagonalizálható.
**Tétel:** Ha a transzformáció sajátvektorai bázist alkotnak, akkor áttérve e bázisra, a bázistranszformáció eredménye az a diagonális mátrix, melynek főátlójában a sajátértékek állnak. $S^{-1}AS=diag(\lambda_{1},\ldots\lambda_{2},\ldots\lambda_{n})$

Összefoglalva az (n x n)-es A mátrix diagonalizálása:

- A sajátértékek kiszámításához meg kell oldanunk a karakterisztikus egyenletet
  $p(\lambda)=det(A-\lambda I_{n})$
- Ennek gyöktényezős alakját tekintve
  $p(\lambda)=(\lambda-\lambda_{1})^{n_{1}}\cdot(\lambda-\lambda_{2})^{n_{2}}\cdot \ldots \cdot (\lambda-\lambda_{k})^{n_{k}}$
  A $\lambda_{i}$ sajátértékek (lehetnek komplexek is!) algebrai multiplicitása $n_{i}$
- Mindegyik sajátértékhez megkeressük a hozzá tartozó sajátvektor, vagyis megoldjuk a következő egyenletet: $det(A-\lambda I)\underline{x}_{k}$
  Legyen $n_{k}$ a $\lambda_{k}$ sajétértékhez tartozó altér dimenziója, másképpen a sajátérték geometriai multiplicitása. Ha minden sajátérték esetén az algebrai és geometriai multiplicitás azonos, akkor megadható sajátvektorokból álló bázis, és ekkor a mátrix diagonalizálható.

Ha a mátrix diagonalizálható, akkor a hozzáshasonló $D$ diagonális mátrix az alábbi képlettel számolható definíció szerint: $D = S^{-1}AS$,
ahol S a sajátvektorokból, mint oszlopvektorokból álló mátrix. Az D diagonális mátrix diagonálisában a sajátértékek állnak, olyan sorrendben, ahogyan a hozzájuk tartozó sajátvektorokat a mátrixba beírtuk, tehát az i. oszlopban a fődiagonálisban az S mátrix i. oszlopvektorában álló sajátvektort meghatározó sajátérték áll.

## Vektortér

olyan objektumok halmaza, amire teljesülnek

- 0 zárt
- asszociatív
- $\exists 1$
- $\exists 1/x$
- eddig kommutatív
- innen számszoros
  - felcserélhető
  - sorrend nem számít
  - disztributív szorzásra skalárral
  - disztributív szorzásra objektummal

## Altér

**def:** ha a V halmaz egy T test felett vektortér, és $W\subseteq V$ ugyanezen test felett szintén vektortér, akkor W a V altere.

**Tétel:** Legyen V vektortér valamely T test felett, és $W\subseteq V$, W akkor és csak akkor altere V-nek, ha minden
$\underline{v}_1, \underline{v}_2 \in W$ és $\lambda \in T$ –re $v_1+v_2 \in W$ és $\lambda v_1 \in W$
Más szavakkal: a részhalmaz zárt az összeadásra és a számszorosra

**biz:**  
A.) Ha W altér, akkor az állítás a definícióból adódik.
B.) Maradék axiómák $:(-1)\underline{v}\in W$ továbbá: $0=1\underline{v}+\underline{v}^{-1}\in W$

## Mátrix inverze

> Inverz mátrix

A nem invertálható négyzetes mátrixot **szinguláris**nak vagy **degenerált**nak nevezik, ekkor a determináns értéke nulla ($det(A)=0$).
Legyen $A$ egy $n\times n$-es mátrix a $K$ test felett. Ekkor a következő állítások ekvivalensek:
$A$

- invertálható.
- sor-ekvivalens az $I_{n}$ $n\times n$-es egységmátrixhoz
- $n$ pivot eleme van.
- determinánsa nem 0.
- rangja $n$.
- Az $Ax=0$ egyenletnek csak a triviális $x=0$ megoldása van (azaz $Null \underline{(A)} = {0}$)
- Minden $b\in K^{n}$ egyenletnek pontosan egy megoldása van.
- oszlopvektorai lineárisan függetlenek.
- oszlopvektorai kifeszítik $K^{n}$-t.
- oszlopvektorai $K^{n}$ bázisát alkotják.
- Az $x\mapsto Ax$ lineáris leképezés bijekció $K^{n}$-ről $K^{n}$-re.
- Van olyan B![B](https://wikimedia.org/api/rest_v1/media/math/render/svg/47136aad860d145f75f3eed3022df827cee94d7a) n×n![n\times n](https://wikimedia.org/api/rest_v1/media/math/render/svg/59d2b4cb72e304526cf5b5887147729ea259da78)-es mátrix, amire $AB=I_{n}$ teljesül.
- $A^{T}$ transzponáltja invertálható mátrix.
- $A^{T}A$ invertálható mátrix.
- 0 nem sajátértéke

## Mátrix invertálása

> Invertálás mátrixoknál

**Gauss elim:** egységmátrix mellé írjuk, sorok mozgatása, szorozgatás, összeadás
**Analitikus:** $A^{-1}=\frac{(C_{i,j})^{T}}{det(A)}$
ahol $|A|=det(A)$ és $C_{i,j} = adj(A)_{[i,j]}$
**Caley-Hamilton:**
mátrixot beírva a karakterisztikus egyenletbe megoldásként
$det(A-\lambda E)=0$
majd E jobb oldalára kerül, bal oldalon kiemelünk A-t, leosztunk vele, kész

## Adjungált mátrix

$(adj(A))_{ik}=det(A_{ki})$
illetve $Dadj(D)=det(D)\cdot E$

számolás:

- aldeterminánsok számolása
- előjelek sakkolása
- transzponálás / főátlóra tükrözés

## Gauss algoritmus

sorcserekor det -1
szorzas nemnullaval det is megszorzodik
nszeres addicional nem valtozik

## Algebrai multiplicitás

sajatertek k-szoros gyoke
$\lambda^{2}$ multiplicitas 2, det szamolasbol jon
geom <= algebrai

## Bázistranszformáció

E, e eredeti
U, u új
$\underline{x}_{[e]}=\underline{\underline{U}}\underline{x}_{[u]}$

$\underline{x}_{[u]}=\underline{\underline{U}}^{-1}\underline{x}_{[e]}$

## Origó körüli forgatás 30 fok

cos30 | -sin30
sin30 | cos30

## Leképezés báziscseréje

$S=[a_1, a_2]$ eredeti bázisok
$T = [b_{1}, b_{2}]$ képtér bázisok
$A$ leképezés
új mátrix új bázisra pedig $A'=T^{-1}AS$

## Diagonalizálhatóság

**def:** az A mátrix diagonalizálható, ha hasonló egy diagonális mátrixhoz.

**tétel:** Az A kvadratikus mátrix akkor és csak akkor diagonalizálható, ha van sajátvektoraiból álló bázis (bizonyítás a következő oldalakon.)

**tétel:** Az A kvadratikus mátrix sajátvektorai akkor és csak akkor alkotnak bázist, ha a sajátértékek algebrai multiplicitása megegyezik a geometriai multiplicitással, minden sajátérték esetén. (Más szavakkal: valamely A (n x n ) típusú mátrix sajátértékei által meghatározott alterek (az ún. sajátalterek) dimenzióinak összege éppen n, akkor a mátrix diagonalizálható.)

**tétel:** Ha valamely A kvadratikus mátrix sajátértékei mind különbözők, akkor a mátrix diagonalizálható.
**biz:** Különböző sajátértékek esetén a sajátvektorok függetlenek, ezért bázist alkotnak.

**tétel:** Az A mátrix akkor és csak akkor diagonalizálható, ha sajátvektorai bázist alkotnak.
HA az A mátrix diagonalizálható, AKKOR a diagonális mátrix elemei az A nátrix sajátértékei, és S oszlopai az A mátrix sajátvektorai.

$SD=AS$
ahol S sajátvektorokból, D diagonalizált, A mátrix

## Homogén lineáris leképezés

Legyenek V és W vektorterek, valamint $\underline{u},\underline{v} \in V, k \in R$. Azt az $L:V \to W$ függvényt, mely a következő két tulajdonsággal rendelkezik, (homogén) lineárisleképezésnek nevezzük.
vektorok összege képek összege
vektor számszorosának képe a kép számszorosa

## sin szemközti/átfogó

## cos melletti/átfogó

## tg szemközti/melletti

## Caley-Hamilton Tétel

Minden négyzetes mátrix gyöke a karakterisztikus polinomjának.

Helyettesitsuk be $\lambda$ helyere A-t es ki kell jojjon a 0 a karakterisztikus egyenletben (=0)

## Szimmetrikus mátrix $A=A^{T}$

$A=A^{T}$
különböző sajátértékhez tartozó sajátvektorok merőlegesek
emiatt szimmetrikus mátrix sajátvektorai mindig bázist alkotnak
emiatt szimmetrikus mátrix diagonalizálható
emiatt, és mert $D=S^{-1}QS$ (q orto diag, ha S orto) szimmetrikus mátrix diagonalizálható

minden négyzetes mátrix felírható szimm+ferdeszimm összegeként

## Ferdén szimm. mátrix $A=-A^{T}$

$A=-A^{T}$

minden négyzetes mátrix felírható szimm+ferdeszimm összegeként
$A=1/2(A+A^T)+1/2(A-A^T)$

## Ortogonális mátrix $A^{-1}=A^{T}$

$A^{-1}=A^{T}$
pl forgatás
A ortogonális mátrix (jele általában Q) csakis valós számokkal kitöltött unitér mátrix.
Ezekre a mátrixokra igaz, hogy transzponáltja egyben inverze is.
$|det(Q)|=1$
Sajátértékeinek abszolútértéke is 1
Oszlop és sorvektorai ortogonálisak

## Bilineáris függvények

Legyen V vektortér a valós test felett. Az $L^{2}:V\times V \to R$ leképezést bilineáris függvénynek nevezzük, ha L mindkét változójában lineáris
aka: $L(v_1+v_2, v3) = L(v_1, v_3)+L(v_2, v_3)$ mindkét oldalra
$L(\lambda v_1 + v_2) = \lambda L(v_1, v_2)$ mindkét oldalra

Szimmetrikus, ha $v_1, v_2$ felcserélhető paraméterek

**def:** az $L^{2}:V\times V \to R$ bilineáris függvénynek a [b]=b*1,\ldotsb_n bázis szerinti L mátrixán azt az $n\times n$ mátrixot értjük, melyben i. sor j. eleme $l*{i,j}=L(b_i, b_j)$

**tétel:** ha $L^{2}:V\times V \to R$ bilineáris függvény, akkor $L^{2}(\underline{x},\underline{y})=\underline{x}^{T}\underline{\underline{L}}\underline{y}$ és L a függvény mátrixa

## Kvadratikus alak

Legyen a V vektortér a valós test felett, és az $L^2 : V \times V\to R$ leképzés szimmetrikus bilineáris függvény.
A $Q : V\to R$ függvény, ahol $Q(x)\coloneqq L^2(x,x)$, az $L^2$ kvadratikus alakja. Szokás Q-t röviden, $L^2$ említése nélkül is kvadratikus alaknak nevezni.
$Q(x)=x^{T}Ax$
itt $A$ szimmetrikus mátrix

## Szimm. mátrix és kvad diagonaliz

> Diagonalizálás szimm, kvad

$x_{[e]}=Ux_{[u]}$
$D=S^{-1}QS$
$Q=SDS^{-1}$

## Spektrál Tétel

Valamely négyzetes mátrix akkor és csak akkor diagonalizálható ortogonálisan, ha szimmetrikus.

## Definitség

> Kvadratikus osztályozása

$Q(x)=x^TQx=u^TDu=\sum\lambda_i u^2_i$

Ha $A$ szimmetrikus (négyzetes) mátrix, akkor a hozzá tartozó $x^TAx$ kvadratikus alak

- acsa pozitív definit ha minden sé pozitív
- acsa negatív definit ha minden sé negatív
- acsa indefinit, ha van poz és neg is

Q

- pozitív def ha Q(x) > 0 minden nemnull x-re
- negatív def ha Q(x) > 0 minden nemnull x-re
  szemi, ha kivesszük a nemnullt

determináns teszt: bal felső négyzetek aldeterminánsai mind pozitívak

## Mátrix definitsége

poz neg definit, ha a hozzá tartozó kvadratikus alak poz neg definit

## Főtengely Tétel

A $Q=x^TQx$ kvadratikus alakhoz tekintsünk $S$ ortogonális transzformációt, amelynek S mátixában az oszlopok a Q szimm mátrix ortonormált sajátvektorai. Áttérve ezen ortonormált svk bázisára, vagyis $x=Su$ transzform, a Q így írható le
$Q=x^TQx=u^TDu=\sum \lambda_i u_i^2$
ahol $\lambda$-k az A sajátértékei. Ezt a transzformációt főtengely transzformációnak nevezzük

## Főtengelyek

$Q=x^TQx=u^TDu$ kvadratikus alak Q nxn-es szimm. mátrixának n különböző sajátértékéhez tartozó sajátaltereit a Q kvadratikus alak főtengelyeinek nevezzük. 2d-ben a megfelelő kúpszelet szimmetria tengelyei a főtengelyek

## Ortonormált sajátvektor

3 x 3 mátrix esetében, ha egyik sajátérték algebrai multiplicitása nagyobb mint egy, akkor a sajátaltér ortonormált bázisvektorait úgy kapjuk meg, hogy egyik bázisvektort felírjuk a másikkal párhuzamos, és arra merőleges öszetevőkkel, és ezen új vektorok alkotják az altér ortogonális bázisát.

Utána normáljuk.

## Kommutatív csoport

> IKEA

inverz - van inverz az egységelemre, vagyis ellentett $a\circ x=e$ 0nak nem kell
kommutatív - a b = b a
egységelem - vele művelet visszaadja a másik oldalt $a\circ e=a$
asszociatív - osszevissza zarojelezgeto

## Szorzás

$(a,b),(c,d)\in C: (a,b)\cdot(c,d)=(ac-bd,ad+bc)\in C$
kommutativ, mert felcserelheto
asszoc mert zarojelezheto
egysegelem $(1,0)$
inverz $(a, b) \circ (x, y) = (1,0)$ megoldásai

szorzas disztributiv az osszeadasra

## Komplex számolása

nevezőt a konjugált/konjugálttal beszorozni

## Komplex abszolútértéke

$|x|=\sqrt{a^2+b^2}=\sqrt{z\overline{z}}$

## Komplex trigonometrikus alakja

$r=\sqrt{a^2+b^2}, \varphi = arctg(b/a)$

így: $z=r(cos\varphi+isin\varphi)$

## Nevezetes szögfüggvény értékek

$0000;30;45;60$
$sin;1/2;\sqrt{2}/2;\sqrt{3}/2$
$cos$ forditva 45re
$tg;\sqrt{3}/3;1;\sqrt{3}$
$ctg$: visszafele

## Komplex hatványozása

> Moivre képlet

A trigonometriai alakban adott $z=r(cos\varphi+isin\varphi)$ komplex szám k-ik hatványa $z^k=r^k(cosk\varphi+isink\varphi)$ ahol k tetszőleges egész

## Komplex osztása

$z_1/z_2=r_1/r_2(cos(\varphi_1-\varphi_2)+isin(\varphi_1-\varphi_2))$
$\overline{z}=r(cos(-\varphi)+isin(-\varphi)$
$1/z=1/r(cos(-\varphi)+isin(-\varphi))$

## Komplex gyökvonás

A $w^n-z=0$ binom EGYENLET megoldásait a $z$ komplex szám $n$-ik gyökeinek nevezzük. A gyökökre teljesül: $w^n=z$

A trigonometriai alakban felírt $z=r(cos\varphi+isin\varphi)$ komplex szám összes n-ik gyöke az
$\sqrt[n]{z}=\sqrt[n]{r}(cos((\varphi+2k\pi)/n))+isin((\varphi+2k\pi)/n)(k=0,1,\ldots,n-1)$
alakban felírt n darab szám, nem függvény!

jelentés: $\sqrt[n]{|z|}$ sugarú körön szabályos n-szög csúcsai

## Másodfokú komplexben

$D = b^2-4ac$ diszkriminans, ez van gyok alatt a masodfoku megoldoban

ha D>0 akkor 2 kul valos gyok
ha D=0 akkor 1 valos kétszeres gyök
ha D<0 akkor 2 komplex (konj, ha együtthatók valósak) gyök

## Gyöktényezős alak

> Polinom gyöktényezős alakja

$f=a_n x^n + \ldots a_1 x + a_0 \in T[x]$ polinom felbontásánál a gyököket (=0 megoldásait) rendre multiplicitás szerint beírogatjuk levonva xből az $a_n$-re
$f=a_n(x-c_1)(x-c_2)\ldots(x-c_n)$

## Egységgyökök

A z=1 speciális esetben elvégzett gyökvonás eredményét, azaz az $x^n-1=0$ binom egzenlet megoldásait n-ik (komplex) egységgyököknek nevezzük.

## Egységgyökök előállítása

$\epsilon_1=cos(2\pi/n)+isin(2\pi/n)$ hatványaiként előállnak, azaz az összes n-ik egységgyök a következő (egy szabályos n-szög csúcsai az egységkörön, melynek egyik csúcsa a z=1)

Definíció: Egy n-ik egységgyök primitív n-ik egységgyök, ha hatványaiként az összes többi egységgyök előáll.

## Egységgyökök összege

Az n-edik egységgyökök (n>1) összege (az összesé) nulla.
**biz:**
Legyen $\epsilon$ primitív egységgyök ekkor $\epsilon \neq 1$. Az egységgyökök összege:

$1+ \epsilon + \epsilon^2 +\ldots+ \epsilon^{n-1}=(\epsilon^{n-1})/(\epsilon-1)=(1-1)/(\epsilon-1)=0$

## Egységgyökök struktúrája

Az n. egységgyökök kommutatív csoportot alkotnak a komplex számok szokásos szorzására nézve.
**biz:**
zárt: $(\epsilon_k\epsilon_i)^n]=(cos(k+l)2\pi/n+isin(k+l)2\pi/n)^n = cos(k+l)n2\pi/n+isin(k+l)n2\pi/n=1$
egység:
$1=1(cos(0/n)+i sin(0/n))$
inverz:
$\epsilon_k\epsilon_j=1(cos(0/n)+isin(0/n))$
$(k2\pi/n)+(j2\pi/n)=n2\pi/n$ ahonnan $j=n-k$
$\epsilon_k$ inverze $\epsilon_k^{-1}=\epsilon_{n-k}$

## Skalárszorzat

számszoros, pl $5\times vektor$
4 tulajdonsággal definiált, két vektorváltozós, valósba képző függvény
pl $|a|\cdot|b|\cdot cos\alpha$

tul:

- poz definit $a\cdot a\geq 0$, $a\cdot a=0 \leftrightarrow a=0$
- szimmetrikus $a\cdot b = b\cdot a$
- homogén $(\lambda a)\cdot b=\lambda a \cdot b$
- lineáris $a\cdot (b+c) = a\cdot b+a\cdot c$

## Skalárszorzat általános vektorterekben

$s(x,y)=\langle x,y \rangle$ skalárszorzat, ha

- poz definit $\forall a\in V |\space \langle a, a\rangle \geq 0$, $\langle a, a\rangle =0 \leftrightarrow a=0$
- szimmetrikus $\forall a, b\in V |\space \langle a, b\rangle = \langle b, a\rangle$
- homogén $\forall a, b\in V \forall\lambda\in R|\space \langle\lambda a, b\rangle=\lambda \langle a, b\rangle$
- lineáris $\forall a,b,c\in V |\space \langle a+b, c \rangle = \langle a, c \rangle + \langle b, c \rangle$

## Skalárszorzat komplexen

$s(x,y)=\langle x,y \rangle$ skalárszorzat, ha

- poz definit $\forall a\in V |\space \langle a, a\rangle \geq 0$, $\langle a, a\rangle =0 \leftrightarrow a=0$
- szimmetrikus $\forall a, b\in V |\space \langle a, b\rangle = \langle \overline{b, a}\rangle$ (konjugalt b,a)
- homogén $\forall a, b\in V \forall\lambda\in R|\space \langle\lambda a, b\rangle=\overline{\lambda} \langle a, b\rangle$
- lineáris $\forall a,b,c\in V |\space \langle a+b, c \rangle = \langle a, c \rangle + \langle b, c \rangle$
  $\langle x,y \rangle=\overline{x}^Ty$

## Skalárszorzat $\sum x_i y_i$

> Véges dimenziójú, euklidészivé tehető

**tétel:** minden véges dimenziójú vektortér euklideszivé tehető
**biz:** konstruktív, konkrét fv $\sum x_i y_i$

- poz definit $\forall a\in V |\space \langle a, a\rangle \geq 0$, $\langle a, a\rangle =0 \leftrightarrow a=0$
- szimmetrikus $\forall a, b\in V |\space \langle a, b\rangle = \langle b, a\rangle$
- homogén $\forall a, b\in V \forall\lambda\in R|\space \langle\lambda a, b\rangle=\lambda \langle a, b\rangle$
- lineáris $\forall a,b,c\in V |\space \langle a+b, c \rangle = \langle a, c \rangle + \langle b, c \rangle$

hol jó?
pl V legyen max 2foku polinomok tere, $P_2$ , egy bázisa $B=(x^2, x, 1)$

$p^1(x)=a_1x^2+a_2x+a_3\cdot 1=a_1b_1+a_2b_2+a_3b_3=[a_1 a_2 a_3][B]$
$p^2(x)=c_1x^2+c_2x+c_3\cdot 1=c_1b_1+c_2b_2+c_3b_3=[c_1 c_2 c_3][B]$

$\langle p^1, p^2 \rangle=\sum_{i=1}^3a_ic_i=a_1c_1+a_2c_2+a_3c_3$

V legyen 2x2 valós elemű, felső háromszög alakú mátrixok tere
$M=\lbrace(a,b;0,d), a,b,d\in R\rbrace$
$B=\lbrace [1,0;0,0],[0,1;0,0],[0,0;0,1]=\lbrace b_1,b_2,b_3 \rbrace$
$A= \ldots = [a_1 a_2 a_3]$
$B= \ldots = [b_1 b_2 b_3]$
$\langle A, C \rangle=\sum_{i=1}^3a_ic_i=a_1c_1+a_2c_2+a_3c_3$

$\langle a,c\rangle=a_T\cdot c=\sum_{i=1}^3a_ic_i=a_1c_1+a_2c_2+a_3c_3$
ahol $\cdot$ a szokásos mátrix szorzás

## Norma

$n: H\to R^+\cup\lbrace 0 \rbrace$ fv norma, amire teljesulnek:
$||\underline{x}||=0 \leftrightarrow x=0$
$||\alpha\underline{x}||=|\alpha|||\underline{x}||$
$||\underline{x}+\underline{y}||\geq ||\underline{x}||+||\underline{y}||$ trig egyenlotlenseg

norma pl $||z||\coloneqq \sqrt{\langle z,z \rangle}$
teljesul mert CBS is igaz nulla kivetelevel

## Komplex vektorok "szöge"

ortok, ha skalár szorzatuk 0

## Komplex vektorok "távolsága"

Metrika: $HxH\to R^+\cup \lbrace 0 \rbrace$ fv

- $m(x,y)=0 \leftrightarrow x=y$
- $m(x,y)=m(x,y)$ - szimmetria
- $m(x,y)=0 \leq m(x,y)+m(x,y)$ trig egylség

$m(x,y)\coloneqq ||x-y||=\sqrt{\langle x-y, x-y \rangle} = \sqrt{\overline{(x-y)}^{-T}(x-y)}=\sqrt{\sum|x_i-y_i|^2}$

## Speciális transzformációk

> Mátrix táblázat

valós ; komplex ; sé; egyéb
szimm; emiriti; valos; sv orto, diagonalizalhato
fszimm; femirit; 0, kepzetes; ha A emir akkor iA ferdemir
orto; uniter; absz 1; norma, tavtarto, det abs 1, oszlopok sorok orto
