# Relacyjny model baz danych
- dr E.C.Codd (1970 r.)
- informacje = relacje
- encje vs związki

# Cechy encji
- nazwa
- atrybuty
- typ danych
- atomowość
- redundancja $\Rightarrow$ UWAGA!
- klucz główny 

# Modelowanie encji
- unkalna nazwa
- unikanie polskich znaków, ale nie wszędzie
- optymalizacja

# Diagram encji (ERD) - przykład
Założenia:
- towart (produkty) podzielone na kategorie
- klienci; każdy klient dokonał przynajmniej jednego zakupu $\Rightarrow$ potrwiedzeniem faktura
- rowart są dostaczan do sklepu dzięki dostawcom
- każdy klient po dokonaniu zakupów otrzymuje fakturę


# Związki między encjami

$\Rightarrow$ związek (asocjacja) - definicja

Cechy związku:
- stopień związku
	- związki unarne - łączą się same z sobą
	- Binarne - dwie encje połączone ze sobą 
	- Ternarne - 3 połączone ze sobą
	- n-arne - n ze sobą
- typy asocjacji
	- 1:1 - jeden do jeden (Każdy uczeń może wypożyczyć tylko i wyłącznie jedną książkę)
	- 1:n - jeden do wiele (Każdy uczeń może wypożyczyć wiele książek jednocześnie)
	- m:n - wiele do wiele (Każdy uczeń może wypożyczyć wiele książek, i książka może być wypożyczona wiele razy)

- związek między encjami jest możlwiy gdy:
	- istnieje klucz podstawowy (główny)
	- istnieje klucz obcy
- istnienie (klasa przynależności związku)
# Diagram ERD $\Rightarrow$ relacja 1:1
*insert zdjęcie relacji 1:1*
# Diagram ERD $\Rightarrow$ relacja 1:n
# Diagram ERD $\Rightarrow$ relacja n:m