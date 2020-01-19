# Форма регистрации v0.1.0

[Демо](https://dimukko.github.io/regex-form-validation)


## Поля с валидацией

- Имя
- Телефон
- Почта
- Url

## Условия выполнения валидации

### Имя

1. только кириллица;
2. первая буква заглавная;
3. можно ввести от 2 до 20 символов — это можно задать в атрибутах `minlength` и `maxlength`;
4. возможна запись двойных имён — например Анна-Мария.

### Почта

1. только латиница;
2. «собака» `@` — обязательный символ;
3. Точка `.` — тоже обязательный символ;
4. Цифры, подчерк, тире — разрешённые символы.

### Телефон

Шаблон для телефона должен находить номера в таких форматах:

```
+7(925)900-90-90
+7(925) 900-90-90
+7 925-900-90-90
+79259009090
89259009090
```

### Сайт

Адрес сайта должен:

1. начинаться с `http://` или `https://`;
2. затем `www.` — это необязательная группа;
3. IP-адрес — `255.255.255.255` или доменное имя — `stasbasov.ru`
4. порт — тоже необязательная группа. Порт начинается с двоеточия, за которым идут от 2 до 5 цифр. Например: `:8080`;
5. путь — последовательность из цифр, слешей и латинских букв, на конце которого может стоять решётка `#`.