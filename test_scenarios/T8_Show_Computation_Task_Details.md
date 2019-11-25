# Test Scenario

## T8 Show Computation Task Details

### Przypadki testowe

#### 1. Otwarcie nieuruchomionego computation taska

___WARUNKI POCZĄTKOWE:___

- Zalogowany użytkownik to "userT8_1".

1. __App User__ wybiera "Show details" przy "Test Task 1".
2. System wyświetla:
    - konfigurację CT:
        ```
        @TODO
        ```
    - aktualny status: ""
    
___WARUNKI SUKCESU:___

- Pojawia się konfiguaracja CT.
- Nie zostają wyświetlone aktualne logi.
- Nie pojawia się żaden status.

#### 2. Otwarcie uruchomionego zloopowanego computation taska

___WARUNKI POCZĄTKOWE:___

- Zalogowany użytkownik to "userT8_1".

1. __App User__ wybiera "Show details" przy "Test Task 2".
2. System wyświetla:
    - konfigurację CT:
        ```
        @TODO
        ```
    - aktualny status: "Working"
    - aktualne logi:
        ```
        <anything>
        APP STARTED
        WAITING FOREVER
        ```
    
___WARUNKI SUKCESU:___

- Pojawia się konfiguracja CT.
- Pojawiają się aktualne logi.
- Pojawia się status "Working".

#### 3. Otwarcie zakończonego computation taska

- Zalogowany użytkownik to "userT8_1".

1. __App User__ wybiera "Show details" przy "Test Task 3".
2. System wyświetla:
    - konfigurację CT:
        ```
        @TODO
        ```
    - aktualny status: "Completed"
    - aktualne logi:
        ```
        <anything>
        APP STARTED
        APP COMPLETED
        <anything>
        ```
    
___WARUNKI SUKCESU:___

- Pojawia się konfiguracja CT.
- Pojawiają się logi poprzedniego wykonywania CT.
- Pojawia się status "Completed".