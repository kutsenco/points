<h1 align="center">Hi there, I'm <a href="https://daniilshat.ru/" target="_blank">Max</a>
<img src="https://github.com/blackcater/blackcater/raw/main/images/Hi.gif" height="32"/></h1>
<h3 align="center">Computer science student, IT news writer from Ukraine</h3>
<h3 align="center">This is my cool emoji and why extend</h4>

## Extend, append, +=

## Метод extend()додає всі елементи iterable (список, кортеж, рядок тощо) у кінець списку.

# Синтаксис:

Тут усі елементи list2 додаються в кінці list1.

- list1 = [1, 2, 3, 4, 5]
- list2 = [6, 7]
- print(list1)

# Параметри extend():

Як згадувалося, extend()метод використовує ітераційний елемент, такий як:

- список
- кортеж
- рядок


## Повернене значення від extend():

# Метод extend():

- змінює вихідний список (list1) 
- він не повертає жодного значення.

# Приклад 1:

- languages1 = ['🎨', '👔']
- languages2 = ['🏸', '🧣']
- languages1.extend(languages2)
- print(languages1)

Вивід:

- ['🎨', '👔', '🏸', '🧣']

# Оператор +
також додавати елементи до списку можна через += (альтернатива extend)

> list1 = ['👩', '🦎']
> list2 = ['👦', '🐱']
> list1 += list2
> print(list1)

# Вивід:

['👩', '🦎', '👦', '🐱']

Також я досліджував результат виводу при двох алгоритмає:
- extend
- append

## Спершу дослідимо роботу extend:

- list1 = [1, 2]
- a = [3, 4]
- list1.append(a)
- print(list1)

# Вивід:

[1, 2, 3, 4]

## Дослідимо роботу append:

- list2 = [1, 2]
- b = [3, 4]
- list2.extend(b)
- print(list2)

# Вивід:

[1, 2, [3, 4]]

### Підсумок:

Використовуючи extend для додаванні елементу в список - він його додає розбиває доданий елемент на менші елементики, та додає їх окремо в результуючий список.
Використовуючи append для додаванні елементу в список - він його додає, як окремий елемент в резулятуючий список. (тобто без робиття його на менші підстанції)
Використовуючи += для додаванні елементу в список - він працює аналогічно до extend.
