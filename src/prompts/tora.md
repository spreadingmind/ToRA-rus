Интегрируй пошаговую логику и код на Python для решения математических задач, следуя следующим рекомендациям:

- Анализируйте вопрос и напишите функции для решения задачи; функция не должна принимать аргументов.
- Представьте окончательный результат в LaTeX, используя `boxed{}`, без указания единиц.
- Используйте символ `pi` и `Rational` из Sympy для $\pi$ и дробей, упрощайте все дроби и квадратные корни, не преобразуя их в десятичные значения.

Вот несколько примеров, на которые вы можете ссылаться:

---

Вопрос: У Оливии было 23 рубля. Она купила пять бубликов по 3 рубля каждый. Сколько денег у нее осталось?

Решение:
```python
def money_left():
    money_initial = 23
    bagels = 5
    bagel_cost = 3
    money_spent = bagels * bagel_cost
    remaining_money = money_initial - money_spent
    return remaining_money
 
remaining_money = money_left()
print(remaining_money)
```
```output
8
```
У Оливии осталось $boxed{8}$ долларов.

---

Вопрос: У Майкла было 58 мячей для гольфа. Во вторник он потерял 23 мяча. В среду он потерял еще 2. Сколько мячей для гольфа у него осталось к концу среды?

Решение:
```python
def remaining_golf_balls():
    golf_balls_initial = 58
    golf_balls_lost_tuesday = 23
    golf_balls_lost_wednesday = 2
    golf_balls_left = golf_balls_initial - golf_balls_lost_tuesday - golf_balls_lost_wednesday
    remaining_golf_balls = golf_balls_left
    return remaining_golf_balls

answer = remaining_golf_balls() 
print(answer)
```
```output
33
```
У Майкла осталось $boxed{33}$ мяча для гольфа к концу среды.

---

Вопрос: В серверной было девять компьютеров. С понедельника по четверг каждый день устанавливали по пять компьютеров. Сколько теперь компьютеров в серверной?

Решение:
```python
def total_computers():
    computers_initial = 9
    computers_per_day = 5
    num_days = 4  # 4 дня с понедельника по четверг
    computers_added = computers_per_day * num_days
    computers_total = computers_initial + computers_added
    return computers_total

total_computers = total_computers()
print(total_computers)
```
```output
29
```
Теперь в серверной $boxed{29}$ компьютеров.

---
