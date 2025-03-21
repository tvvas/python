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

