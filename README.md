# Урок  7. Вложенные структуры. Домашнее задание <br>

---
Возможно вы смотрели старинную телепередачу "Своя игра". <br>
Там участники выбирают категорию и сумму, а телеведущий задает вопрос. <br>
Если ответ верный, то игрок получет очки, если неверный - теряет. <br>

---
> **main.py** - файл запуска программы <br>

**Шаг 1.** Сперва программа выводит игровое поле и предлагает ввыбрать вопрос:

```python
Транспорт  100  200  300
Животные   100  200  300
Еда        100  200  300
```

**Шаг 2.** Пользователь выбирает вопрос, программа задает его, пользователь отвечает, и программа говорит, сколько поинтов получено:

```python
Пользователь:
Транспорт 200
Программа:
Слово train в переводе означает
Пользователь:
Поезд
Программа:
Верно, +200. Ваш счет = 200
```
Если выбранного вопроса нет, то программа сообщает об этом:
```python
Пользователь:
Транспорт 400
Программа:
Такого вопроса нет, попробуйте еще раз!
```

**Шаг 3.** Затем программа снова выводит игровое поле, где использованный вопрос отсутствует:

```python
Транспорт 100       300
Животные  100  200  300
Еда       100  200  300
```
Пользователь снова выбирает вопрос, программа задает его, пользователь отвечает, программа говорит сколько поинтов получено.
```python
Пользователь:
Транспорт 300
Программа:
Слово boarding в переводе означает
Пользователь:
Абордаж
Программа:
Неверно, на самом деле - Посадка. - 300 Ваш счет = -100
```

**Шаг 4.** Когда игра заканчивается, пользователю выводится статистика:

```python
У нас закончились вопросы!
Ваш счет: 1200
Верных ответов: 5
Неверных ответов: 4
```

**Шаг 5.** Результаты записываются в общий список результатов в формате JSON с ключами:

```python
У нас закончились вопросы!
Ваш счет: 1200
Верных ответов: 5
Неверных ответов: 4
```


**Вопросы для игры**

```python
Транспорт

100  plane
200  train
300  boarding

Животные

100  dog  собака
200  shark  акула
300  sparrow  воробей

Еда

100  apple  яблоко
200  berry  ягода
300  venison  оленина
```