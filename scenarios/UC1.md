## Scenariusz do przypadku użycia UC1: Show Computation Cockpit

### Scenariusz główny
1. Launcher wysyła do Library zapytanie o listę danych aplikacji App-usera <<*action*>>
2. Library rozpoczyna obsługę zapytania <<*action*>>
3. Library pobiera listę danych aplikacji App-usera z bazy aplikacji <<*data*>>
4. Library przesyła listę danych aplikacji do Launchera <<*data*>>
5. Launcher pobiera listę Computation Tasks z bazy <<*data*>>
6. Launcher wyświetla listy aplikacji oraz Computation Tasks <<*screen*>>

### Scenariusz alternatywny I
2. Library odrzuca połączenie <<*action*>>
3. Launcher wyświetla komunikat o błędzie <<*screen*>>

### Scenariusz alternatywny II
5. Launcher nie może połączyć się z bazą zawierającą Computation Tasks <<*action*>>
6. Launcher wyświetla komunikat o błędzie <<*screen*>>