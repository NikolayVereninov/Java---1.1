# Отчёт о тестировании Money Transfer

## Краткое описание

22.11.21 - 22.11.21 было проведено тестирование приложения  Money Transfer

На тестирование затрачено: 00:30

В результате тестирования выявлены следующие дефекты:
 ** integer number too large **
скриншот   ![image](https://user-images.githubusercontent.com/89935534/142914394-7065c950-9db9-4a17-8cf5-5a8748ebcf12.png)

## Описание процесса тестирования

В процессе тестирования использовались следующие артефакты*:
Использовал чек-лист допустимых значений и не допустимых значений.

В качестве тестовых данных использовались данные 
* данные с задачи *2_000_000_000 + 500_000_000* ожидаемый результат *2_500_000_000*
* Фактический результат *integer number too large*
* произвольные значения 2_000_000_000 + 147_000_000 ожидаемый результат 2_147_000_000 
* Фактический результат 2_147_000_000 
* произвольное значения 2_000_000_000 + 449_000_000 ожидаемый  результат 2_449_000_000
* Фактический результат  *integer number too large*

Тестирование производилось в следующем окружении:
* версия и разрядность ОС Windows 10 Home 64 bit
* версия Java 11
