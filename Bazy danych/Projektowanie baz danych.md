## Baza danych
jest zbiór danych zapisanych na nośniku twardym lub przenośnym, zapisana w odpowieniej strukturze

## Systemy zarządzania baz danych - SZBD
oprogramowanie służące do obsługi i tworzenia struktur baz danych. Są 2 rodzaje takiego oprogramowania:
1. desktop'owe
2. serwerowe

## Cechy baz danych
1. Trwałość danych - nie znikają same z siebie i można liczyć na ich obecność
2. niezależność danych:
	- fizyczna niezależność - nie ważne z jakiego oprogramowania się korzysta, będzie można korzystać z niej (nie ma znaczenia client z którego się korzysta aby dostać się do danych z bazy)
	- logiczna niezależność - użytkonicy są chronieni przed modyfikacją struktur danych (odpowiednie przypisanie przywilejów dla danych użytkowników)
3. ochrona (bezpieczeństwo) danych - ochrona bazy danych przed użyciem jej przez osoby do tego nie powołane
4. Integralność danych - dokładne odzwierciedlenie potrzeb, przez które została stworzona (minimum co jest potrzebne, jest zgodne z światem rzeczywistym)
5. współdzielenie danych - jest dostępna dla wielu użytkowników jednocześnie na odpowiedniej ilości maszyn
6. abstrakcja danych - dane opisują tylko i wyłącznie wymagane i istotne aspekty obietków ze świata rzeczywistego (nie ma danych nie potrzebnych jak na przykład koloru paczki)

## Najważniejsze cechy SZBD
- obsługa użytkowników bazdy danych
- modyfikacja kont użytkowników bazy danych
- zarządzanie prawami dostępu użytkowników
- tworzenie struktury bazy danych
- CRUD
- obsługa zapytań (later ma być)
- generowanie raportów i zestawień
- administracja bazą danych

## Etapy projektowania BD
- ==Analiza== - przeanalizowania problemu, czyli jaki jest cel bazy danych, jakie dane będzie przechowywać, i jakie oczekiwania do niej ma jej klient - jest to bardzo ważny krok, złe jego wykonanie będzie się wiązało ze zmianami jej struktury co często jest bardziej czasochłonne niż samo jej tworzenie
- ==Projektowanie(Implementacja)== - przemyślenie jak zorganizować ułożenie danych w tabelach
- ==Testowanie== - sprawdzanie czy wszystko działa i jest sprawne
- ==Wdrożenie i utrzymanie== - pierwsze oficjalne uruchomienie i obsługa

## Normalizacja
Jest to proces optymalizacji struktur danych - polega ona aby jak najbardziej zmniejszy redundację danych (redundacja - powtarzanie się)

Rodzaj Normalizacji:
- 1 NF
- 2 NF
- 3 NF
- BCNF (lub 3.5 NF) - tzw. postac normalna Boyce'a - Codda
- 4 NF
- 5 NG
==Na tych zajęciach będą tylko i wyłącznie pierwsze 3 formy normalizacji==