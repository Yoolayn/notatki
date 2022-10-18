[[Matematyka dyskretna/Informacje organizacyjne|]]
# Najważniejsze oznaczenia

## Oznaczenia zbiorów

Zbiór liczb całkowitych => Z
- Przykłady: -5, -4, -3, -2, -1, 0, 1, 2, ...

Zbiór liczb rzeczywistych => R

Zbiór liczb wymiernych => Q
- Przykłady: $\frac{a}{b}$

Zbiór liczb niewymiernych => R - Q
-Przykłady: $\sqrt2, \pi$

## oznaczenia zakresów
\[a,b] - taki x, że $a\leq x\leq b$
(a,b) - taki x, że $a\lt x\lt b$
\[a,b) - taki x, że $a\leq x\lt b$
(a,b] - taki x, że $a\lt x\leq b$

## wartość bezwzględna
$|x|$ - wartość bezwzględna

$|x|=\begin{cases}
	x&(jeżeli\ x\geq 0)\\
	-x&(jeżeli\ x\lt 0)
\end{cases}$

## potęgi
funkcja potęgowa to: $x^n$
- przykłady: $x^0=1;x^n=x*x*x*\ldots*x\ dla\ n\geq 1; 0^0=1;(x^n)^m=>x^{n*m}$

## logarytmy
$\log_bx=?$  => logarytm o podstawie b z x
- przykłady: $\log_416=2$

## reszta z dzielenia
resztę z dzielenia można zdefiniować jako liczbę jakiej nam brakuje aby liczba była podzielna przez liczbę całkowitą

$x \oplus k=r(=x-k\times \frac{x}{\lfloor k\rfloor})$

r => ile nam brakuje żeby liczba była podzielona przez k, kiedy k jest liczbą całkowitą

$8\oplus 3=2$

$8=2\times3+2$

$-5\oplus 2=(-6+1\oplus 2=1)$

$(-11)\oplus 4=(-12+1)\oplus 4=1$

$x\ div\ k$ - ile razy k mieści się w $x=\frac{x}{k}$

## Sumy i dzielenie
$\sum\limits^n_{i=1}=x_1+x_2+x_3+\ldots+x_n$

$\sum\limits^8_{i=8}(8-i)=8+7+6+5+4+3+2+1+0$

| i=0 | i=1 | i=2 | i=3 | i=4 | i=5 | i=6 | i=7 | i=8 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| j=8 | j=7 | j=6 | j=5 | j=4 | j=3 | j=2 | j=1 | j=0 | 

$j=8+7+6+5+4+3+2+1+0$

![[Brudnopis 2022-10-05 09.48.08.excalidraw]]

![[Brudnopis 2022-10-05 09.53.10.excalidraw]]

$\prod\limits^n_{i=1}x_{1}\times x_{2}\times x_{3}\times\ldots\times x_n$

## Zbiory

$x\in S$ - $x$ jest elementem zbioru S
S - zbiór
|S| - liczebność zbioru (lub elementu)
S = {1, 2, auto, pociąg} => wszystko może być elementem takiego zbioru
S = {$x_1,x_2,x_3,x_4,x_5,\ldots,x_n$}
S = {x:P(x)} => zbiór takich x, które spełniają wyrażenie P(x)
zbiór pusty: {} lub $\cancel\circ$
S - T = {$x:x\in S$ oraz $x\cancel\in T$}
$\bar S=\set{x:x\in U\ i\ x\cancel\in S}$