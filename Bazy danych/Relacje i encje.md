# Relacyjny model baz danych
- dr E.C.Codd (1970r.)
- informacje = relacje
- encje vs związki

# Cechy encji
- nazwa
- atrybuty
- typ danych
- atomowość
- redundacja $\Rightarrow$ UWAGA!
- klucz główny

# Modelowanie encji
- unikalna nazwa
- unikanie polskich znaków, ale nie wszędzie
- optymalizacja

# Diagram encji (ERD) - przykład
Założenia:
- towar (produkty) podzielone na kategorie
- klienci; każdy klient dokonał przynajmniej jednego zakupu $\Rightarrow$ potwierdzeniem jest faktura
- towar są dostarczane do sklepu dzięki dostawcom
- każdy klient po dokonaniu zakupów otrzymuje fakturę

![[20221018_093540.jpg]]
$\Rightarrow$ związek (asocjacja) - definicja

Cechy związku:
- stopień związku:
	- związki unarne - łączą się same z sobą
	- binarne - dwie encje połączone ze sobą
	- ternarne - trzy tabele połączone ze sobą
	- n-arne - n ze sobą
- typy asocjacji
	- 1:1 - jeden do jeden (Każdy uczeń może wypożyczyć tylok i wyłącznie jedną książkę)
	- 1:n - jeden do wiele (Każdy uczeń może wypożyczyć wiele książek jednocześnie)
	- n:m - wiele do wiele (Każdy uczeń może wypożyczyć wiele książek, i książka może być wypożyczona wiele razy)

- związek między encjami jest możliwy gdy:
	- istnieje klucz podstawowy (główny)
	- istnieje klucz obcy
- istnienie (klasa przynależności związku)

# Diagram ERD $\Rightarrow$ relacja 1:1
![[20221018_095051.jpg]]
# Diagram ERD $\Rightarrow$ relacja 1:n
# Diagram ERD $\Rightarrow$ relacja n:m