# ILogger

Базовый класс используется для интерфейса с файлом crafttweaker.log и другими логгерами (такими как плейер).

Этот класс был добавлен модом с mod-id `crafttweaker`. Так что если вы хотите использовать эту функцию, вам нужно установить этот мод.

## Импорт класса
Вам может потребоваться импортировать пакет, если вы столкнетесь с какими-либо проблемами (например, с заливкой массива), так что лучше быть в безопасности, чем извиняться и добавлять импорт.
```zenscript
crafttweaker.api.ILogger
```

## Методы
### debug

Регистрирует отладочное сообщение.

```zenscript
logger.debug(сообщение как String);
logger.debug("message");
```

| Параметр  | Тип    | Описание             |
| --------- | ------ | -------------------- |
| сообщение | String | сообщение для входа. |


### ошибка

Регистрирует сообщение об ошибке.

```zenscript
logger.error(сообщение как строка);
logger.error("message");
```

| Параметр  | Тип    | Описание             |
| --------- | ------ | -------------------- |
| сообщение | String | сообщение для входа. |


### инфо

Регистрирует информационное сообщение.

```zenscript
logger.info(сообщение как строка);
logger.info("message");
```

| Параметр  | Тип    | Описание             |
| --------- | ------ | -------------------- |
| сообщение | String | сообщение для входа. |


### предупреждение

Регистрирует предупреждение.

```zenscript
logger.warning(сообщение как String);
logger.warning("message");
```

| Параметр  | Тип    | Описание             |
| --------- | ------ | -------------------- |
| сообщение | String | сообщение для входа. |



