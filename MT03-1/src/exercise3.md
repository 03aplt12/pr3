# Попарное тестирование

# Поле Username может иметь следующие значения :

   standard_user  
   problem_user  
   performance_glitch_user  
   locked_out_user  
   asd123 (любой невырный логин)  
   '    ' (пустое значение)  

# Поле Password может иметь следующие значения :

   secret_sauce (верный пароль)  
   QWER123 (любой неверный пароль)  
   '     ' (пустое значение)  
С учетом входных данных проводим по 3 тест-кейса для каждой из 6 учетных записей (всего 18), попарно тестируя имя пользователя и пароль.  



## Тест-кейс №1 - Авторизация на сайте https://www.saucedemo.com/ через учётную запись "standard_user"

## Вариант с действительным паролем

1. Предшествующие условия:
   - перейти на страницу авторизации https://www.saucedemo.com/
2. Шаги:
   - навести курсор и нажать на поле Username
   - ввести "standard_user"
   - навести курсор и нажать на поле Password
   - ввести "secret_sauce"
   - нажать на кнопку LOGIN
3. Ожидаемый результат:
   - при нажатии на поле ввода Username, появляется возможность ввода с клавиатуры
   - при нажатии на поле ввода Password, появляется возможность ввода с клавиатуры
   - при введенных данных Username - "standard_user" и Password - "secret_sauce", и при дальнейшем нажатии на кнопку LOGIN происходит авторизация и открывается стартовая страница интернет магазина
 
 ## Вариант с недействительным паролем

1. Предшествующие условия:
   - перейти на страницу авторизации https://www.saucedemo.com/
2. Шаги:
   - навести курсор и нажать на поле Username
   - ввести "standard_user"
   - навести курсор и нажать на поле Password
   - ввести "QWER123"
   - нажать на кнопку LOGIN
3. Ожидаемый результат:
   - при нажатии на поле ввода Username, появляется возможность ввода с клавиатуры
   - при нажатии на поле ввода Password, появляется возможность ввода с клавиатуры
   - при введенных данных Username - "standard_user" и Password - "QWER123", и при дальнейшем нажатии на кнопку LOGIN происходит ошибка - Epic sadface: Username and password do not match any user in this service

## Вариант без пароля

1. Предшествующие условия:
   - перейти на страницу авторизации https://www.saucedemo.com/
2. Шаги:
   - навести курсор и нажать на поле Username
   - ввести "standard_user"
   - поле Password остается пустым
   - нажать на кнопку LOGIN
3. Ожидаемый результат:
   - при нажатии на поле ввода Username, появляется возможность ввода с клавиатуры
   - при введенных данных Username - "standard_user", и при дальнейшем нажатии на кнопку LOGIN происходит ошибка - Epic sadface: Password is required


## Тест-кейс №2 - Авторизация на сайте https://www.saucedemo.com/ через  учётную запись "problem_user"

## Вариант с действительным паролем

1. Предшествующие условия:
   - перейти на страницу авторизации https://www.saucedemo.com/
2. Шаги:
   - навести курсор и нажать на поле Username
   - ввести "problem user"
   - навести курсор и нажать на поле Password
   - ввести "secret_sauce"
   - нажать на кнопку LOGIN
3. Ожидаемый результат:
   - при нажатии на поле ввода Username, появляется возможность ввода с клавиатуры
   - при нажатии на поле ввода Password, появляется возможность ввода с клавиатуры
   - при введенных данных Username - "problem_user" и Password - "secret_sauce", и при дальнейшем нажатии на кнопку LOGIN происходит авторизация и открывается стартовая страница интернет магазина

## Вариант с недействительным паролем

1. Предшествующие условия:
   - перейти на страницу авторизации https://www.saucedemo.com/
2. Шаги:
   - навести курсор и нажать на поле Username
   - ввести "problem_user"
   - навести курсор и нажать на поле Password
   - ввести "QWER123"
   - нажать на кнопку LOGIN
3. Ожидаемый результат:
   - при нажатии на поле ввода Password, появляется возможность ввода с клавиатуры
   - при введенных данных Username - "problem user" и Password - "QWER123", и при дальнейшем нажатии на кнопку LOGIN происходит ошибка  - Epic sadface: Username and password do not match any user in this service.

## Вариант без пароля

1. Предшествующие условия:
   - перейти на страницу авторизации https://www.saucedemo.com/
2. Шаги:
   - навести курсор и нажать на поле Username
   - ввести "problem_user"
   - поле Password остается пустым
   - нажать на кнопку LOGIN
3. Ожидаемый результат:
   - при нажатии на поле ввода Username, появляется возможность ввода с клавиатуры
   - при введенных данных Username - "problem_user", и при дальнейшем нажатии на кнопку LOGIN происходит ошибка - Epic sadface: Password is required


## Тест-кейс №3 - Авторизация на сайте https://www.saucedemo.com/ через  учётную запись "performance_glitch_user"

## Вариант с действительным паролем

1. Предшествующие условия:
   - перейти на страницу авторизации https://www.saucedemo.com/
2. Шаги:
   - навести курсор и нажать на поле Username
   - ввести "performance_glitch_user"
   - навести курсор и нажать на поле Password
   - ввести "secret_sauce"
   - нажать на кнопку LOGIN
3. Ожидаемый результат:
   - при нажатии на поле ввода Username, появляется возможность ввода с клавиатуры
   - при нажатии на поле ввода Password, появляется возможность ввода с клавиатуры
   - при введенных данных Username - "performance_glitch_user" и Password - "secret_sauce", и при дальнейшем нажатии на кнопку LOGIN через некоторое время происходит авторизация и открывается стартовая страница интернет магазина

## Вариант с недействительным паролем

1. Предшествующие условия:
   - перейти на страницу авторизации https://www.saucedemo.com/
2. Шаги:
   - навести курсор и нажать на поле Username
   - ввести "performance_glitch_user"
   - навести курсор и нажать на поле Password
   - ввести "QWER123"
   - нажать на кнопку LOGIN
3. Ожидаемый результат:
   - при нажатии на поле ввода Password, появляется возможность ввода с клавиатуры
   - при введенных данных Username - "performance_glitch_user" и Password - "QWER123", и при дальнейшем нажатии на кнопку LOGIN происходит ошибка - Epic sadface: Username and password do not match any user in this service.

## Вариант без пароля

1. Предшествующие условия:
   - перейти на страницу авторизации https://www.saucedemo.com/
2. Шаги:
   - навести курсор и нажать на поле Username
   - ввести "performance_glitch_user"
   - поле Password остается пустым
   - нажать на кнопку LOGIN
3. Ожидаемый результат:
   - при нажатии на поле ввода Username, появляется возможность ввода с клавиатуры
   - при введенных данных Username - "performance_glitch_user", и при дальнейшем нажатии на кнопку LOGIN происходит ошибка - Epic sadface: Password is required


## Тест-кейс №4 - Авторизация на сайте https://www.saucedemo.com/ через  учётную запись "locked_out_user"

## Вариант с действительным паролем

1. Предшествующие условия:
   - перейти на страницу авторизации https://www.saucedemo.com/
2. Шаги:
   - навести курсор и нажать на поле Username
   - ввести "locked_out_user"
   - навести курсор и нажать на поле Password
   - ввести "secret_sauce"
   - нажать на кнопку LOGIN
3. Ожидаемый результат:
   - при нажатии на поле ввода Username, появляется возможность ввода с клавиатуры
   - при нажатии на поле ввода Password, появляется возможность ввода с клавиатуры
   - при введенных данных Username - "locked_out_user" и Password - "secret_sauce", и при дальнейшем нажатии на кнопку LOGIN происходит ошибка - Epic sadface: Sorry, this user has been locked out.

## Вариант с недействительным паролем

1. Предшествующие условия:
   - перейти на страницу авторизации https://www.saucedemo.com/
2. Шаги:
   - навести курсор и нажать на поле Username
   - ввести "locked_out_user"
   - навести курсор и нажать на поле Password
   - ввести "QWER123"
   - нажать на кнопку LOGIN
3. Ожидаемый результат:
   - при нажатии на поле ввода Password, появляется возможность ввода с клавиатуры
   - при введенных данных Username - "locked_out_user" и Password - "QWER123", и при дальнейшем нажатии на кнопку LOGIN происходит ошибка - Epic sadface: Username and password do not match any user in this service.

## Вариант без пароля

1. Предшествующие условия:
   - перейти на страницу авторизации https://www.saucedemo.com/
2. Шаги:
   - навести курсор и нажать на поле Username
   - ввести "locked_out_user"
   - поле Password остается пустым
   - нажать на кнопку LOGIN
3. Ожидаемый результат:
   - при нажатии на поле ввода Username, появляется возможность ввода с клавиатуры
   - при введенных данных Username - "locked_out_user" и при дальнейшем нажатии на кнопку LOGIN происходит ошибка - Epic sadface: Password is required

## Тест-кейс №5 - Авторизация на сайте https://www.saucedemo.com/ через учётную запись с неверным логином

## Вариант с действительным паролем

1. Предшествующие условия:
   - перейти на страницу авторизации https://www.saucedemo.com/
2. Шаги:
   - навести курсор и нажать на поле Username
   - ввести неверный логин, например "asd123"
   - навести курсор и нажать на поле Password
   - ввести "secret_sauce"
   - нажать на кнопку LOGIN
3. Ожидаемый результат:
   - при нажатии на поле ввода Username, появляется возможность ввода с клавиатуры
   - при нажатии на поле ввода Password, появляется возможность ввода с клавиатуры
   - при введенных данных Username - "asd123" и Password - "secret_sauce", и при дальнейшем нажатии на кнопку LOGIN происходит ошибка - Epic sadface: Username and password do not match any user in this service.

## Вариант с недействительным паролем

1. Предшествующие условия:
   - перейти на страницу авторизации https://www.saucedemo.com/
2. Шаги:
   - навести курсор и нажать на поле Username
   - ввести неверный логин, например "asd123"
   - навести курсор и нажать на поле Password
   - ввести "QWER123"
   - нажать на кнопку LOGIN
3. Ожидаемый результат:
   - при нажатии на поле ввода Password, появляется возможность ввода с клавиатуры
   - при введенных данных Username - "asd123" и Password - "QWER123", и при дальнейшем нажатии на кнопку LOGIN происходит ошибка - Epic sadface: Username and password do not match any user in this service.

## Вариант без пароля

1. Предшествующие условия:
   - перейти на страницу авторизации https://www.saucedemo.com/
2. Шаги:
   - навести курсор и нажать на поле Username
   - ввести неверный логин, например "asd123"
   - поле Password остается пустым
   - нажать на кнопку LOGIN
3. Ожидаемый результат:
   - при нажатии на поле ввода Username, появляется возможность ввода с клавиатуры
   - при введенных данных Username - "asd123" и при дальнейшем нажатии на кнопку LOGIN происходит ошибка - Epic sadface: Password is required.

## Тест-кейс №6 - Попытка авторизация на сайте https://www.saucedemo.com/ с незаполненным логином

## Вариант с действительным паролем

1. Предшествующие условия:
   - перейти на страницу авторизации https://www.saucedemo.com/
2. Шаги:
   - навести курсор и нажать на поле Username
   - не вводить логин
   - навести курсор и нажать на поле Password
   - ввести "secret_sauce"
   - нажать на кнопку LOGIN
3. Ожидаемый результат:
   - при нажатии на поле ввода Username, появляется возможность ввода с клавиатуры
   - при нажатии на поле ввода Password, появляется возможность ввода с клавиатуры
   - при введенных данных Username - "      " и Password - "secret_sauce", и при дальнейшем нажатии на кнопку LOGIN происходит ошибка - Epic sadface: Username is required

## Вариант с недействительным паролем

1. Предшествующие условия:
   - перейти на страницу авторизации https://www.saucedemo.com/
2. Шаги:
   - навести курсор и нажать на поле Username
   - не вводить логин
   - навести курсор и нажать на поле Password
   - ввести "QWER123"
   - нажать на кнопку LOGIN
3. Ожидаемый результат:
   - при нажатии на поле ввода Password, появляется возможность ввода с клавиатуры
   - при введенных данных Username - "       " и Password - "QWER123", и при дальнейшем нажатии на кнопку LOGIN происходит ошибка - Epic sadface: Username is required

## Вариант без пароля

1. Предшествующие условия:
   - перейти на страницу авторизации https://www.saucedemo.com/
2. Шаги:
   - навести курсор и нажать на поле Username
   - не вводить логин
   - поле Password остается пустым
   - нажать на кнопку LOGIN
3. Ожидаемый результат:
   - при нажатии на поле ввода Username, появляется возможность ввода с клавиатуры
   - при введенных данных Username - "       "  и при дальнейшем нажатии на кнопку LOGIN происходит ошибка - Epic sadface: Password is required.