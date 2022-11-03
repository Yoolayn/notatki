# Działania na zbiorach
- suma: $A \cup B = \set{x:x \in A \lor x \in B}$
- iloczyn (przekrój): $A \cap B = \set{x:x \in A \land x \in B}$
- różnica: $A \setminus B = \set{x:x \in A \land x \not\in B}$
- różnica sumetryczna: $A \oplus B = (A \setminus B) \cup (B \setminus A)$
- iloczyn kartezjański (produkt): $A \times B = \set{(x,y): x \in A \land y \in B}$

Niech U będzie ustalonym zbiorem i niech $A \subset U$. Dopenieniem A do zbioru U nazywamy zbiór $$\overline{A} = U \setminus A$$
Inne oznaczenia to $A', A^\subset$

$\forall_x$ - dla każdego x
$\exists_x$ - istnieje x
# Podzbiory
Definicja:
Dwa zbiory są równe wtedy i tylko wtedy gdy mają te same elementy, czyli $$A=B\Leftrightarrow\forall_{x}(x\in A \Leftrightarrow x \in B)$$
Z tego wynika, że zbiory A i B są różne (piszemy $A \not = B$) wtedy i tylko wtedy, gdy istnieje element, który należy do jednego z tych zbiorów i nie należy do drugiego.
Zapis z użyciem kwantyfikatorów i spójników logicznych:
$$A \not = B \Leftrightarrow \exists_{x} ((x \in A \land x \not \in B) \lor (x \not \in A \land x \in B))$$
Do (1), (2), (3) i (4) wrócimy do omówienia praw dla kwantyfikatorów
# Zbiór potęgowy
Definicja:
Niech zbiór A będzie dowolnym zbiorb. <b>Zbiorem potęgowym</b> zbioru A nazywamy zbiór oznaczany przez $P(A)$ lub $2^A$ i składający się ze wszystkich podzbiorów zbioru A, czyli mamy $$P(A)=\set{B:B\subset A}$$
zbiór pusty $\emptyset$ i zbiór A są elementami zbioru $P(A): \set{\emptyset, A}\subset P(A)$
Dla dowolnych zbiorów A i B mamy: $$A \subset B \Leftrightarrow P(A) \subset P(B)$$
# Funkcja zdaniowa
Definicja: Przez funkcję zdaniową zmiennej x, której zakresem zmnienności jest zbiór X, będziemy rozumieli wytażenie $\phi(x)$, które staje się prawdziwe lub fałszywe, po podstawieniu każdego z elementów x, zbioru X.

Mówimy, że element $x_0$ ze zbioru X spełnia funckję $\phi(x)$, gdy zdanie $\phi(x)$ jest prawdziwe.

Funkcją zdaniową jest wyrażenie $$\phi(x): x-5>0,\ dla\ x\in \mathbb{R}$$
Funkcję zdaniową spełnia każdy element ze zbioru $(5, \infty)$, nie spełnia każdy element ze zbioru $(-\infty, 5]$
# Kwantyfikatory
Niech $\phi(x)$ będzie funkcją zdaniową zmiennej $x \in X$. Przez
(1) $\forall_{x} \in x\ \phi(x)$ oraz (2) $\exists_{x}\in x\ \phi(x)$
rozumiemy odpowiednio zdania:
- dla każdego $x \in X$ zachodzi (jest prawdziwe) $\phi(x)$,
- istnieje $x \in X$, że zachodzi (jest prawdziwe) $\phi(x)$
znak $\forall$ - nazywamy kwantyfikatorem ogólnym, natomiast znak $\exists$ - kwantyfikatorem szczegółowym
- Zdanie (1) uważamy za prawdziwe wtedy i tylko wtedy, gdy $\phi(x)$ jest prawdziwe, dla każdego $x \in X$,
- natomiast zdanie (2) - gdy istnieje $x \in X$, dla którego $\phi(x)$ jest prawdziwe.
Przykłady:
- Kwadrat dowolnej liczby rzeczywistej jest nieujemny $$\forall_{x\in \mathbb{R}}x^{2}\ge0$$
- Równanie $x^{2}-1=0$ ma rozwiązanie w zbiorze liczb rzeczywistych $$\exists_{x\in\mathbb{R}}x^{2}-1=0$$
# Kwantyfikatory ograniczone do pozbioru
Niech $\phi(x)$ będzie funkcją zdaniową o zakresie $x \in X$ i niech $A \subset X$. Kwantyfikatory ograniczone do zbioru A definiujemy następująco:
- $\forall_{x\in A}\phi(x)\Leftrightarrow\forall_{x}(x \in A \Rightarrow\phi(x))$,
- $\exists_{x\in A}\phi(x)\Leftrightarrow\exists_{x}(x\in A \land\phi(x))$
Przykłady:
- $A \subset B \Leftrightarrow\forall_{x}(x \in A \Rightarrow\phi(x))$
- $A \cap B\not= \emptyset\Leftrightarrow\exists_{x}(x \in A \land x \in B) \equiv\exists_{x\in A}x \in B$
# Zmienne związane i wolne
Każdy kwantyfikator dotyczy pewniej funkcji zdaniowej stojącej za nim - nazywamy ją zasięgiem$$\forall_{x}\underbrace{\exists_{x} \underbrace{(...)}_{zasięg\ dla\ y})}_{zasięg\ dla\ x}$$
Definicja:
Zmienną wyrażeniu nazywamy związaną, jeśli wiąże ją jakiś kwantyfikator tzn. leży ona w zasięgu kwantyfikatora $\forall_x$ lub $\exists_x$. Zmienną, która nie jest związana nazywamy *wolną*
Przykład $\forall_{x}(x>y)$ - x jest związaną, y jest zmienną wolną
Przez $D_{\phi}$ oznaczamy zbiór tych elementów zbioru X, dla których $\phi(x)$ jest prawdziwe $$D_{\phi}= \set{x \in X; \phi(x)}$$
zbiór $D_\phi$ nazywamy *diagramem* funkcji $\phi$. Jeśli $\phi$ jest funckją zdaniową dwóch zmiennych $x \in X$ i $y \in Y$, to $$D_\phi=\set{(x,y)\in X \times Y: \phi(x,y)}$$
Zauważmy, że
- zdanie $\forall_x\phi(x)$ jest prawdziwe $\Leftrightarrow D_{\phi}= X$
- zdanie $\exists_x\phi(x)$ jest prawdziwe $\Leftrightarrow D_{\phi}\not=\emptyset$
# Lemat
Niech $\phi(x)$ i $\psi(x)$ będą funkcjami zdaniowymi zmiennej $x\in X$. Wtedy:
- $D_{\phi\lor\psi}=D_{\phi}\cup D_\psi$
- $D_{\phi\land\psi}=D_{\phi}\cap D_\psi$
- $D_{\neg\phi} = D_{\phi}^C$
# Prawa rachunku kwantyfikatorów
Zdanie zapisane z użyciem kwantyfikatorów nazywamy prawem rachunku kwantyfikatorów, gdy jest ono prawdziwe dla każdej interpretacje występujących w nim symboli funkcji zdaniowych.

Stwierdzenie, że zdanie $\forall_x\phi(x)\Rightarrow\exists_x\phi(x)$ jest prawem rachunku kwantyfikatorów - oznacza, że jest ono prawdziwe dla każdej funkcji zdaniowej $\phi(x)$, niezależnie od jej matematycznej treści.
## Prawa de Morgana
Twierdzenie:
Niech $\phi(x)$ będzie funkcją zdaniową o zakresie zmienności X. Wtedy następujące wyrażenia są prawami rachunku kwantyfikatorów. $$\forall_x\phi(x)\Rightarrow\exists_x\phi(x)$$
Prawa de Morgana
$$\neg\forall_x\phi(x)\Leftrightarrow\exists_x\neg\phi(x)\ (\neg\forall_x\phi(x)\equiv\exists_x\neg\phi(x))$$
$$\neg\exists_x\phi(x)\Leftrightarrow\forall_x\neg\phi(x)\ (\neg\exists_x\phi(x)\equiv\forall_x\neg\phi(x))$$

#### przykład
Niech $\phi(x)$ będzie funkcją zdaniową o zakresie zeminności X. Wtedy następujące wyrażenie są prawami rachunku kwantyfikatorów

$\forall_x\phi(x)\Rightarrow\exists_x\phi(x)$
Prawa de Morgana
$\forall_x\phi(x)\Leftrightarrow\exists_x\neg\phi(x)(\neg\forall_x\phi(x)\equiv\exists_x\neg\phi(x))$
$\neg\exists_x\phi(x)\Leftrightarrow\forall_x\neg\phi(x)(\neg\exists_x\phi(x)\equiv\forall_x\neg\phi(x))$
Niech $\phi(x)$ i $\psi(x)$ będą funkcjami zdaniowymi o zkaresie zmienności X. Wtedy następujące wyrażenia są prawami rachunku kwatyfikatorów.
1. $\forall_x(\phi(x)\land\psi(x))\Leftrightarrow\forall_x\phi(x)\land\forall_x\psi(x)$
2. $\exists_x(\phi(x)\lor\psi(x))\Leftrightarrow\phi(x)\lor\exists_x\psi(x)$
3. $\exists_x(\phi(x)\land\psi(x))\Rightarrow\exists_x\phi(x)\land\exists_x\psi(x)$
4. $\forall_x\phi(x)\lor\forall_x\psi(x)\Rightarrow\forall_x(\phi(x)\lor\psi(x))$


$\neg(p\Rightarrow q)\equiv (p\land\neg q)$
- $\phi(x):4, \psi(x): x$ jest liczbą pierwszą
- $\phi(x): x$ liczba parzysta, $\psi(x):x$liczba nie parzysta

Niech $\psi(x, y)$ będzie funkcją zdaniową o zakresie zmiennych $x\in X$ oraz $y\in Y$, gdzie X i Y są niepustymi zbiorami
$\forall_x\forall_y\phi(x, y)\Leftrightarrow\forall_x\forall_y\psi(x,y)$
$L\equiv D_y=X-Y\equiv P$
istnieje na przykład $x_0$, że $\forall_y$ jest prawdziwa
$\exists_x\forall_y\phi(x,y)\not\Leftarrow\forall_y\exists_x\phi(x,y)$
$\forall_y\exists_x\phi(x,y)\Rightarrow\exists_x\forall_y\phi(x,y)\equiv p\land\neg q$
$\forall_y\exists_xx+y=0$
$\exists_x\forall_yx+y = 0$ - fałszywe
