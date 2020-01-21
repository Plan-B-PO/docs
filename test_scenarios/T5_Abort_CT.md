# Test Scenario

## T5 Anulowanie CT

### Sprawdzane UC

- [UC3](../scenarios/UC3_Abort%20CT)

### Dane początkowe

![model](data/T5_in.svg)

### Warunki początkowe 

- Zalogowany __App User__ to _userT5_1_.
- `Test Task 03` nie jest uruchomiony
- `Test Task 04` jest uruchomiony i zapętlony \[status = IN_PROGRESS\]
- `Test Task 05` jest uruchomiony i zapętlony na pierwszym etapie \[status = IN_PROGRESS\]

### Przypadki testowe

#### 1. Przerwana próba anulowania zapętlonego tasku.

1. __App User__ wybiera opcję wyświetlenia zdefiniowanych CT
2. System wyświetla listę nazw zdefiniowanych CT 
    ```
    - "Test Task 03"
    - "Test Task 04"
    - "Test Task 05"
    ```
3. __App User__ wybiera opcję "Abort" przy "Test Task 04". 
4. System wyświetla okno potwierdzenia, z pytaniem 
   "Are you sure, you want to abort "Test Task 04"?"
5. __App User__ wybiera opcję "NO"
6. System zamyka okno potwierdzenia.

___WARUNEK SUKCESU:___

- Żaden Computation nie został przerwany.

#### 2. Anulowanie nieuruchomionego tasku.

1. __App User__ wybiera opcję wyświetlenia zdefiniowanych CT
2. System wyświetla listę nazw zdefiniowanych CT 
    - `"Test Task 03"`
    - `"Test Task 04"`
    - `"Test Task 05"`
3. __App User__ wybiera opcję "Abort" przy "Test Task 03". 
4. System wyświetla okno potwierdzenia, z pytaniem 
   "Are you sure, you want to abort "Test Task 03"?"
5. __App User__ wybiera opcję "YES"
6. System wyświetla informację "Test Task 03 hasn't been activated".
7. __App User__ wybiera opcję "OK"

___WARUNEK SUKCESU:___

- Żaden Computation nie został przerwany.

#### 3. Anulowanie zapętlonego tasku.

1. __App User__ wybiera opcję wyświetlenia zdefiniowanych CT
2. System wyświetla listę nazw zdefiniowanych CT 
    - `"Test Task 03"`
    - `"Test Task 04"`
    - `"Test Task 05"`
3. __App User__ wybiera opcję "Abort" przy "Test Task 04". 
4. System wyświetla okno potwierdzenia, z pytaniem 
   "Are you sure, you want to abort "Test Task 04"?"
5. __App User__ wybiera opcję "YES"
6. System wyświetla informację o poprawnym anulowaniu "Test Task 04".
7. __App User__ wybiera opcję "OK"

___WARUNEK SUKCESU:___

- _Launcher_ wyświetla status "CANCELED" przy "Test Task 04".


#### 4. Anulowanie zapętlonego dwuetapowego tasku.

1. __App User__ wybiera opcję wyświetlenia zdefiniowanych CT
2. System wyświetla listę nazw zdefiniowanych CT 
    - `"Test Task 03"`
    - `"Test Task 04"`
    - `"Test Task 05"`
3. __App User__ wybiera opcję "Abort" przy "Test Task 05". 
4. System wyświetla okno potwierdzenia, z pytaniem 
   "Are you sure, you want to abort "Test Task 05"?"
5. __App User__ wybiera opcję "YES"
6. System wyświetla informację o poprawnym anulowaniu "Test Task 05".
7. __App User__ wybiera opcję "OK"

___WARUNEK SUKCESU:___

- _Launcher_ wyświetla status "CANCELED" przy "Test Task 05".
