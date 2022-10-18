[[Matematyka Elementarna/Informacje organizacyjne|]]
# Język logiki

## zdania
Język logiki zajmuje się zdaniami, którym można przypisać wartość logiczną, czyli stwierdzić czy jest ono prawidziwe(T) czy fałszywe(F)

- oznaczenia zdań: p, q, r, s

## spójniki

 1. $\neg$ lub $\sim$ - negacja
 2. $\land$ - koniunkcja
 3. $\lor$ - alternatywa
 4. $\Rightarrow$ lub $\rightarrow$ - implikacja
 5. $\Leftrightarrow$ lub $\leftrightarrow$ - równoważność

### czytanie spójników
1. $\neg p$ lub $\sim p$ - "nie p" lub "nie prawda p"
2. $p\land q$ - "p i q"
3. $p\lor q$ - "p lub q"
4. $p\Rightarrow q$ lub $p\rightarrow q$ - "p implikuje q" lub "jeśli p to q"
5. $p\Leftrightarrow q$ lub $p\leftrightarrow q$ - "p wtedy i tylko wtedy, gdy q"

### wartości spójników

#### Koniunkcja

|  p  |  q  | $p\land q$ |
|:---:|:---:|:----------:|
|  T  |  T  |     T      |
|  T  |  F  |     F      |
|  F  |  T  |     F      |
|  F  |  F  |     F      |

#### Alternatywa
|  p  |  q  | $p\lor q$ |
|:---:|:---:|:---------:|
|  T  |  T  |     T     |
|  T  |  F  |     T     |
|  F  |  T  |     T     |
|  F  |  F  |     F     | 

#### Negacja
|  p  | $\neg$$ p |
|:---:|:---------:|
|  T  |     F     |
|  F  |     T     | 

#### implikacja
|  p  |  q  | p$\Rightarrow$q |
|:---:|:---:|:----------------:|
|  T  |  T  |        T         |
|  T  |  F  |        F         |
|  F  |  T  |        T         |
|  F  |  F  |        T         | 

#### Równoważność
|  p  |  q  | p$\Leftrightarrow$q |
|:---:|:---:|:-------------------:|
|  T  |  T  |          T          |
|  T  |  F  |          F          |
|  F  |  T  |          F          |
|  F  |  F  |          F          | 

### Tautologia
#### Prawa de Morgana
(1)$$\neg (p \lor q) \Leftrightarrow \neg p \land \neg q$$
(2)$$\neg (p \land q) \Leftrightarrow \neg p \lor \neg q$$

	(1) - nie (p lub q), gdy nie p i nie q 
	(2) - nie (p i q), gdy nie p lub nie q

	Rozumiem to jako, że gdy pomnoży się słowa p jak i q przez negację to odwraca się znaki or i and

#### Sprawdzanie Tautologii
Aby sprawdzić czy dane zdanie jest tautologią trzeba sprawdzić wartości tego zdania dla każdej możliwej wariacji słów występujących w tym zdaniu. Sprawdza się to rozpisując to w tabeli, w tym przykładzie rozpiszę tabelę dla tego przykładu:
$$\phi = \neg (p \lor q) \Leftrightarrow \neg q \land \neg q$$

|  1  |  2  |     3     |        4        |    5     |    6     |           7           |   8    |
|:---:|:---:|:---------:|:---------------:|:--------:|:--------:|:---------------------:|:------:|
| $p$ | $q$ | $p\lor q$ | $\neg(p\lor q)$ | $\neg p$ | $\neg q$ | $\neg p \land \neg p$ | $\phi$ |
|  F  |  F  |     F     |        T        |    T     |    T     |           T           |   T    |
|  F  |  T  |     T     |        F        |    T     |    F     |           F           |   T    |
|  T  |  F  |     T     |        F        |    F     |    T     |           F           |   T    |
|  T  |  T  |     T     |        F        |    F     |    F     |           F           |   T    | 
jeżeli w ostatniej kolumnie $\phi$ wszystkie wartości to prawda (T), wtedy takie zdanie jest tautologią

kolejnym przykładem jest:$$\neg (p \land q) \Rightarrow \neg p \land \neg q$$

| $p$ | $q$ | $\neg p$ | $\neg q$ | $\neg(p \land q)$ | $\neg p \land \neg q$ | $\neg(p \land q) \Rightarrow \neg p \land \neg q$ |
|:---:|:---:|:--------:|:--------:|:-----------------:|:---------------------:|:-------------------------------------------------:|
|  1  |  1  |    0     |    0     |         0         |           0           |                         1                         |
|  1  |  0  |    0     |    1     |         1         |           0           |                         0                         |
|  0  |  1  |    1     |    0     |         1         |           0           |                         0                         |
|  0  |  0  |    1     |    1     |         1         |           1           |                         1                         | 

W ostatniej kolumnie pojawiły się dwie wartości fałsz (0), oznacza to, że to zdanie nie jest tautologią
### Formuły logicznie równoważne - prawa logiczne
Formuły $\phi$ i $\psi$ są logicznie równoważne jeżeli zdanie $\phi \Leftrightarrow \psi$ jest tautologią.
Takie zdanie zapisuje się jako $\phi \equiv \psi$

przykład:

| $p$ | $q$ | $r$ | $q \land r$ | $p \lor (q \land r)$ | $p \lor q$ | $p \lor r$ | $(p \lor q)\land(p \lor r)$ |
|:---:|:---:|:---:|:-----------:|:--------------------:|:----------:|:----------:|:---------------------------:|
|  T  |  T  |  T  |      T      |          T           |     T      |     T      |              T              |
|  T  |  T  |  F  |      F      |          T           |     T      |     T      |              T              |
|  T  |  F  |  T  |      F      |          T           |     T      |     T      |              T              |
|  T  |  F  |  F  |      F      |          T           |     T      |     T      |              T              |
|  F  |  T  |  T  |      T      |          T           |     T      |     T      |              T              |
|  F  |  T  |  F  |      F      |          F           |     T      |     F      |              F              |
|  F  |  F  |  T  |      F      |          F           |     F      |     T      |              F              |
|  F  |  F  |  F  |      F      |          F           |     F      |     F      |              F              | 
Kolumny 5 jak i ostatnia mają takie same wyniki co oznacza, że są równoważne
#### Podstawowe prawa logiczne
<div style="float: left">
	<table>
		<tr>
			<td style="border-color: blue"><span class="math display">\begin{align} p \land T \equiv p \\p \lor F \equiv p \end{align}</span></td>
		</tr>
		<tr>
			<td style="border-color: blue"><span class="math display">\begin{align} p \lor T \equiv T \\ p \land F \equiv F \end{align}</span></td>
		</tr>
		<tr>
			<td style="border-color: blue"><span class="math display">\begin{align} p \lor p \equiv p \\p \land p \equiv p \end{align}</span></td>
		</tr>
		<tr>
			<td style="border-color: blue"><span class="math display">\begin{align} \neg(\neg p) \equiv p \end{align}</span></td>
		</tr>
		<tr>
			<td style="border-color: blue"><span class="math display">\begin{align} p \lor q \equiv q \lor p \\ p \land q \equiv q \land p \end{align}</span></td>
		</tr>
		<tr>
			<td style="border-color: blue"><span class="math display">\begin{align} (p \lor q) \land r \equiv p \lor (q \lor r) \\ (p \land q) \land r \equiv p \land (q \land r) \end{align}</span></td>
		</tr>
		<tr>
			<td style="border-color: blue"><span class="math display">\begin{align} p \lor (q \land r) \equiv (p \lor q) \land (p \lor r) \\ p \land (q \lor r) \equiv (p \land q) \lor (p \land r) \end{align}</span></td>
		</tr>
		<tr>
			<td style="border-color: blue"><span class="math display">\begin{align} \neg(p \land q) \equiv \neg p \lor \neg q \\ \neg (p \lor q) \equiv \neg p \land \neg q \end{align}</span></td>
		</tr>
		<tr>
			<td style="border-color: blue"><span class="math display">\begin{align} p \lor (p \land q) \equiv p \\ p \land (p \lor q) \equiv p \end{align}</span></td>
		</tr>
		<tr>
			<td style="border-color: blue"><span class="math display">\begin{align} p \lor \neg p \equiv T \\ p \land \neg p \equiv F \end{align}</span></td>
		</tr>
	</table>
</div>
<div style="float:left;margin-top:120px;margin-left:15px">
	<span>Nazwy praw zaczynając od 3 pozycji to:<br/>
		- idempotentności alternatywy i koniunkcji<br/>
		- podwójnej negacji<br/>
		- przemienności alternatywy i koniunkcji<br/>
		- rozdzielczości<br/>
		- de Morgana<br/>
		- pochłaniania <br/>
		- wyłącznonego środka, sprzeczności
	</span>
</div>
<div style="clear:both"></div>

##### wykorzystanie prawa wyłączonego środka w dowodzeniu
Czy istnieją liczby niewymierne a i b, takie że $a^b$ jest liczbą wymierną? Odpowiedź: tak

*Dowód*. liczba $c=(\sqrt2)^\sqrt2$. Zgodnie z prawem wyłączonego środka są dwie możliwości
1. c jest wymierna
2. c niej est wymierna (jest niewymierna)

> Jeśli zachodzi przypadek 1 to przyjmujemy $a=\sqrt2$ i $b=\sqrt2$
> Jeśli natomiast prawdą jest 2 to przyjmując $a = c$ i $b = \sqrt2$ mamy
> $$((\sqrt2)^\sqrt2)^\sqrt2=(\sqrt2)^{\sqrt2\times\sqrt2}=2$$

a i b nie zostały wskazane ale wiemy, że istnieją podobno
#### Inna ważne prawa logiczne i ich dowody -cd.
1. $(p \Rightarrow q) \equiv \neg p \lor q$ - prawo eliminacji implikacji
2. $\neg (p \Rightarrow q) \equiv p \land \neg q$ - prawo negacji implikacji
3. $(p \Rightarrow q) \equiv (\neg q\Rightarrow \neg p )$ - prawo kontrapozycji (transpozycji)
4. $[(p \Rightarrow q) \land p] \Rightarrow q$ - prawo odrywania
5. $[(p \Rightarrow q) \land (q \Rightarrow r)] \Rightarrow (p \Rightarrow r)$ - prawo przechodniości implikacji
6. $(p \Leftrightarrow q) \equiv (p \Rightarrow q) \land (q \Rightarrow p)$ - prawo eliminacji równoważności

##### Dowód prawa eliminacji implikacji
$(p \Rightarrow q) \equiv \neg p \lor q$

dowód:

| $p$ | $q$ | $\neg p$ | $\neg p \lor q$ | $p \Rightarrow q$ | $(\neg p \lor q) \Leftrightarrow (p \Rightarrow q)$ |
|:---:|:---:|:--------:|:---------------:|:-----------------:|:---------------------------------------------------:|
|  1  |  1  |    0     |        1        |         1         |                          1                          |
|  1  |  0  |    0     |        0        |         0         |                          1                          |
|  0  |  1  |    1     |        1        |         1         |                          1                          |
|  0  |  0  |    1     |        1        |         1         |                          1                          | 

##### Dowód prawa negacji implikacji
$\neg (p \Rightarrow q) \equiv p \land \neg q$

dowód:

$\neg(p \Rightarrow q) \equiv \neg(\neg p \lor q)$
$\neg(p \Rightarrow q) \equiv p \land \neg q$

##### Dowód prawa kontrapozycji
$(p \Rightarrow q) \equiv \neg p \lor q$
$(p \Rightarrow q) \equiv q \lor \neg p$
$(p \Rightarrow q) \equiv \neg (\neg q) \lor \neg p$
$(p \Rightarrow q) \equiv (\neg q \Rightarrow \lor \neg p)$