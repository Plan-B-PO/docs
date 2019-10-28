# Test Scenario

## UC4 Activate CT

### Scenariusz główny

##### 1. __App User__ wybiera opcję wyświetlenia zdefiniowanych CT
##### 2. System wyświetla listę zdefiniowanych CT
##### 3. __App User__ wybiera opcję "Activate" przy zdefiniowanym CT
##### 4. System wyświetla informację o poprawnym uruchomieniu CT
##### 5. __App User__ wybiera opcję "OK"
 
### 4a. CT miał niepoprawnie zdefiniowany logger.

##### 4a1. System wyświetla otrzeżenie o niemożliwości skomunikowania się z loggerem.
##### GOTO 5

### 5a. App User wybiera opcję "Abort"

##### _\<\<invokes\>\>_ UC3 Abort CT