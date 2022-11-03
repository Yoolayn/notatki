21.10.2022

Niech $\phi(x)$ będzie funkcją zdaniową o zakresie zmienności X. Wtedy następujące wyrażenia są prawami rachunku kwantyfikatorów

$\forall_x\phi(x)\Rightarrow \exists_x\phi(x)$
Prawa de Morgana
$\forall_x\phi(x)\Leftrightarrow\exists_{x}\neg\phi(x)\ (\neg\forall_x\phi(x)\equiv\exists_{x}\neg\phi(x))$
$\neg\exists_{x}\phi(x)\Leftrightarrow\forall_x\neg\phi(x)\ (\neg\exists_{x}\phi(x)\equiv\forall_x\neg\phi(x))$
Niech $\phi(x)$ i $\psi(x)$ będą funkcjami zdaniowymi o zakresie zmienności X. Wtedy następujące wyrażenia są prawami rachunku kwantyfikatorów.
1. $\forall_x(\phi(x)\land\psi(x))\Leftrightarrow\forall_x\phi(x)\land\forall_x\psi(x)$
2. $\exists_{x}(\phi(x)\lor\psi(x))\Leftrightarrow\phi(x)\lor\exists_{x}\psi(x)$
3. $\exists_{x}(\phi(x)\land\psi(x))\Rightarrow\exists_{x}\phi(x)\land\exists_{x}\psi(x)$
4. $\forall_x\phi(x)\lor\forall_x\psi(x)\Rightarrow\forall_x(\phi(x)\lor\psi(x))$
$\neg(p\Rightarrow q)\equiv (p \land \neg q)$
- $\phi(x): 4|x$, $\psi(x):x$ jest liczbą pierwszą
- $\phi(x): x$ liczba parzysta, $\psi(x): x$ liczba nie parzysta

Niech $\phi(x,y)$ będzie funkcją zdaniową o zakresie zmiennych $x \in X$ oraz $y \in Y$ gdzie X i Y są niepustymi zbiorami
$\forall_x\forall_{y}\ \phi(x,y)\Leftrightarrow\forall_x\forall_y\phi(x,y)$
$L \equiv D_{y}= X - Y \equiv P$
$\exists_{x}\forall_y\phi(x,y)\Rightarrow\forall_y\exists_{x}\phi(x,y)$
istnieje na przykład $x_0$ że $\forall_y$ jest prawdziwa
$\exists_{x}\forall_y\phi(x,y)\not\Leftarrow\forall_y\exists_{x}\phi(x,y)$
$\forall_y\exists_{x}\phi(x,y)\Rightarrow\exists_{x}\forall_y\phi(x,y)\equiv p\land \neg q$a
$\forall_y\exists_{x}x+y = 0$
$\exists_x\forall_{y}x+y=0$ - fałszywe!
---
28.10.2022

Funkcje - szczególny przypadek relacji
![[Brudnopis 2022-10-28 12.15.44.excalidraw]]

$\forall_{x_1,x_2}(x_{1}\not=x_{2}\Rightarrow f(x_{1})\not =f(x_{2}))$
$f: \mathbb{R}\Rightarrow [0, \infty), f(x)=x^{2}$
$f:[0, \infty)\Rightarrow[0,\infty), f(x)=x^{2}$ jest bijekcją, $f^{-1}(x)=\sqrt{x}$
$f: (-\infty,0] \Rightarrow[0,\infty), f(x)=x^{2}$ jest bijekcją $f^{-1}(x) =-\sqrt x$
- $sin(0)=0\Rightarrow \arcsin(0)=0$
- $\sin(\frac{\pi}{2})$

# Twierdzenie
jeśli funkcje $f: X\Rightarrow Y$ i $g: Y\Rightarrow Z$, są odwracalne

# Definicja
Dana jest funckja $f: X \Rightarrow Y$ i podzbiorów A zbioru X. Obraze, zbioru A poprzez funckję f nazywamy zbiór
$$f(A) = \set{y \in Y: \exists_{x\in A}f(x)=y}=\set{f(x): x\in A}$$
# Twierdzenie
Dla funckji $f:X \Rightarrow Y$ praz dowolnych podzbiorów A i B zbioru X mamy:
1. $\text{jeśli} A \subset B\text{, to } f(A)\subset f(B)$
2. $f(A\cup B)=f(A)\cup f(B)$
3. $f(A\cap B)\subset f(A)\cup f(B)$
4. $f^{-1}(A\setminus B)=f^{-1}(A)\setminus f^{-1}(B)$

wytłumaczenie 3
3. $f(A\cap B)\subset f(A)\cup f(B)$
$y\in f(A\cup B)\Rightarrow\exists_{x\in A\cap B}f(x)= y$
$x\in A\cap B\Rightarrow x \in A \land x\in B$
$f(x)=y$
$f(A)\land f(B)\not\subset f(A\cap B)$
---
# relacje
## Definicja
Niech X i Y będą zbiorami niepustymi. Dowolny podzbiór iloczynu kartezjańskiego X $\times$ Y nazywamy relacją binarną z X do Y. Jeśli X = Y, to mówimy, że R jest relacją w zbiorze X (lub na zniorze X).

### Przykład 1.
Każda funckja $f:X\Rightarrow Y$ jest relacją pomiędzy elementami zbioru X i Y

### Przykład 4. 
Niech $X = \set{1, 2, 3, 4}$. Które uporządkowane pary są w relacji R na X, jeśli $$R = \set{(x,y); \text{x dzieli y}?}$$
