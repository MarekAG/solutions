###Zadanie 1a MongoDB

Do zadania wybralem miesieczna baze danych z postow reddita z kwietnia 2015
Nazwa pliku: RC_2015-01

#####Import pliku bazy danych Reddit RC_2015-01 do bazy MongoDB wersja 3.0.7

```sh
time bunzip2 -c RC_2015-05.bz2 | mongoimport --drop --host 127.0.0.1 -d test -c reddit
```
Sredni czas importu to ok 9000 pozycji na sekunde.
Procesor obciazoy byl w ~80%. Obciazenie skakalo, gdyz import przebiegal poszczegolymi paczkami:



