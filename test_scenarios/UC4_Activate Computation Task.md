# Test Scenario

## UC4 Activate CT

### Scenariusz główny

##### 1. __App User__ wybiera opcję wyświetlenia zdefiniowanych CT
##### 2. System wyświetla listę zdefiniowanych CT
##### 3. __App User__ wybiera opcję "Activate" przy zdefiniowanym CT
##### 4. System wyświetla dane wejściowe CT.
##### 5. __App User__ wybiera opcję "OK"
##### 6. System wyświetla informację o poprawnym uruchomieniu CT
##### 7. __App User__ wybiera opcję "OK"
 
### 5a. __App USer__ wybiera opcję "Cancel"

##### 5a1. System przechodzi do widoku CT.
 
### 6a. CT miał niepoprawnie zdefiniowany logger.

##### 6a1. System wyświetla otrzeżenie o niemożliwości skomunikowania się z loggerem.
##### GOTO 5

### 7a. __App User__ wybiera opcję "Abort"

##### _\<\<invokes\>\>_ UC3 Abort CT