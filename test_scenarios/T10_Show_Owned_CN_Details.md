# Test Scenario

## T4 Show Owned CN Details

### Warunki początkowe

- Zalogowany użytkownik to `userT10_1`.
- Początkowy widok to "Owned mashine list".

### Przypadki testowe

#### 1. Wyświetlenie detali zadeklarowanej maszyny.

1. __Supplier__ klika przycisk "Details" przy maszynie `mashineT10_1`.
2. System wyświetla widok detali maszyny zawierający:
    - name
    - _:MachineDetails_
    - status: "Declared"
3. __Supplier__ naciska na przysik "Show token"
4. System wyświetla token.
    
___WARUNKI SUKCESU:___

- Wyświetliły się zadeklarowane paramety maszyny.
- Token wyświetlił się po naciśnięciu na przycisk.

#### 2. Wyświetlenie detali zaakceptiowanej maszyny.

1. __Supplier__ klika przycisk "Details" przy maszynie `mashineT10_1`.
2. System wyświetla widok detali maszyny zawierający:
    - name
    - _:MachineDetails_
    - status: "Off"
    
___WARUNKI SUKCESU:___

- Wyświetliły się zadeklarowane paramety maszyny.

#### 3. Wyświetlenie detali uruchomionej maszyny.

1. __Supplier__ klika przycisk "Details" przy maszynie `mashineT10_1`.
2. System wyświetla widok detali maszyny zawierający:
    - name
    - _:MachineDetails_
    - status: "Waiting"
    
___WARUNKI SUKCESU:___

- Wyświetliły się zadeklarowane paramety maszyny.