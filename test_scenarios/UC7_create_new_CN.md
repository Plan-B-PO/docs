# Test Scenario

## UC7 create new CN

### Sprawdzane UC

- [UC7](../scenarios/UC7_create_new_CN)

### Warunki początkowe 

- Zalogowany __Supplier__ to _3_.

### Przypadki testowe

#### 1. Pomyślne zarejestrowanie maszyny.

1. __Supplier__ wybiera opcję dodanie nowego CN.
2. System wyświetla formularz dodania CN.
	```
	  - "Name"
	  - "Cpu"
	  - "Gpu"
	  - "Memory"
	  - "Local Storage" 
	```
3. __Supplier__ uzupełnia formularz
	```json
    {
      "Name": "Machine1",
      "Cpu": 4,
      "Gpu": 4,
      "Memory": 32,
      "Local Storage": 128
    }
	```
4. __Supplier__ wybiera opcję _Create_.
5. System wyświetla wygenerowany token: (np. `d7156b67f89e2ccbb226ecd5aabcdd93`)
6. __Supplier__ wybiera opcję `OK`.
7. System wyświetla listę CN.

___WARUNEK SUKCESU:___
- System wyświetlił token.
- Nowy CN został dodany do listy.

#### 2. Błąd formularza.

1. __Supplier__ wybiera opcję dodanie nowego CN.
2. System wyświetla formularz dodania CN.
    ```
	  - "Name"
	  - "Cpu"
	  - "Gpu"
	  - "Memory"
	  - "Local Storage" 
	```
3. __Suplier__ uzupełnia pole formularza.
	```json
    {
      "Name": "Machine2_#asd",
      "Cpu": 4,
      "Gpu": 4,
      "Memory": 32,
      "Local Storage": 128
    }
    ```
4. System wyświetla komunikat błędu "Wrong name given".

___WARUNEK SUKCESU:___

- Komunikat błedu jest wyświetlony
- Nie wyświetla się w żaden sposób aktywny przycisk _Create_.