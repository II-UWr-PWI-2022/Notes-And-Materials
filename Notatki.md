# Podział tematów

* **Dokumentacja**: wszyscy swoją część
* **Interfejs**: Jakub Karwala
* **Testowanie**: Jan Burdzicki
* **Boty**: Jan Burdzicki, Joanna Suwaj, Cyryl Szatan
* **Turniej botów i opcja gry przeciw komputerowi na 3 poziomach trudności**: Krzysztof Szymański
* **Silnik gry**: Krystian Mikoda
* **Profile użytkowników, statystyki, ranking, dodatki**: Mateusz Kozłowski

# Podział na branche

Na każdą część zrobić osobny branch, np. jeśli robimy zmianę związaną z interfejsem, to robimy to na branchu interface, jeśli robimy zmianę dotyczącą dodatków na branchu add-ons. Możecie nazywać dowolnie brancha (język ang i zwrot pasujący do zagadnienia) i dzielić na podbranche (ale wątpię, żeby to było potrzebne)

# Styl Commitów

```
<typ>[scope - opcjonalnie]: <opis>

[body - opcjonalnie]
```

## Typy:

* **build** -> zmiany dotyczące procesu build
* **chore** -> inne zmiany, które nie zmieniają plików źródłowych i plików testowych
* **docs** -> zmiany w dokumentacji
* **feat** -> dodanie feature'u
* **fix** -> naprawienie buga
* **perf** -> poprawa performance'u
* **refactor** -> zmiany kodu, które nie naprawiają bugów i nie dodają nowych feature'ów
* **revert** -> cofnięcie poprzedniego commita
* **style** -> zmiany, które nie mają wpływu na znaczenie kodu (białe spacje, formatowanie, itp.)
* **test** -> dodawanie testów lub poprawianie obecnych

## Scope - gdzie zostały dokonane zmiany

## Uwaga! Jeśli zmiany były ważne, zmieniały działanie kodu w stosunku do poprzedniej wersji, to można dodać `!` przed `:`.

## Subject Line:

* długość <= 50 znaków
* brak kropki na końcu
* rozkazująca forma czasowników
* krótkie wspomnienie czego dotyczyły zmiany

## Body:

* długość linii <= 72 znaków
* rozkazująca forma czasowników
* opis co, gdzie, ale nie jak -> jeśli ktoś chce zobaczyć jak, to zajrzy do kodu, ale musi się przynajmniej orientować co i gdzie zostało zmienione
* wspomnienie jakie komponenty zostały zmienione

## Ogólne:

* pusta linia pomiędzy subject line i body

## Przykładowy commit:

```
fix: prevent racing of requests

Introduce a request id and a reference to latest request. Dismiss
incoming responses other than from latest request.

Remove timeouts which were used to mitigate the racing issue but are
obsolete now.
```

# Styl kodu

* snake case
* nazwy zmiennych, funkcji i komentarze po ang
* przed funkcjami komentarze co ta funkcja robi
* nazwy klas i structów z dużej litery

# Dokumentacja

TODO: napisać