# Задача № 2 "Читаем логи"

## Краткое описание

1. Создан проект на базе Maven из архива.
2. Выполнена проверка кода плагином SpotBugs Maven Plugin v.3.1.12.2
3. Обнаружена ошибка RV_RETURN_VALUE_IGNORED_NO_SIDE_EFFECT
4. Ошибка исправлена, возвращаемое значение получено и выведено в консоль.

## Код

```java
System.out.println(service.calculate(amount, registered));
```
## Лог
```
 [INFO] --- spotbugs-maven-plugin:3.1.12.2:check (default-cli) @ bonus-calculator ---
 [INFO] BugInstance size is 0
 [INFO] Error size is 0
 [INFO] No errors/warnings found
 [INFO] ------------------------------------------------------------------------
 [INFO] BUILD SUCCESS
 [INFO] ------------------------------------------------------------------------
 [INFO] Total time:  8.994 s
 [INFO] Finished at: 2020-05-10T12:07:57+07:00
 [INFO] ------------------------------------------------------------------------
```