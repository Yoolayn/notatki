# Prawa zmieniające zdania w inne
## Prawa de Morgana

$\neg(p\lor q)\Leftrightarrow\neg p\land \neg q$
$\neg(p\land q)\Leftrightarrow\neg p\lor\neg q$
- nie p lub/i q jest równe nie p i/lub nie q
	- zdanie logiczne można "odwrócić" jeżeli jest znegowane
	- jeżeli spełnia warunek to wtedy trzeba odwrócić znak i/lub na odwrotny i negację zmienić z całego zdania na osobne słowa

[[Język Logiki#Sprawdzanie Tautologii|Przykład sprawdzania tautologii]]

dodatkowe permutacje na podstawie de Morgana:

	jak zmienić p lub q ktore nie sa znegowane i podobne, dzięki prawu podwójnej negacji. Głównie ja napisałem, żebym nie musiał tego 300 razy wyliczać, ale jest to łatwe do zrobienia

$(p \lor q) \Leftrightarrow \neg(\neg p \land \neg q)$
$(\neg p \lor q) \Leftrightarrow \neg(p \land \neg q)$
$(p \lor \neg q) \Leftrightarrow \neg(\neg p \land q)$

---

## Prawo idempotentności alternatywy i koniunkcji

$p\lor p\equiv p$
$p\land p\equiv p$

oznacza to, że prawa [[Matematyka Elementarna/Zdania logiczne i spójniki#Alternatywa|alternatywy]] i [[Matematyka Elementarna/Zdania logiczne i spójniki#Koniunkcja|koniunkcji]] użyte w przypadku tego samego słowa nie mają znaczenia (**p** <u>i\lub</u> **p** zawsze da **p**)

---

## Podwójnej negacji

$\neg(\neg p)\equiv p$

zanegowana negacja przestaje działać, czyli minus i minus daje plus

---

## Przemienności alternatywy i koniunkcji

$p \lor q \equiv q \lor p$
$p \land q \equiv q \land p$

[[Matematyka Elementarna/Zdania logiczne i spójniki#Alternatywa|alternatywa]] i [[Matematyka Elementarna/Zdania logiczne i spójniki#Koniunkcja|koniunkcja]] są przemienne, czyli można słowa dawać obojętnej kolejności i da to ten sam wynik, czyli podobnio do dodawania i mnożenia

---

## Łączności alternatywy i koniunckji

$(p\lor q)\lor r \equiv p \lor (q \lor r)$
$(p\land q)\land r \equiv p \land (q \land r)$

działania [[Matematyka Elementarna/Zdania logiczne i spójniki#Koniunkcja|koniunkcji]] i [[Matematyka Elementarna/Zdania logiczne i spójniki#Alternatywa|alternatywy]] są przemienne, podobnie do dodawania i mnożenia czyli można je wykonywać w dowolnej kolejności, ponieważ dadzą ten sam wynik

---

## Rozdzielności

$(p \lor q)\lor r \equiv(p \lor q)\land(p \lor r)$
$(p \land q)\land r \equiv(p \land q)\lor(p \land r)$

Rozdzielczość oznacza, że [[Matematyka Elementarna/Zdania logiczne i spójniki#Alternatywa|alternatywy]] i [[Matematyka Elementarna/Zdania logiczne i spójniki#Koniunkcja|koniunkcja]] działają podobnie do mnożenia przez nawiasy

---

## Pochłaniania

$p \lor(p\land q)\equiv p$
$p \land(p\lor q)\equiv p$

wynik p lub (p i q) daje wynik p, wynik p i (p lub q) daje wynik p daje wynik p pochłaniając słowo q
- jeżeli sprawdzimy p lub (p i q) da to wyniki równe p (p i q da prawdę wtedy i tylko wtedy gdy wyniki będą
	równe, a p lub p zawsze da p)

---

## Wyłączonego środka, sprzeczności

$p \lor \neg p\equiv \boldsymbol{T}$
$p \land \neg p\equiv \boldsymbol{F}$

słowo i znegowane słowo zawsze będą przeciwne sobie, dlatego używając [[Matematyka Elementarna/Zdania logiczne i spójniki#Koniunkcja|koniunkcji]] zawsze da to fałsz, a [[Matematyka Elementarna/Zdania logiczne i spójniki#Alternatywa|alternatywy]] zawsze da prawdę

---

## Eliminacji implikacji

$p \Rightarrow q \equiv \neg p \lor q$
$p \Rightarrow q \equiv p \land \neg q$

można wyeliminować [[Matematyka Elementarna/Zdania logiczne i spójniki#implikacja|implikację]] poprzez zanegowanie pierwszego słowa co zmienia [[Matematyka Elementarna/Zdania logiczne i spójniki#implikacja|implikację]] w [[Matematyka Elementarna/Zdania logiczne i spójniki#Alternatywa|alternatywę]] lub negując drugie słowo i robiąc z tego [[Matematyka Elementarna/Zdania logiczne i spójniki#Koniunkcja|koniunkcję]]

---

## Negacji implikacji

$\neg(p\Rightarrow q)\equiv p \land \neg q$

podobnie do [[Matematyka Elementarna/Prawa Logiki#Eliminacji implikacji|eliminacji implikacji]] można znegować [[Matematyka Elementarna/Zdania logiczne i spójniki#implikacja|implikację]] negując drugie słowo i porównać używając [[Matematyka Elementarna/Zdania logiczne i spójniki#Koniunkcja|koniunkcji]]

---

## Kontrapozycji (transpozycji)

$(p\Rightarrow q)\equiv (\neg q\Rightarrow\neg p)$

pozwala to zmienić słowa w [[Matematyka Elementarna/Zdania logiczne i spójniki#implikacja|implikacji]] miejscami zmieniając uzależnienie słowa p od słowa q na uzależnienie słowa q od słowa p

---

## Odrywania

$[(p\Rightarrow q)\land p]\Rightarrow q$

wynikiem implikacji słowa p ze słowem q i słowa p wynikiem są wyniki słowa p oznacza to że wzór $[(p\Rightarrow q)\land p]$ można zapisać jako p

---

## Przechodniości implikacji

$[(p\Rightarrow q)\land(q\Rightarrow r)]\Rightarrow(p\Rightarrow r)$

implikacja słowa p ze słowem q i implikacja słowa q ze słowem r można zapisać jako implikację słowa p ze słowem r w skrócię usuwając "middle-man'a", ale tylko wtedy gdy implikacja pierwsza zależy od tego samego słowa, które jest związane w drugiej implikacji, czyli żeby to słowo było koło siebie w zdaniu logicznym

---

## Eliminacji równoważności

$(p\Leftrightarrow q)\equiv(p\Rightarrow q)\land(q \Rightarrow p)$

[[Matematyka Elementarna/Zdania logiczne i spójniki#równoważność|równoważność]] można usunąć zmieniając ją w [[Matematyka Elementarna/Zdania logiczne i spójniki#Koniunkcja|koniunkcję]] dówch odwrotnych [[Matematyka Elementarna/Zdania logiczne i spójniki#implikacja|implikacji]] ($p \Rightarrow q$ i $q \Rightarrow p$)

---

# Dodatkowe spoza wykładu

	wzięte z etrapeza

---

## Sprowadzenie do absurdu

$(p \Rightarrow q)\Leftrightarrow [(p \land \neg q)\Rightarrow 0]$

---
# Przdatne tautologie, które można dodawać do dowodów formalnych

## Wprowadzanie alternatywy

$p \Rightarrow (p \lor q)$

---

## opuszczenie koniunkcji

$(p \land q) \Rightarrow p$

---

## Sprowadzenie do sprzeczności

$(p \Rightarrow 0)\Rightarrow \neg p$

---

## Modus ponendo ponens

$[p \land (p \Rightarrow q)]\Rightarrow q$

---

## Modus tollendo tollens

$[(p \lor q )\land \neg p ]\Rightarrow q$
$p \Rightarrow[q \Rightarrow (p \land q)]$

---

## Przechodniść równoważnośc

$[(p \Leftrightarrow q)\land(q \Leftrightarrow r)]\Rightarrow(p \Leftrightarrow r)$

---
## Przechodniość implikacji

$[(p \Rightarrow q)\land(q \Rightarrow r)]\Rightarrow (p \Rightarrow r)$
$(p \Rightarrow q) \Rightarrow [( p \lor r ) \Rightarrow (q \lor r)]$
$(p \Rightarrow q) \Rightarrow [( p \land r ) \Rightarrow (q \land r)]$
$(p \Rightarrow q) \Rightarrow [(q \Rightarrow r) \Rightarrow (p \Rightarrow r)]$

---

## Prawa dylematu konstrukcyjnego

$[(p \Rightarrow q)\land(r \Rightarrow s)]\Rightarrow[(p \lor r)\Rightarrow(q \lor s)]$
$[(p \Rightarrow q) \land ( r \Rightarrow s )] \Rightarrow [ (p \land r) \Rightarrow (q \lor s) ]$

---

## Prawa dylematu destrukcyjnego

$[(p \Rightarrow q) \land (r \Rightarrow s)]\Rightarrow[(\neg q \lor \neg s) \Rightarrow (\neg p \lor \neg r)]$
