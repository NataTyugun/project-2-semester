# project-2-semester
from tkinter import *
from tkinter.ttk import Combobox

window = Tk()

window.title("Приложение :'Подсчёт калорий'")
window.geometry('620x620')

canvas = Canvas(window, height=500, width = 500)
canvas.pack()

frame = Frame(window, bg="lavender")
frame.place(relx=0.04, rely=0.04, relwidth=0.9, relheigh=0.9)

title=Label(frame, text="<дата>", bg="white", font=70)
title.pack()
btn = Button(frame,text = 'Кнопка', bg="pink",font=70)
btn.pack()
#не работает Combobox
combo = Combobox(window)  
combo['дата'] = (1, 2, 3, 4, 5, 'Текст')
combo.grid(column=0, row=0)
ombo.pack()


window.mainloop()
