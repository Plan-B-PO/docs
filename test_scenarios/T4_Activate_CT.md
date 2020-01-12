# Test Scenario

## T4 Aktywowanie CT

### Sprawdzane UC

- [UC4](../scenarios/UC4_Activate%20Computation%20Task)

### Dane początkowe

![model](data/T4_in.svg)

### Warunki początkowe 

- Zalogowany __App User__ to _userT4_1_.
- Zalogowani __Supplierzy__ to _userT9_1_ i _userT10_1_ i są w widoku posiadanych maszyn.
- Wszystkie uruchomione maszyny należą do _userT9_1_ lub _userT10_1_.

### Przypadki testowe

#### 1. Uruchomienie poprawnego tasku

1. __App User__ wybiera opcję wyświetlenia zdefiniowanych CT
2. _Launcher_ wyświetla listę nazw zdefiniowanych CT 
    ```
    - "Test Task 01"
    ```
3. __App User__ wybiera opcję "Activate" przy "Test Task 01". 
4. _Launcher_ wyświetla dane wejściowe CT.
    ```
    logger = default
    ```
5. __App User__ wybiera opcję "OK"
6. _Launcher_ wyświetla informację o poprawnym uruchomieniu CT "Test Task 01".
7. __Supplierzy__ odświeżają swoje strony i sprawdzają statusy maszyn.
8. __App User__ wybiera opcję "OK"
9. _Launcher_ wyświetla widok CT "Test Task 01" ze statusem "IN_PROGRESS"
10. __App User__ wybiera opcję "Refresh logs" po około 30 sekundach
11. _Launcher_ wyświetla log z aktualną godziną. 
12. __Supplierzy__ odświeżają swoje strony i sprawdzają statusy maszyn.

___WARUNEK SUKCESU:___

- Do domyślnego loggera zostały wypisane logi. 
- Status computation taska się zmienił.
- Status którejś z maszyn zmienić się na "WORKING" z "WAITING".