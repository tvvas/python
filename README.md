Практична робота 12

1. Запустити програму IDLE (в меню Пуск -> Python -> IDLE)
2. Створити новий файл (File -> New File)
3. Зберегти файл (File -> Save File As...)
4. Скопіювати і вставити наступний код

```python
https://github.com/tvvas/python

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
