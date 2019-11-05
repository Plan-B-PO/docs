# Test Scenario

## UC7 create new CN

### Sprawdzane UC

- [UC7](../scenarios/UC7_create_new_CN)

### Warunki początkowe 

- Zalogowany __Supplier__ to _user01_.

### Przypadki testowe

#### 1. Pomyślne zarejestrowanie maszyny.

1. __Supplier__ wybiera opcję dodanie nowego CN
2. System wyświetla formularz dodania CN
	```
	Nazwa
	```
3. __Supplier__ uzupełnia formularz
	```
	Nazwa: Machine 1
	```
4. __Supplier__ wybiera opcję `Utwórz`.
5. System wyświetla wygenerowany token, np:
`d7156b67f89e2ccbb226ecd5aabcdd93`
6. __Supplier__ wybiera opcję `OK`.
7. System wyświetla listę CN

___WARUNEK SUKCESU:___
- System wyświetlił token
- Nowy CN został dodany do listy

#### 2. Błąd formularza.

1. __Supplier__ wybiera opcję dodanie nowego CN
2. System wyświetla formularz dodania CN
	```
    Nazwa
    CPU
    GPU
    Memory
    Local Storage
	```
3. __Suplier__ uzupełnia pole formularza
	```
	Nazwa: ?#$Machine_1 asd
	```
4. System wyświetla komunikat błędu "Błąd w polu: Nazwa"

___WARUNEK SUKCESU:___

- Przycisk `Utwórz` jest zablokowany
- Komunikat błedu jest wyświetlony