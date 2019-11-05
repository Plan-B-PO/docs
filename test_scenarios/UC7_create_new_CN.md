# Test scenario

## UC7 Create new CN

### Główny

##### 1. __Supplier__ wybiera opcję dodania nowego CN
##### 2. System wyświetla formularz dodania nowego CN
##### 3. __Supplier__ wypełnia formularz 
##### 4. __Supplier__ naciska przycisk "Akceptuj"
##### 5. System wyświetla komunikat o wygenerowanym tokenie
##### 6. __Supplier__ wybiera opcję "Zakończ"
##### 7. _\<\<invokes\>\>_ UC8 Show owned CN list

# Test Scenario

## UC7 create new CN

### Sprawdzane UC

- [UC3](../scenarios/UC7_create_new_CN)

### Warunki początkowe 

- Zalogowany __Supplier__ to _user02_.

### Przypadki testowe

#### 1. Pomyślne zarejestrowanie maszyny.

1. __Supplier__ wybiera opcję dodanie nowego CN
2. System wyświetla formularz dodania CN
	```
	Nazwa
	```
3. __Suplier__ uzupełnia formularz
	```
	Nazwa: Machine 1
	```

#### 2. Błąd formularza.

1. __Supplier__ wybiera opcję dodanie nowego CN
2. System wyświetla formularz dodania CN
	```
	Nazwa
	```
3. __Suplier__ uzupełnia formularz
	```
	Nazwa: ?#$Machine_1 asd
	```
4. System wyświetla komunikat błędu "Błąd w polu: Nazwa"

___WARUNEK SUKCESU:___

- System nie pozwolił na utworzenie CN z błędną nazwą