# Zdanie:
	zdanie to wyrażenie logiczne, na które można odpowiedzieć bez zastanawiania się nad szczegółami

---

# Spójniki logiczne
	spójniki logiczne służą do łączenia zdań logicznych w duże większe i bardziej skomplikowane

---

## Negacja
	Negacja powoduje odwrócenie wartości logicznych, na przykład zdanie znegowane dające wynik prawdy dają teraz fałsz

- Czyta się to jako: "Nie prawda, że p/q"
---

## Koniunkcja
	Działa jak and lub && z języków programowania, czyli jeżeli oba są prawdą to wynik to też prawda

- Czyta się to jako: "p i q"

| p | q | p$\land$q |
|---|---|:--------:|
| T | T | T |
| T | F | F |
| F | T | F |
| F | F | F |

---

## Alternatywa
	Jest to OR lub || z języków programowania czyli jeżeli jedno z nich jest prawdą to wynik to też prawda

- Czyta się to jako: "p lub q"

| p | q | p$\lor$q |
|---|---|:--------:|
| T | T | T |
| T | F | T |
| F | T | T |
| F | F | F |

---

## Implikacja
	Można to wytłumaczyć tak, że jeżeli p => q to wtedy wynik końcowy jest uzależniony od tego czy wartość p jest zgodna z wartością q, czyli wartość q ma możliwość nadpisania wartości p jeżeli jest ona większa od niej samej

- Czyta to się jako: "jeśli p, to q" lub "p implikuje q"

| p | q | p$\Rightarrow$q |
|---|---|:--------------:|
| T | T | T |
| T | F | F |
| F | T | T |
| F | F | T |

---

## Równoważność
	Zwraca prawdę wtedy kiedy obie wartości są sobie równe, czy to prawda czy fałsz

- Czyta to się jako: "p wtedy i tylko wtedy gdy q"

| p | q | p$\Leftrightarrow$q |
|---|---|:-------------------:|
| T | T | T |
| T | F | F |
| F | T | F |
| F | F | T |

---

## Kolejność uproszczania

-- najsilniejsze --

- negacja
- koniunkcja i alternatywa
- implikacja i równoważność

-- najsłabsze --
