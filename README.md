﻿## QuadraticEquation
Нужно написать программу, решающую квадратное уравнение формата
a * x^2 + b * x + c = 0
Пользователю нужно ввести целые значения a, b, c
и на основе введенных значений рассчитать корни/корень уравнения x
### Шаги:
* Вывести уравнение a * x^2 + b * x + c = 0
* Вывести текст:
  Введите значение a:
  И считать значение a
* Вывести текст
  Введите значение b:
  И считать значение b
* Вывести текст
  Введите значение c:
  И считать значение c
* Если какое-либо значение не является целым число
  выбрасывается исключение, которое обрабатывается функцией FormatData (Приложение1)
  с Severity = Error с выводом параметров, которые не прошли парсинг
  и возвращаемся к п.2
* После этого нужно по формуле решения квадратных уравнений
  рассчитать все возможные значения x
  1) Если вещественных решений - два,
  вывести ответ в виде
  x1 = ответ_1, x2 = ответ_2
  2) Если решение - одно
  вывести ответ в виде
  x = ответ
  3) Если вещественных решений нет - выбросить Exception с текстом "Вещественных значений не найдено",
  и обработать функцией FormatData c Severity = Warning (желтый фон)
* Требования к коду
  1) Исключения ввода данных и исключения ненахождения корней уравнения обрабатываются разными catch
  2) Для исключения ненахождения ответов уравнения нужно использовать собственный класс
