# Test Scenario

## UC9 Signal own status

### Sprawdzane UC

- [UC9](../scenarios/UC9_signal_own_status)

### Warunki początkowe 

- Maszyna jest zarejestrowna w systemie
- Klient działa na maszynie

### Przypadki testowe

#### 1. Pomyślne wyświetlenie listy posiadanych maszyn.

1. __App User__ wybiera opcję wyświetlenia posiadanych CN
2. System wyświetla listę posiadanych CN - pokazując ich nazwy oraz statusy
    ```
    - "Test Machine 01 - online"
    - "Test Machine 04 - offline since 2 days"
    ```

___WARUNEK SUKCESU:___

- Użytkownik dowiedział się, które z jego maszyn działają w systemie.

#### 2. Wyświetlenie pustej listy maszyn.

1. __App User__ wybiera opcję wyświetlenia posiadanych CN
2. System wyświetla komunikat
	```
	Nie znaleziono dostępnych maszyn. Zarejestruj nową.
	```
	oraz przycisk dodania nowej maszyny.

___WARUNEK SUKCESU:___

- Użytkownik dowiedział się o możliwości zarejestrowania maszyny.