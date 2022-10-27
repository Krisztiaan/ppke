# DM II. fogalmak

## Univerzum

nemüres halmaz, a változók (x, y) ennek elemein futnak végig, ezek az individuumváltozók

## Prédikátum

az univerzum elemei között kapcsolatot, relációt fejez ki
pl: $P(x,y)$ jelentse hogy $x<y$
prefix jelöléssel $< x, y \to P(x,y) \lor Pxy$

### Elsőrendű logika szintaxisa

Változó szimbólumok: $x, y, z$
Konstans szimbólumok: $a, b, c$
Prédikátum szimbólumok (állítás): $P, Q, S$
Függvény szimbólumok: $f, g$
Logikai összekötők (műveleti jelek): $\land \lor \neg \to \implies$
Kvantorok: $\forall \space \exists \space \exists! \space \nexists$
Zárójelek: $(,)$

### Kvantorok hatásköre

$\exists x P(x,y) \lor Q(x)$
$x$ kötött a kvantor mögött, vagy a kvantor mögötti formulában
$x$ szabad $Q(x)$-ben
**Zárt formula**: mondat, minden változó kötött

### Formulaképzés szabályai

Kifejezés: individumváltozók + konstansok

### Atomi formulák

Ha a $P$ "n" argumentumú prédikátum szimbólum, és $t_1, t_2, \ldots, t_n$ termek, akkor $P(t_1, t_2, \ldots, t_n)$ atomi formula. A nulla argumentumos prédikátum szimbólumot az ítéletváltozóknak feleltetünk meg. Így az elsőrendű logika a nulladrendű kiterjesztése.

## De Morgan azonosságok

$\neg (a \land b) = \neg a \lor \neg b$
$\neg (a \lor b) = \neg a \land \neg b$

$a \land b = \neg (\neg a \lor \neg b)$
$a \lor b = a \lor b$
$a \implies b = \neg a \lor b$
$a \iff b = (a \land b) \lor (\neg a \land \neg b)$

$\neg\forall x P(x) \equiv \exists x \neg P(x)$ -> Nem minden $x$-re igaz $P(x)$ ekvivalens azzal, hogy létezik $x$ amire nem igaz $P(x)$
$\neg \exists xP(x)\equiv \forall x \neg P(x)$ -> Nem létezik $x$ amire igaz $P(x)$ ekviv minden $x$-re nem igaz $P(x)$
$\neg \exists x\neg P(x)\equiv \forall xP(x)$ -> Előbbi, csak negált P-vel
$\neg \forall x \neg P(x) \equiv \exists xP(x)$ -> Nem minden $x$-re nem $P(x)$ akkor létezik $x$ hogy $P(x)$

## Disztributív szabályok

$(p \lor q) \land r \equiv (p \land r) \lor (q \land r)$
$(p \land q) \lor r \equiv (p \lor r) \land (q \lor r)$

## Érvényes formula

> Nulladrendi tautológia

Minden interpretáció minden értékadására igaz.
pl: piros seggű páviánokon vizsgáljuk hogy piros-e a segge

## Azonosan hamis formula

Minden interpretáció minden értékadására hamis.
pl: piros seggű páviánokon vizsgáljuk hogy delfinek-e

## Mondat

Zárt formula, minden változó kvantált, ami azt jelenti, igazságértéke csak az interpretációtól függ

## Konjunktív normálforma

> KLÓZ alak

**Konjuntív normálforma:** olyan formula, amiben csak $\neg, \lor, \land$ operátorok vannak

> A prenex formába való átírás algoritmusa

- A logikai összekötőjelek átírása $\neg, \land, \lor$-ra
- A De Morgan szabályok alkalmazása addig, amíg a $\neg$ hatásköre atomi formula nem lesz
- A változók standardizálása (kvantoronkénti átnevezése)
  - pl $\forall x(P(x)\lor \exists xQ(x))$ formulából $\forall x(P(x)\lor \exists y Q(y)$
- A kvantorkiemelési szabályok alkalmazása, amíg minden kvantor a formula elejére nem kerül
- A kvantorok, és őket követő változók sorrendjét meg kell tartani
- A formula konjunktív normálformára hozása disztributív szabályok alkalmazásával

## Skólemizálás

> Prenex

Egzisztenciális kvantorok kiküszöbölése
x -> f(x) ek átírása
Konjuktív normálformára írás
Átnevezések

## Konjukció $\land$

$\land$

## Rezolúció

- Skólemnormálforma
- Klózhalmaz ($\land$)
- Unifikáció (egymás alá klózok nélkül)
- Rezolválás (csík huzi)
- nil / mindig logikai köv
  **Helyes**: rezolvensek következmények
  **teljes**: ha kontradikció a formula, levezethető az üres halmaz

## Szitaformula

$\lvert A \cup B \cup C \rvert = \lvert A\rvert + \lvert B \rvert + \lvert C\rvert - \lvert A\cap B\rvert - \lvert A \cap C\rvert - \lvert B\cap C\rvert + \lvert A\cap B\cap C\rvert$

## Egyszerű gráf

nemüres V csúcsok, pontok halmaza
különböző elemekkel rendelkező, és különböző rendezetlen párokból álló élek halmaza
nincs többszörös él, se hurok

## Multigráf

nemüres V csúcsok/pontok halmaza,  
E élek halmaza,  
$f$ függvény: $E \to \{\{u,v\}|u,v\in V,u\neq v\}$
Az él többszörös, ha $f(e_1)=f(e_2)$.

## Pszeudo gráf

nemüres V csúcsok, pontok halmaza,
E élek halmaza -hurokél

## Irányítatlan gráf

A v pont fokszáma, foka, a rá illeszkedő élek darabszáma, $deg(v)$ vagy $fok(v)$

## K-reguláris gráf

minden pontjának foka $k$

## Irányított gráf

nemüres V csúcsok, pontok halmaza,
E rendezett, különböző pontPÁROK halmaza
befok, kifok: végpont, kezdőpont

## Gráf

Egy irányítatlan gráf $G=(V, E)$
csúcsok egy $V / V(G)$ **nemüres** halmazából,
élek egy $E / E(G)$ halmazából és
egy $f$ függvényből áll, amely minden egyes $a\in E$ élnek egy $(u, v)=(v, u)$ **rendezetlen párt** feleltet meg, ahol $u, v \in V$ pontok az él végpontjai
**Irányított** gráf, ha az $f: E \to V \times V$, vagyis $f$ az élekhez **rendezett** $(u, v)$ párokat rendel

## Fokszámsorozat

**def**: G gráf fokszámsorozata pontjai fokszámának nagyság szerint rendezett felsorolása
**def**: adott $d_1\leq d_2\leq \ldots \leq d_k$ fokszámsorozat realizálható a G gráffal, ha a G-nek ez éppen a fokszámsorozata (a fokszámsorozat **realizálható**)

## Teljes gráf

minden pont között van él
$K_5$ - Kuratowski gráf

## Teljes gráf élszáma

Az $n$ csúcsú teljes gráf éleinek száma $\binom{n}{2} = \frac{n\cdot (n-1)}{2}$

## Páros gráf

**def**: G páros gráf, ha csúcsai két olyan osztályba csoportosíthatók, melyekre igaz, hogy csak a különböző osztályokban lévő csúcsok között lehet él.
**jel**: $G_{m,n}$ egyik osztályban m, másikban n csúcs van
$K_{m,n}$ egyik osztályban minden csúcs össze van kötve másik ösztályban mindennel
$K_{3,3}$ Kuratowski gráf

## Izomorf gráfok

két gráf izomorf, ha egyikük pontjai és élei kölcsönösen egyértelmű és illeszkedéstartó módon megfeleltethetők a másikuk pontjainak, illetve éleinek
**invariáns**: megegyezik pontok és élek száma, fokszámsorozat, körök száma és hossza

## Kézfogási Tétel

minden irányítatlan gráfban a fokszámok összege az élek számának kétszeresével egyenlő
**biz**: bárhogy húzunk élet, +2 fok
**következmény**: irányítatlan gráfokban a páratlan fokszámú pontok száma páros
**biz**: az n db páros fokszámú pontra $2k_1+2k_2+\ldots+2k_n=2(k_1+k_2+\ldots+k_n) \to$ páros
az m db páratlan fokszámú pontra $(2l_1+1)+(2l_2+1)+\ldots.+(2l_m+1)=2(l_1+l_2+\ldots.+l_m)+1+1+\ldots+1=2(l_1+l_2+\ldots.+l_m)+m$
tudjuk hogy $2|E|=$ párosak + páratlanok összege
$2|E|= 2(k_1+k_2+\ldots.+k_n)+2(l_1+l_2+\ldots.+l_m)+m$
csak akkor marad páros, ha $m$ is páros, ami a páratlan pontok száma

## Kézfogási tétel irG

minden irányított gráfban a fokszámok összegére igaz, hogy a befokok összege megegyezik a kifokok összegével

## Részgráf

Egy $G*$ gráfot a $G$ részgráfjának nevezünk, ha $G*$ csak $G$-beli pontokat és éleket tartalmaz.
Ha $G*$ nem azonos $G$-vel, akkor a $G$ gráf valódi részgráfjának nevezzük.

## Élsorozat

élsorozatnak az élek olyan rendezett halmazát nevezzük, amely a következő tulajdonságokkal rendelkezik:

- első és utolsó éltől eltekintve bármely él egyik végpontja előző élhez, másik a következőhöz illeszkedik
- első él végpontja a következőhöz ill., másik a sorozat kezdőpontja
- utolsó él fordítva
- minden él pontosan egyszer fordul elő

### Nyílt élsorozat

kezdő és végpont nem egyezik

## Zárt élsorozat

kezdő és végpont egyezik

### Út, kör hossza

benne lévő élek száma

## Séta

csúcsok többször is szerepelhetnek az élsorozatban

## Összefüggő gráf

Ha egy gráfban bármely két pont úttal elérhető, akkor a gráfot összefüggőnek nevezzük.
Azt mondjuk, hogy egy gráf A és B csúcsa relációban áll egymással, ha van köztük út.
Bizonyítható, hogy ez ekvivalencia reláció.
Ezen ekvivalencia reláció egy osztályba tartozó csúcsai a gráf (összefüggő) komponensei.

## Euler út, kör, gráf

út: séta, kör: zárt séta
G gráfban **Euler-út**nak nevezünk egy olyan élsorozatot, amely G összes élét pontosan egyszer tartalmazza. Ha ez az élsorozat zárt, akkor **Euler-kör**.

Ha egy gráfban van Euler-kör, akkor azt **Euler gráf**nak nevezzük

Így minden Euler-kör Euler-út is

## Euler út, kör $\exists$

G-ben acsa van Euler kör, ha minden pontjának fokszáma páros, ekkor Euler gráfnak hívjuk
G-ben acsa van Euler út, ha pontosan két páratlan fokszámú pontja van, a többi pontja páros fokszámú (NEM Euler gráf)

## Azonos fokú csúcsok

Minden 1-nél több csúcsú egyszerű gráfban van két azonos fokú csúcs.
**biz**: az n csúcsú gráf lehetséges fokszámai: $0, 1, 2\ldots n-1$
$0$ és $n-1$ nem lehet egyszerre
Próbáljuk meg egyenletesen elosztani a fokszámokat a csúcsok között: $n$ csúcs van és $n-1$ db fokszám: viszont kettőnek egyenlőnek kellene lenni!

## Összefüggő G éleinek száma

Ha egy gráfban bármely két pont úttal elérhető, akkor a gráfot összefüggőnek nevezzük.
Az n pontú összefüggő gráfnak legalább $n - 1$ éle van.
**biz**: a csúcsok számára vonatkozó teljes indukció
Ha a G n pontú gráfnak van elsőfokú pontja:
akkor a hozzátartozó éllel együtt töröljük a gráfból  
n-1 pontú összefüggő gráfot kapunk, melyre érvényes az indukciós feltétel:
n-1 csúcsa és legalább n-2 éle van  
A törölt élt és pontot visszavéve adódik, hogy G-nek minimum n éle van.
Ha nincs elsőfokú pontja, akkor minden pont foka legalább 2, és így a fokszámok összege minimum $2(n+1) > n$

## Összefüggő G-ben kör

Ha egy n pontú gráfnak legalább n éle van, akkor van benne kör.
**biz**: csúcsok számára TI
Az állítás n = 1 esetén nyilvánvalóan igaz.  
Tegyük fel, hogy az n pontú és legalább n élű gráfban van kör.  
Legyen G egy n + 1 pontú gráf, amelynek legalább n + 1 éle van.  
Ha van elsőfokú pontja, töröljük a rá illeszkedő éllel együtt.  
A maradék gráfban az indukciós feltétel szerint van kör.  
Visszavéve az elsőfokú pontot és a rá illeszkedő élet, az előző kört uu. tartalmazza a kapott gráf.
Ha nincs elsőfokú pontja, akkor minden pont legalább másodfokú.  
Ekkor az előző tétel szerint van a gráfban kör.

## Fa, éleinek száma

Ha egy gráf összefüggő és nem tartalmaz kört, akkor fagráfnak vagy röviden fának nevezzük.

Tétel: Az n pontú fagráf éleinek száma n - 1.  
Bizonyítás 1: _Összefüggő G-ben kör_
indirekt: kör egy élének törlése milyen hatással van az összefüggőségre – ha lenne benne kör, egy élét törölve mi lesz a helyzet

**def**: a fa összefüggő körmentes gráf
Egy összefüggő gráf akkor és csak akkor fa, ha bármely két pontja között pontosan egy út van.
az n pontú, n-1 élú összefüggő gráf fa.

## Prüfer-kód

- Prüfer-kód: n csúcsú fa ↔ n-2 db szám
- Minden szám 1 és n közötti lehet
- Kölcsönösen egyértelmű: n csúcsú fák ↔ n-2 hosszú sorozatok
- Tétel (Cayley): $T(n)=n^{n-2}$

## Prüfer-kód Gból

- Bemenet egy számozott fa (csúcsait az 1, 2, \ldots, *n* számokkal címkézzük meg)
- Végezzük el az alábbiakat mindaddig, amíg egyetlen él marad

- válasszuk ki a legkisebb számú _levelet_ (= fokszáma 1),
- írjuk ki a vele szomszédos csúcs számát,
- töröljük a fából a kiválasztott csúcsot (természetesen a hozzáilleszkedő éllel együtt).

- Az eredményül kapott számok a kiírás sorrendjében képezik a Prüfer-kódot.

## Prüfer-kódból G

- Bemenet: egy *n-2* elemű Prüfer-kód, amelyhez hozzáadjuk az *n* értéket utolsónak.
- Végezzük el *n-1*-szer a következőket:
- meghatározzuk azt a legkisebb pozitív természetes számot amelyikhez még nem húztunk élt és nem eleme a sorozatnak
- kössük össze egy éllel az ezzel a számmal jelölt csúcsot a sorozat első elemével,
- töröljük a sorozat első elmét **ez után újra jöhet a törölt szám!**

## Részgráf

R gráf G részgráfja, ha R megkapható G-ből pontok és élek elhagyásával

## Feszítő részgráf, fa

részgráf: R, ha G minden pontját tartalmazza, G-ből csak élek hiányoznak
fa: az R minden pontját tartalmazó fa

## Kruskal algoritmus

Élenként építjük a gráfot
Olyan élet választunk, ami a nem választottak közül legkisebb élsúlyú
Ha nem alkot kört eddigiekkel, jöhet
Fának n-1 éle van, n-1 elérésénél abbahagyjuk

## Prim algoritmus

Élenként építjük a gráfot
Olyan élet választunk, ami a nem választottak közül legkisebb élsúlyú, és az eddig kiválasztottakkal összefüggőt alkoz
Ha nem alkot kört eddigiekkel, jöhet
Fának n-1 éle van, n-1 elérésénél abbahagyjuk

## Gráf típusok

_Típus & Élek & Többsz. él & hurok_
**Egyszerű** & irtlan & nem & nem
**Multi** & irtlan & igen & nem
**Irányított** & irnyit & nem & igen
**IrMulti** & ir & igen & igen

## Illeszked./inciden. mátrix

G irányított gráf, n ponton e éllel. Az $n \times e$ –es $B(G)$ mátrixot a $G$ gráf illeszkedési mátrixának nevezzük, ha
$b_{i,j}= 0, 1, -1$ ahol
0: ha j-ik él nem illeszkedik az i-ik ponthoz
1: ha j-ik él kezdőpontja az i-ik pont
-1: ha j-ik él végpontja az i-ik pont

## Dijkstra

kezdőcsúcs szomszédaira ideiglenes címke súllyal
legalacsonyabb súly a következő, onnan ugyanez, ha kell, javítás
stb.

## Síkgráfok

Egy gráf síkgráf=síkba rajzolható gráf, ha lerajzolható úgy a síkba, hogy élei csak a gráf csúcsaiban metszik egymást.
A síkot tartományokra bontja

## Euler poliéder Tétel

A G összefüggő, egyszerű síkgráf esetében
$p-e+t=2$
ahol
$p$ = gráf pontjainak (csúcsainak) száma,  
$e$ = gráf éleinek száma,  
$t$ = a sík gráf által létrehozott területeinek száma, a végtelen területet is számolva

következmény: $e\leq 3p-6$ ha min 3 pontú a gráf

A G összefüggő, egyszerű síkgráf esetében, ha p=csúcsszám, e=élszám, t=síkban a gráf által felosztott területek száma (külsővel együtt), akkor: $p-e+t=2$
**biz**: a(z adott síkgráfot)gráfot lépésenként (újra) lerajzoljuk, mindig úgy, hogy a lerajzolás során összefüggő maradjon:

1. lépés: 1 csúcs, igaz (1-0+1=2)
2. lépés: 2 csúcs, 1 él, 1 tart. igaz
   n. lépés: tfh n-1 lépésig igaz a formula, a következő kétféle lehet
   a. új csúcs, rá ill. éllel együtt, aminek szomszédja már lerajzolva, élnek másik végpontja, él++, csúcs++, terület marad, igaz így? $p-e+t\leftrightarrow (p+1)-(e+1)+t=2$
   b. új él, így t++ él++, innen $p-e+t\leftrightarrow p-(e+1)+(t+1)=2$

### Euler p.tétel következményei

$e\leq 3p-6$ ha min 3 pontú a gráf
$e\leq 2p-4$ ha min 3 pontú a gráf, és nincs 3 hosszú köre
Ha összefüggő, egyszerű síkba rajzolható gráf, akkor a minimális fokszáma legfeljebb 5.

## Kuratowski-Tétel

Valamely gráf akkor és csak akkor sík gráf, ha nem tartalmaz K5-tel vagy K3,3-mal izomorf/homeomorf részgráfot.
biz: Euler tétel miatt megdőlnek

## Fáry-Wagner tétel

Ha egy síkba rajzolható gráf, akkor léteik olyan síkbarajzolása, amelyben minden él egyenes szakasz.

## Homeomorf

élre szabad pontot beiktatni. Ha a gráfnak van olyan részgráfja, amelyben minden pont foka kettő, de nem kör, ezeket a pontokat szabad törölni: uv élből uw, wv élek keletkezhetnek, és fordítva (u, v, w pontok)

## Szabályos test

Szabályos test: konvex poliéder, amelynek élei, élszögei és lapszögei is egyenlők.
szabályos poliéder:
pk=2e
tn=2e
min fokszám max 5
ha van 5 min fokszámú csúcs, akkor még van 11
csak 5 szabályos poliéder van

## Konvex poliéder

Az olyan poliédert (térbeli testet), amelynek oldallapjai konvex sokszögek, konvex poliédernek nevezzük.

## Sztereografikus projekció

Egy gráf pontosan akkor síkbarajzolható, ha gömbre rajzolható.
**biz**: Sztereografikus projekció. A gömböt a síkra helyezzük, (déli pólus), majd az északi pólusból egyeneseket húzunk a gráf pontjaihoz (éleinek pontjaihoz), ezen egyeneseknek a gömbbel levő másik metszéspontja lesz a vetített képpont.

## Gömbre $\leftrightarrow$ síkbarajzolható

ennyi

## Hamilton út, kör

A G gráf egy H útját Hamilton-útnak mondjuk, ha a csúcsok mind különbözők és e csúcspontokon kívül más csúcspontja nincs G-nek.
A G gráf K körét Hamilton-körnek mondjuk, ha K tartalmazza G minden csúcspontját.

biztos van: teljes gráf, kör

**tétel**: Ha a G n pontú egyszerű gráf minden pontjának foka legalább n/2, akkor a G összefüggő – később: H-gráf!

**biz**: Legyen u és v két különböző csúcsa G-nek. A feltétel szerint u-val és v-vel is legalább n/2, n/2 pont van összekötve az u-ból illetve v-ből induló élek által, a fokszám feltétel miatt. Az előbb említett u-val, illetve v-vel közvetlenül összekötött pontok között van olyan, mely u-val is v-vel is össze van kötve, (ha nem lenne ilyen akkor G csúcsainak a száma nagyobb egyenlő volna, mint $[n/2+n/2+2]$) azaz u és v között vezet út.

## Ore Tétel

Elégséges feltétel Hamilton kör létezésére
$\delta(u)+\delta(v)\geq n$

**biz**:

- indirekt tfh. $\exists$ olyan gráf, amely teljesíti a felételt és nincs H-köre
- a csúcsok megtartásával vegyünk éleket a gráfhoz mindaddig, amíg egy Hamilton kör keletkezik
- az utolsó u,v él elhagyásával H-út van, ez látható fekete vonallal az ábrán
  $u\to v_1 \to v_2 \to \ldots \to v_k \to v_{k+1} \to \ldots \to v$
  $u \to v$ nem létezhet mert akkor lenne H-kör
  $u$ szomszédai nem lehetnek $v$ szomszédainak szomszédai
  becslés $u$ fokszámára $\delta(u)\leq (n-1)-\delta(v)$
  ahol $\delta(v)$ v szomszédai, nincs hurokél, így $n-1$ az összes fokszám

## Dirac Tétel

Ha az n=2k csúcspontú egyszerű G gráf bármely pontjának a foka legalább k, akkor van G-nek Hamilton-köre.
**biz**: valóban G-ben létezik Hamilton-kör, mivel az ORE tétel feltételei teljesülnek

## Pósa Lajos tétele

Legyenek az n csúcsú G egyszerű gráf csúcsai fokszám szerint rendezve,
Ha minden $k\lt n/2$-re teljesül hogy $\delta(u_k)\geq k+1$ akkor van G-ben Hami kör

## Kromatikus szám

χ(G) a gráf ún. kromatikus száma az a szám, ahány szín legalább kell (χ(G)-1 db szín nem elegendő) a G gráf csúcsainak olyan kiszínezéséhez, hogy a szomszédok más színűek legyenek. Az azonos színű pontok halmazát színosztálynak nevezzük.

## Színezés

Valamely, legalább egy élet tartalmazó gráf akkor és csak akkor páros, ha kromatikus száma 2.  
**biz**: Ha páros a gráf, akkor az egy-egy osztály pontjai között nincs él, ezek egy-egy színnel színezhetők. Továbbá, ha a gráfnak van egy éle, akkor min 2 szín kell.
Ha két szín elegendő egy gráf színezéséhez, akkor az egy színosztályba tartozó pontok között nincs él, ha lenne, nem lehetnének azonos színűek, ezért a színosztályok egyben a páros gráf definíciójában szereplő két csúcshalmazt alkotják.

páros hosszú körök kromatikus száma 2, páratlan hosszú körök kromatikus száma 3.
az n pontú teljes gráf kromatikus száma n.

Tétel: Ha a maximális fokszám a G gráfban $\Delta$, akkor $\chi(G)\leq\Delta +1$
**biz**: Bármely x ponttal is kezdjük a színezést, az x pont szomszédjainak színezéséhez nem kell több szín, mint $\Delta$.
Az x pontot pedig színezhetjük a $\Delta +1$ színnel.

## Klikk

G egy teljes részgráfját klikknek nevezzük. A G-ben található maximális méretű klikk mérete, vagyis pontjainak száma az ún. klikk
szám, jelölése: $\omega(G)$.
Tétel: a G gráf kromatikus száma nem lehet kisebb a klikkszámnál: $\chi(G)\geq\omega(G)$.

## NégyszínTétel

Ha G síkbarajzolható gráf, akkor $\chi(G)\leq 4$

## Ford-Fulkerson Tétel

Legyen H=(G,c) hálózat. Ekkor a maximális folyamérték egyenlő a minimális vágással.
biz:
Az előző tételnél láttuk (Maximális folyam), hogy a maximális folyam egyenlő egy alkalmas vágás kapacitásával. Másrészt azt is bizonyítottuk, hogy bármely folyam nem lehet na- gyobb bármely vágás kapacitásánál. Ezért az előző tétel bizonyításában szereplő $(N_{0}, N/N_{0})$ vágás minimális vágás kell legyen.

## Maximális folyam

Ha $s \in N_{0}, t\in N- N_{0}$, akkor a folyam akkor és csak akkor maximális, ha nincsen javító út.
biz:
Ha a folyam maximális, nem létezhet javítóút, mert akkor azt használva a folyam értéke növelhető lenne.  
Ha nincsen javító út, akkor a folyam maximális. Ennek belátásához tekintsük azokat a csúcsokat, ahová még nem vezet javító út, legyen ezek halmaza $N_{0}$, és $s$ is kerüljön ebbe a halmazba. Tekintsük az $(N_{0}, N-N_{0})$ vágást. Tekintsük azokat az előremutató éleket, amelyek $N_{0}$-ból $N-N_{0}$-ba mutatnak. Ezeken a folyamérték egyenlő a kapacitással, máskülönben $j$ is $N_{0}$-hoz tartozna. Ehhez hasonlóan a hátramutató $j \to i$ éleken a folyam 0.
