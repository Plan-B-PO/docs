# Test Scenario

## T7 Show Computation Cockpit

### Dane początkowe

@TODO

### Przypadki testowe

### Warunki Początkowe

- Strona startowa to strona logowania.

#### 1. Otwarcie kokpitu bez zapamiętanych tasków

___WARUNKI POCZĄTKOWE:___

1. __App User__ wprowadza dane logowania:
    ```
        userT7_1 / pass
    ```
2. System wyświetla kokpit zawierający następujące komponenty:
    - Własne, zapisane Aplikacje:
        - `testApp01`
            - name
            - icon
            - description
    - Przycisk "Create new task"

___WARUNEK SUKCESU:___

- Został wyświetlony Application Shelf.
- Nie zostały wyświetlony żadne taski.

#### 2. Otwarcie kokpitu ze zdefiniowanymi taskami

___WARUNKI POCZĄTKOWE:___

1. __App User__ wprowadza dane logowania:
    ```
        userT7_2 / pass
    ```
2. System wyświetla kokpit zawierający następujące komponenty:
    - Własne, zapisane Aplikacje:
        - `testApp01`
            - name
            - icon
            - description
    - Przycisk "Create new task"
    - Własne CT:
        - `testTask01`
            - name
            - \<przyciski akcji\>
            - status: "Completed"

___WARUNEK SUKCESU:___

- Został wyświetlony Application Shelf.
- Został wyświetlony CT o statusie "Completed"

#### 3. Otwarcie kokpitu z uruchomionymi taskami

1. __App User__ wprowadza dane logowania:
    ```
        userT7_3 / pass
    ```
2. System wyświetla kokpit zawierający następujące komponenty:
    - Własne, zapisane Aplikacje:
        - `testApp03`
            - name
            - icon
            - description
    - Przycisk "Create new task"
    - Własne CT:
        - `testTask04`
            - name
            - \<przyciski akcji\>
            - status: "Running"

___WARUNEK SUKCESU:___

- Został wyświetlony Application Shelf.
- Został wyświetlony CT o statusie "Running"