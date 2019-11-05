# Test Scenario

## UC8 Show owned CN list

### Sprawdzane UC

- [UC8](../scenarios/UC8_Show%20owned%20CN%20list)

### Warunki początkowe 

- Zalogowany __Supplier__ to _user01_.

### Przypadki testowe

#### 1. Pomyślne wyświetlenie listy posiadanych maszyn.

1. __Supplier__ wybiera opcję wyświetlenia posiadanych CN
2. System wyświetla listę posiadanych CN - pokazując ich nazwy oraz statusy
    ```
    - "Test Machine 01 - online"
    - "Test Machine 04 - offline since 2 days"
    ```

___WARUNEK SUKCESU:___

- Użytkownik dowiedział się, które z jego maszyn działają w systemie.

#### 2. Wyświetlenie pustej listy maszyn.

1. __Supplier__ wybiera opcję wyświetlenia posiadanych CN
2. System wyświetla komunikat
	```
	Nie znaleziono dostępnych maszyn. Zarejestruj nową.
	```
	oraz przycisk dodania nowej maszyny.

___WARUNEK SUKCESU:___

- Użytkownik dowiedział się o możliwości zarejestrowania maszyny.