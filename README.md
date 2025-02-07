# Math
Реализация версии математической библиотеки math.h на языке C. Эта библиотека реализует базовые математические операции, которые затем используются в различных алгоритмах. 

## Содержание
- [Обзор некоторых функций "math.h"](#обзор-некоторых-функций-mathh)
- [Технологии](#технологии)
- [Использование](#использование)
- [Разработка](#разработка)
- [Тестирование](#тестирование)

## Обзор некоторых функций "math.h"

| No. | Function | Description |
| --- | -------- | ----------- |
| 1 | `int abs(int x)` | вычисляет абсолютное значение целого числа |
| 2 | `long double acos(double x)` | вычисляет арккосинус |
| 3 | `long double asin(double x)` | вычисляет арксинус |
| 4 | `long double atan(double x)` | вычисляет арктангенс |
| 5 | `long double ceil(double x)` | возвращает ближайшее целое число, не меньшее заданного значения |
| 6 | `long double cos(double x)` | вычисляет косинус |
| 7 | `long double exp(double x)` | возвращает значение e, возведенное в заданную степень |
| 8 | `long double fabs(double x)` | вычисляет абсолютное значение числа с плавающей точкой |
| 9 | `long double floor(double x)` | возвращает ближайшее целое число, не превышающее заданное значение |
| 10 | `long double fmod(double x, double y)` | остаток операции деления с плавающей точкой |
| 11 | `long double log(double x)` | вычисляет натуральный логарифм |
| 12 | `long double pow(double base, double exp)` | возводит число в заданную степень |
| 13 | `long double sin(double x)` | вычисляет синус |
| 14 | `long double sqrt(double x)` | вычисляет квадратный корень |
| 15 | `long double tan(double x)` | вычисляет тангенс |  

## Технологии
- язык С
- check.h
- Makefile
- make
- gcov
- clang-format

## Использование

1. Для установки проекта необходимо склонировать репозиторий, перейти в папку `./C_Math/src`

2. Скомпилировать и запустить проект: 
```sh
make
```
или 

```sh
make all
```
или
```sh
make rebuld
```
При вводе данной команды проект компилируется, запускаются тесты, открывается html страница, отображающая покрытие тестами

3. Запуск тестов
```sh
make test
``` 
4. Генерация файла .o
```sh
make s21_math.o
```
5. Отображение покрытия тестами
```sh
make gcov_report
```
6. Запуск unit-тестов
```sh
make check
```
7. Очистка проекта
```sh
make clean
```

## Разработка
- Реализация некоторых функций библиотеки [**math.h**](#обзор-некоторых-функций-mathh)
- Библиотека разработана на языке Си стандарта C11 с использованием компиятора gcc 
- Ориентировка на стандарт POSIX.1-2017
- Реализация придерживается Google Style
- Решение оформлено в виде статической бибилотеки
- В цели gcov_report формируется отчёт gcov в виде html страницы. Для этого unit-тесты запускаются с флагами gcov  
- Makefile для сборки библиотеки и тестов
- Общая проверяемая точность - 16 значащих цифр
- Проверяемая точность дробной части - максимум 6 знаков после запятой.

## Тестирование
- Присутствует полное покрытие unit-тестами функций библиотеки c помощью библиотеки `Check.h`
- Unit-тесты проверяют результаты работы реализации путём сравнения ее с реализацией стандартной библиотеки math.h
- Unit-тесты покрывают около 90% каждой функции

### Причина разработки данного проекта
Учебное задание в Школе 21 от Сбера

## Команда проекта
- [Анна Б.](https://github.com/BalagurovaA)
- [Аделина Ш.](https://github.com/llllenivka)
