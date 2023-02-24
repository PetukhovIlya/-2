from tkinter import *
from tkinter import ttk
 
def click_button():
     label["text"] = "Привет "+entry.get()
     entry.insert(0,"")

root = Tk()
root.title("Моя программа")
root.geometry("250x200")

entry = ttk.Entry()
entry.pack(anchor=NW, padx=6, pady=6)

label = ttk.Label(text="Представьтесь!")
label.pack(anchor=NW, padx=6, pady=6)

# стандартная кнопка
btn = ttk.Button(text="Кнопка", command=click_button)
btn.pack()
 
root.mainloop()
