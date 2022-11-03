# Kod graya
> jest to kod zwany refleksyjnym, czyli uporządkowany kod binarny bezwagowy i niepozycyjny, w którym dwa kolejne słowa kodowe różnią się od siebie tylko stanem jednego bitu, ponad to także ostatni i pierwszy wyraz tego kodu spełniają tę własność ( a zatem kod Graya jest także kodem cyklicznym)

## Algorytm rozszerzania kodu graya
> Załózmy, że cia C jest kodem Graya, w którym słowa kodowe są długości n. Aby otrzymać kod Graya o słowach
## Algorytm wyznaczania i-tego wyrazu n-bitowego kodu Graya
1. Zapisz pomniejszony o jeden numer wyrazu kodu Graya w anturalnym kodzie dwójkowym na zadanej liczbie bitów (brakujące bity uzupełniej bitem 0)
2. Przesuń kopię ciągu z kroku 1 o jeden bit w prawo (najmniej znaczący bit oddrzuć, a na początku dopisz wartości 0, czyli podziel całkowicie przez 2)
3. Wykonaj XOR na odpowiednich bitach liczb z kroków 1 oraz 2; wynik jest wyrazem w kodzie Graya 
### Przykład:
W oparciu o algorytm i-tego wyrazu n-bitowego kodu Graya wyznacz 10-ty wyraz 1-bitowego (przykładowego Graya)
Interesuje nas 10-ty wyraz. Mamy $(9)_{10}$ = $(1001)_2$, a przesunięcie tego ciągu binarnego w prawo o jeden bit daje w yniku ciąg $(0100)_{2}$

| XOR | 0   | 1   |
| --- | --- | --- |
| 0   | 0   | 1   |
| 1   | 1   | 0    |

|     | 1001 |
| --- | ---- |
| XOR | 0100 |
|     | 1101 |

Za tem 10-ty wyraz ciągu Graya to $1101_{2}$

kod Graya:

![[Brudnopis 2022-10-26 08.46.32.excalidraw]]

### Przeszukiwanie binarne

Załóżmy, że mamy "Czarne pudełko", które przechowuje równanie poziomej prostej y = c (której nie znamy), zwanej dalej murem. Jedyny możliwy sposób korzystania z pudełka to zapytanie o to, czy dana wartość d jest większa od c (dla podanego na wejściu argumentu d).
Rozważmy teraz punkt P=P(t), zwany dalej żabą, który porusza się tj. skacze, w czasie o wektor v = \[2,1], startując z punktu P(0) = (0,5) (czyli P(0) = (0,5), P(2) = (4,7), ..., P(i + 1) = P(i) + v, ...). Zaimplementuj efektywny algorytm wyznaczający najwięszką liczbę skoków, które jest w stanie wykonać żaba, aby nie uderzyć w mur.

![[Brudnopis 2022-10-26 09.13.53.excalidraw]]

przykład
wymyślić liczbę między 0-15
zostało wybrane 10

Pytam się czy liczba jest większa, czy mniejsza równa 7 (połowa zbioru)
w tym wypadku większa więc dzielę zbiór większy od 7 na 2 częsci równe i pytam się które jest większe i tak do otrzymania szukanej liczby

| {0, 1, 2, 3, 4, 5, 6, 7} | {8, 9, 10, 11, 12, 13, 14, 15} |
|:------------------------:| ------------------------------ |
|           Nie            | Tak                            |
|      {8 ,9, 10, 11}      | {12, 13, 14, 15}               |
|           Tak            | Nie                            |
|          {8, 9}          | {10, 11}                       |
|           Nie            | Tak                            |
|           {10}           | {11}                           |
|           Tak            | Nie                            |

 ---

 Drzewa przeszukiwań binarnych

węzły po lewej są mniejsze równe, a po prawej są większe od poprzedniego korzenia
![[Brudnopis 2022-11-02 08.27.41.excalidraw]]

Algorytm:
- jeżeli drzewo jest puste elementu nie ma w drzewie
- jeżeli jest nie puste to:
	- jeżeli element drzewa jest równy szukanej to znaleźliśmy szukany element
	- jeżeli jest większe to szukamy w prawej stronie
	- jeżeli jest mniejsze lub równe to szukamy w lewej stronie
