# Więcej o dowodzeniu ... modus tollens

## Prawo kontrapozycji
	prawo kontrapozycji jest jedny z częściej używanych praw w uzasadnianiu, też w dowodzeniu twierdzeń

$$(p \Rightarrow q) \equiv (\neg \Rightarrow \neg p)$$
To prawo można również sformułować tak, że jeżeli założy się że z p wynika q oraz że q jest fałszywe to trzeba zzakceptować, że p jest fałszywe
$$((p \Rightarrow p) \land \neg q) \Rightarrow \neg p$$
To prawo zapisane w formie wnioskowania:
$$\frac{(p \Rightarrow q), \neg q}{\neg p}$$
Nad kreską znajdują się zdania prawdziwe, przecinek oznacza spójnik logiczny $\land$, pod kreską następnik implikacji

### Przykład

Modul tollendo tollens - tryb obalający \[...] przez obalenie \[...] Jeżeli nie ma śladów uderzeń na zwłokach, a przy tym gdyby zmarły był bity przed śmiercią, to by były ślady uderzeń na zwłokach, wtedy nieprawda, że zmarły był bity przed śmiercią

# Więcej o uzasadnianiu, dowodzeniu ...
	Kolejnym prawem będącym podstawą głównych metdo dowodzenia, jest prawo sprowadzenia do sprzeczności (do absurdu)

$$(\neg \phi \Rightarrow 0) \Rightarrow \phi$$
gdzie 0 jest dowolną formułą sprzeczną. Powyższe prawo zapisane w postaci reguły wnioskowania $$\frac{\neg \phi \Rightarrow 0}{\phi}$$
Dowód:

$(\neg \phi \Rightarrow 0) \Rightarrow \phi \equiv \neg (\neg \phi \Rightarrow 0) \lor \phi$  - prawo eliminacji implikacji
$(\neg \phi \Rightarrow 0) \Rightarrow \phi \equiv (\neg \phi \land \neg 0) \lor \phi$  - prawo negacji implikacji
$(\neg \phi \Rightarrow 0) \Rightarrow \phi \equiv (\neg \phi \land 1) \lor \phi$
$(\neg \phi \Rightarrow 0) \Rightarrow \phi \equiv \neg \phi \lor \phi$  - prawo wyłaczonego środka
$(\neg \phi \Rightarrow 0) \Rightarrow \phi \equiv 1$

Szczególnymi przypadkami tego prawa są też reguły wnioskowania
$\cfrac{(p \land \neg q) \Rightarrow 0}{p \Rightarrow q}, \cfrac{(p \land \neg q) \Rightarrow q}{p \Rightarrow q}, \cfrac{(p \land \neg q) \Rightarrow \neg p}{p \Rightarrow q}, \cfrac{\neg p \Rightarrow p}{p}$

### Przykład
Wykaż, że poniższa formuła jest tautologią$$\phi: \neg(p \lor q) \Rightarrow (\neg p \lor \neg q)$$
*Dowód przez sprzeczność.* Przypuśćmy, że formuła nie jest tautologią: $\neg\phi$.
Zatem dla pewnego wartościowania przyjmuje wartość zero
Kiedy implikacja daje wartość logiczną 0?
Gdy przy pewnym warościowaniu poprzednik ma wartość 1, a następnik 0 $$\underbrace{\neg(p \lor q)}_{1}\Rightarrow \underbrace{(\neg p \lor \neg q)}_0$$
Jeżeli $p$o$p$rzednik im$p$likacji ma wartość 1, to wówczas $p$ i $q$ mają wartości 0. Ale wówczas następnik implikacji, czyli $(\neg p \lor \neg q)$ na wartość 1, a nie 0.

# Dodatkowe spójniki logiczne (funktory)

$\oplus$ - alternatywa wykluczająca (rozłączna)
$p \oplus q$ - "albo p, ablo q"

| $p$ | $q$ | $p \oplus q$ |
|:---:|:---:|:------------:|
|  T  |  T  |      F       |
|  T  |  F  |      T       |
|  F  |  T  |      T       |
|  F  |  F  |      F       |

$$p \oplus q \equiv (p \land \neg q) \lor (\neg p \land q)$$

$\downarrow$ - binegacja (spójnik Pearce'a)
$|$ - dyzjunkcja - (kreska Sheffera)

$p \downarrow q \Leftrightarrow \neg p \land \neg q$ - (ani p ani q)
$p|q \Leftrightarrow \neg p \lor \neg q$ - ( nieprawda, że p lub nieprawda, że q)

# Nadmiar spójników

Każda formuła zdaniowa zapisana za pomocą funktorów $\neg, \lor, \land, \Rightarrow, \Leftrightarrow$ jest równoważna pewnej formule zapisanej tylko i wyłącznie za pomocą funktorów $\neg, \lor$.

*Dowód.* Wystarczy pokazac, że zdania $p\land q, p \Rightarrow q \ i \ p \Leftrightarrow q$ zapiszemy wykorzystując tylko spójniki $\neg, \lor$. Mamy:
- $p \land q \equiv \neg(\neg p \lor \neg q)$
- $p \Rightarrow q \equiv \neg p \lor q$
- $p \Leftrightarrow q \equiv (p \Rightarrow q) \land (q \Rightarrow p) \equiv (\neg p \lor q) \land (\neg q \lor p)$

Za pomocą funktora $|\ (\downarrow)$ można zdefiniować negację i wszystkie pozostałe funktory 