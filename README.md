# Погружение в Python (семинары)
## Урок 6. Модули

### Задание 1
В модуль с проверкой даты добавьте возможность запуска в терминале с 
передачей даты на проверку.

### Задание 2
Добавьте в пакет, созданный на семинаре шахматный модуль. Внутри него напишите код, 
решающий задачу о 8 ферзях. Известно, что на доске 8×8 можно расставить 8 ферзей так, 
чтобы они не били друг друга. Вам дана расстановка 8 ферзей на доске, определите, 
есть ли среди них пара бьющих друг друга. Программа получает на вход восемь пар 
чисел, каждое число от 1 до 8 - координаты 8 ферзей. 
Если ферзи не бьют друг друга верните истину, а если бьют - ложь. 

### Задание 3
Напишите функцию в шахматный модуль. Используйте генератор случайных чисел для 
случайной расстановки ферзей в задаче выше. Проверяйте различный случайные варианты 
и выведите 4 успешных расстановки.

### Решение
**Задание 1**

Реализовано в файле ch_date.py и частично в файле main.py

**Задание 2 и 3**

Реализовано в файле main.py

Случайным образом не удалось сделать генерацию корректной расстановки 8 ферзей 
на шахматной доске (не удавалось найти корректную расстановку за адекватное время).
В место этого - была написана функция *chess.my_arrangement()*, которая предоставляет ВСЕ
корректные решения сразу (их всего 92 случая), а после - случайным образом выбираются
4 решения для тестирования.