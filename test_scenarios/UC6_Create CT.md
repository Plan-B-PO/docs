# Test Scenario

## UC6 Create CT

### Główny

##### 1. __App User__ wybiera opcję utworzenia CT
##### 2. System wyświetla listę aplikacji
##### 3. __App User__ wybiera aplikację z listy
##### 4. System wyświetla szczegóły aplikacji
##### 5. __App User__ wybiera opcję "Create CT"
##### 6. System wyświetla formularz tworzenia CT
##### 7. __App User__ wypełnia formularz tworzenia CT
##### 8. __App User__ wybiera opcję "Create"
##### 9. System wyświetla informację o poprawnie utworzonym CT
##### 10. __App User__ wybiera opcję "OK"
##### 11. System wyświetla listę CT 

### 9a. __Użytkownik__ podał niepoprawne dane loggera.

##### 9a1. GOTO 10 _(bez obsługi teraz, do wykorzystania później)_

### 11a. __App User__ wybiera opcję "Activate"

##### 11a1. _\<\<invokes\>\>_ UC4 Activate Computation Task 