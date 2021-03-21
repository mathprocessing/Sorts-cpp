# Описание
* Пусть определена коллекция случайных чисел
Это могут быть как целые числа (если нам надо что-то отсортировать)
так и ассоциативный массив т.е. ключ-значение
  1. Целые числа
  => сравниваем числа
  2. Ассоциативный массив пар ключ-значение (ключ указывает на произвольный тип данных)
  => сравниваем ключи
  В обоих случаях должно выполняться свойство транзитивности операции сравнения
  transitivity: forall a b c, a < b and b < c => a < c

* Пусть дана коллекция [7, 1, 3, 2, 5, 8, 4, 6]
Тогда в конце должна быть отсортированная последовательность [1, 2, .., 8]

Мы начинаем сортировку вставками с разбиения коллеции на две части:
1. [7] единственный элемент слева
2. [1, 3, 2, 5, 8, 4, 6]

## Этап 1
Смотрим на левую (1-ую) коллекцию и видим один единственный элемент
поэтому можем применить лемму: forall (A: List)(x : T), sorted [x]

## Этап 2

