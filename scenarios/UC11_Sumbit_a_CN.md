 ## Scenariusz do przypadku użycia UC11: Submit a CN.

SP: Supplier jest w widoku detali maszyny

### Scenariusz główny
1. Supplier wybiera opcję "Download script".
2. System generuje skrypt aktywacyjny.
3. System udostępnia skrypt aktywacyjny.
4. Supplier zapisuje skrypt aktywacyjny.
5. Supplier uruchamia na maszynie skrypt aktywacyjny.
6. Maszyna przesyła do systemu wartość tokenu.
7. System waliduje token.
8. System przesyła do maszyny status walidacji.
9. Maszyna odbiera status walidacji.
10. Maszyna wyświetla status o poprawnym zarejestrowaniu.
11. Maszyna przesyła do systemu status aktywacji.
12. System odbiera status aktywacji.
13. System wyświetla komunikat o poprawnym zarejestrowaniu maszyny.
14. Supplier zamyka okno komunikatu


### Scenariusz alternatywny I
[zawyżone parametry maszyny]

10. Maszyna wyświetla status o zawyżonych parametrach.
11. Maszyna przesyła do systemu status aktywacji.
12. System odbiera status aktywacji.
13. System wyświetla komunikat o zawyżonych parametrach maszyny.
14. Supplier zamyka okno komunikatu.


### Scenariusz aletrnatywny II
[brak walidacji tokenu]

10. Maszyna wyświetla status o błędnym tokenie.

