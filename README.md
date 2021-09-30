# gvaluer
Code smells finding practice

# Code smells:

  * Название методов в стиле snake_case, хотя в С++ принято называть в стиле CamelCase
  * Неверная расстановка {} в классах и методах (fixed)
  * Нет комментариев к глобальным переменным
  * Bloaters: огромный main, выполнен рефакторинг функций.
  * Bloaters: очень большой метод parse_group, трудно сказать что он делает и изменить без входных данных
  * Primitive Obsession: 20 полей в классе Group, можно разбить на несколько структур, но, опять же, трудно понять по переменным что к чему относится, нигде нет комментариев.
  * Primitive Obsession: аналогично в классе ConfigParser
  * Switch Statements: метод parse_status
  * Shotgun Surygery: при изменении класса Group нужно будет менять класс ConfigParser
  * Повторение кода в методе parse_group класса ConfigParser
