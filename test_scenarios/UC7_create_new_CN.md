# Test scenario

## UC7 Create new CN

### Główny

##### 1. __Supplier__ uruchamia klienta systemu na maszynie
##### 2. __Supplier__ wybiera opcję dodania nowego CN
##### 3. System wyświetla formularz dodania nowego CN
##### 4. __Supplier__ wypełnia formularz 
##### 5. __Supplier__ naciska przycisk "Akceptuj"
##### 6. System wyświetla komunikat o pomyślnym dodaniu nowego CN
##### 7. __Supplier__ wybiera opcję "Zakończ"
##### 8. _\<\<invokes\>\>_ UC8 Show owned CN list

### 5a. __Supplier__ podał dane nieistniejącej maszyny.

##### 5a1. System wyświetla komunikat o braku połączenia
##### 5a2. ___GOTO 7___