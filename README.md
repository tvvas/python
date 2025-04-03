# Практична робота 12

1. Запустити програму IDLE (в меню Пуск -> Python -> IDLE)
2. Створити новий файл (File -> New File)
3. Зберегти файл (File -> Save File As...)
4. Скопіювати і вставити наступний код

```python
from tkinter import *
from turtle import *

def draw_graphics():
    # Малюємо 
    t.forward(100)
    t.right(90)

def clear_graphics():
    # Очищуємо екран
    t.clear()

# Глобальне вікно turtle та черепашка
screen = Screen()
screen.setup(width=800, height=600)

t = Turtle()  # Створюємо черепашку

# Головна програма Tkinter
tk = Tk()

# Додаємо кнопки
button_draw = Button(tk, text="Намалювати", command=draw_graphics)
button_draw.pack(pady=10)

button_clear = Button(tk, text="Очистити екран", command=clear_graphics)
button_clear.pack(pady=10)

# Запускаємо головний цикл Tkinter
tk.mainloop()
```

5. Запустити програму на виконання (Run -> Run Module)
6. Переконатися, що появилося вікно із кнопками і вікно для малювання
7. Натиснути на кнопки у вікні, перевірити що відбувається
8. Змінити програму так, щоб при натисканні кнопки було зображено коло (можна скористатися довідкою https://pythonsandbox.com/docs/turtle)
9. Пояснити кожен рядок програми

# Практична робота 13

1. Запустити програму IDLE (в меню Пуск -> Python -> IDLE)
2. Створити новий файл (File -> New File)
3. Зберегти файл (File -> Save File As...)
4. Скопіювати і вставити код із попередньої практичної роботи
5. Додати кнопку і назвати її "Квадрат"
6. Написати функцію `draw_k()`, яка будує квадрат
7. Зробити так, щоб при натисканні на кнопку "Квадрат" був зображений квадрат

# Практична робота 14

1. Запустити програму IDLE (в меню Пуск -> Python -> IDLE)
2. Створити новий файл (File -> New File)
3. Зберегти файл (File -> Save File As...)
4. Скопіювати і вставити наступний код

```python
from tkinter import *
tk = Tk()
tk.geometry("300x250")

def click():
    label_greeting.config(text="Привіт,"+entry1.get())

label1 = Label(text="Ім'я")
entry1 = Entry()    

btn = Button(text="Привітання", command=click)

label_greeting = Label()

label1.place(x=50, y=20, width=110, height=35)
entry1.place(x=150, y=20, width=110, height=35)
btn.place(x=100, y=100, width=110, height=35)
label_greeting.place(x=100, y=140, width=110, height=35)
```

5. Запустити програму на виконання (Run -> Run Module)
6. Переконатися, що появилося вікно із текстовим полем і кнопкою
7. Ввести ім'я у текстове поле і натиснути на кнопку. Переконатися, що появиться привітання
8. Пояснити кожен рядок коду
9. Змінити програму так, щоб появилося поле "Прізвище" і при введенні імені і прізвища та натисканні кнопки виводилося відповідне привітання

# Практична робота 15

1. Запустити програму IDLE (в меню Пуск -> Python -> IDLE)
2. Створити новий файл (File -> New File)
3. Зберегти файл (File -> Save File As...)
4. Скопіювати і вставити наступний код
   
```python
from tkinter import *
from turtle import *

def draw_graphics():
    # Малюємо
    x = entry.get()
    x = int(x)
    t.forward(x)
    t.right(90)

def clear_graphics():
    # Очищуємо екран
    t.clear()

# Глобальне вікно turtle та черепашка
screen = Screen()
screen.setup(width=800, height=600)

t = Turtle()  # Створюємо черепашку

# Головна програма Tkinter
tk = Tk()

# Додаємо текстове поле
entry = Entry(tk)
entry.pack(pady=10)

# Додаємо кнопки
button_draw = Button(tk, text="Намалювати", command=draw_graphics)
button_draw.pack(pady=10)

button_clear = Button(tk, text="Очистити екран", command=clear_graphics)
button_clear.pack(pady=10)

# Запускаємо головний цикл Tkinter
tk.mainloop()
```

5. Запустити програму на виконання (Run -> Run Module)
6. Переконатися, що появилося вікно із текстовим полем і кнопками
7. Ввести число 100 у текстове поле і натиснути кнопку "Намалювати". Переконатися, що буде побудовано відрізок
8. Змінити число на 50 у текстовому полі і натиснути кнопку "Намалювати". Переконатися, що буде побудовано відрізок меншої довжини
10. Пояснити кожен рядок коду

# Практична робота 16

1. Відкрити код із попередньої роботи
2. Додати кнопку і назвати її "Коло". Таким чином має бути три кнопки
3. Зробити так, щоб при натисканні на кнопку "Коло" було побудоване коло із радіусом, введеним у текстове поле
4. Продемонструвати роботу програми
5. Пояснити кожен рядок коду

# Практична робота 17

1. Відкрити код із роботи 15
2. Додати ще одне текстове поле
3. Змінити назву кнопки "Намалювати" на "Прямокутник"
4. Зробити так, щоб при натисканні на кнопку "Прямокутник" було побудовано прямокутник із довжиною, введеною у перше текстове поле, і шириною, введеною у друге текстове поле
5. Продемонструвати роботу програми
6. Пояснити кожен рядок коду

# Практична робота 18

1. Запустити програму IDLE (в меню Пуск -> Python -> IDLE)
2. Створити новий файл (File -> New File)
3. Зберегти файл (File -> Save File As...)
4. Скопіювати і вставити наступний код

```python
from tkinter import *
from turtle import *



def draw_graphics():
    # Малюємо
    x = entry1.get()
    x = int(x)
    t.left(90)
    t.forward(x)

def clear_graphics():
    # Очищуємо екран
    t.clear()

# Глобальне вікно turtle та черепашка
screen = Screen()
screen.setup(width=800, height=600)

t = Turtle()  # Створюємо черепашку


tk = Tk()

# Перший рядок: Label і Entry
label1 = Label(tk, text="Довжина сходинки:")
label1.grid(row=0, column=0, padx=5, pady=5)

entry1 = Entry(tk)
entry1.grid(row=0, column=1, padx=5, pady=5)

# Другий рядок: Label і Entry
label2 = Label(tk, text="Кількість сходинок:")
label2.grid(row=1, column=0, padx=5, pady=5)

entry2 = Entry(tk)
entry2.grid(row=1, column=1, padx=5, pady=5)

# Додаємо кнопки
button_draw = Button(tk, text="Намалювати сходи", command=draw_graphics)
button_draw.grid(row=2, column=0, columnspan=2, padx=5, pady=5)

button_clear = Button(tk, text="Очистити екран", command=clear_graphics)
button_clear.grid(row=3, column=0, columnspan=2, padx=5, pady=5)


root.mainloop()
```
5. Дописати код так, щоб при натисканні кнопки було побудовано введену кількість сходинок. Інформацію про цикли можна знайти тут https://www.w3schools.com/python/python_for_loops.asp
