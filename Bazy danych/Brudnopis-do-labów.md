Założenia:
- sklep sprzedaje produkty podzielone na kategorie
- należy uwzględnić dane klientów - każdy klient dokonał przynajmniej jednego zakupu
- sklep ma możliwość wystawienia faktur
- sklep musi obsługiwać reklamacje
---

| <span style="color:red">Klienci </span> |
| -------- |
| id |
| imie     |
| nazwisko |
| nip      | 

| <span style="color:red">produkty </span> |
| --------- |
| id        |
| nazwa     |
| cena      |
| kategoria |

| <span style="color:red">zakupy </span> | 
| -------------------------------------- |
| id                                     |
| data                                   |
| ilość                                  |
| id_klienta                             |
| id_produktu                            |
| id_pracownika                          |

| <span style="color:red">pracownicy </span>|
| ---------- |
| id         |
| imie       |
| nazwisko   |
| adres           |

| <span style="color:red">Kategoria</span> |
| --------- |
| id        |
| nazwa     | 

| <span style="color:red"> reklamacje </span> |
| ---------- |
| id         |
| id_zakupu  |
| data           |
