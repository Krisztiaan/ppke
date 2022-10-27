# Képletek

## Euler formula

$e^{ix}=\cos{x}+i\sin{x}$
ebből ha $x\to -x$
$e^{-ix}=\cos{(-x)}+i\sin{(-x)}i=\cos{x}-i\sin{x}$
így:
$\cos{x}=\frac{e^{ix}+e^{-ix}}{2}$
$\sin{x}=\frac{e^{ix}-e^{-ix}}{2i}$

## Lipschitz feltétel

Azt mondjuk, hogy az $f$ valós-valós függvény teljesíti a **Lipschitz-tulajdonság**ot (vagy **Lipschitz-folytonos**, vagy a matematikus argóban *lipschitzes*), ha létezik olyan $L$ nemnegatív valós szám, amelyre az $f$ függvény értelmezési tartományában) lévő minden $x$ és $y$ pontra fennáll az
$|f(x)-f(y)|\leq L\cdot|x-y|$
egyenlőtlenség.
