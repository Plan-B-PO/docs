# Test scenario

## UC7 Create new CN

### Główny

##### 1. __Supplier__ uruchamia klienta systemu na maszynie
##### 2. Klient systemu wyświetla token autoryzacji nowej maszyny
##### 3. __Supplier__ wybiera opcję dodania nowego CN
##### 4. System wyświetla formularz dodania nowego CN
##### 5. __Supplier__ wypełnia formularz 
##### 6. __Supplier__ naciska przycisk "Akceptuj"
##### 7. System wyświetla komunikat o pomyślnym dodaniu nowego CN
##### 8. __Supplier__ wybiera opcję "Zakończ"
##### 9. _\<\<invokes\>\>_ UC8 Show owned CN list

### 2a. Maszyna dodana wcześniej

##### GOTO 9

### 6a. __Supplier__ podał dane nieistniejącej maszyny.

##### 6a1. System wyświetla komunikat o braku połączenia
##### 6a2. ___GOTO 7___