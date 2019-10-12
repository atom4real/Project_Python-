from tkinter import *
import tkinter.messagebox
#DEV_INTOUCH KHURWONG

MainWindow = Tk()
MainWindow.title('X-and-O__DEV by Intouch_Khurwong')

def DisButton():
    bt1.config(state = DISABLED)
    bt2.config(state = DISABLED)
    bt3.config(state = DISABLED)
    bt4.config(state = DISABLED)
    bt5.config(state = DISABLED)
    bt6.config(state = DISABLED)
    bt7.config(state = DISABLED)
    bt8.config(state = DISABLED)
    bt9.config(state = DISABLED)

def CheckForWin():
    if (bt1['text'] == 'X' and bt2['text'] == 'X' and bt3['text'] == 'X' or 
        bt4['text'] == 'X' and bt5['text'] == 'X' and bt6['text'] == 'X' or
        bt7['text'] == 'X' and bt8['text'] == 'X' and bt9['text'] == 'X' or
        bt1['text'] == 'X' and bt5['text'] == 'X' and bt9['text'] == 'X' or
        bt3['text'] == 'X' and bt5['text'] == 'X' and bt7['text'] == 'X' or
        bt1['text'] == 'X' and bt4['text'] == 'X' and bt7['text'] == 'X' or
        bt2['text'] == 'X' and bt5['text'] == 'X' and bt8['text'] == 'X' or
        bt3['text'] == 'X' and bt6['text'] == 'X' and bt9['text'] == 'X'):
        tkinter.messagebox.showinfo('X-and-O', "Player X's Winning")
        DisButton()

    elif(bt1['text'] == 'O' and bt2['text'] == 'O' and bt3['text'] == 'O' or 
         bt4['text'] == 'O' and bt5['text'] == 'O' and bt6['text'] == 'O' or
         bt7['text'] == 'O' and bt8['text'] == 'O' and bt9['text'] == 'O' or
         bt1['text'] == 'O' and bt5['text'] == 'O' and bt9['text'] == 'O' or
         bt3['text'] == 'O' and bt5['text'] == 'O' and bt7['text'] == 'O' or
         bt1['text'] == 'O' and bt4['text'] == 'O' and bt7['text'] == 'O' or
         bt2['text'] == 'O' and bt5['text'] == 'O' and bt8['text'] == 'O' or
         bt3['text'] == 'O' and bt6['text'] == 'O' and bt9['text'] == 'O'):
        tkinter.messagebox.showinfo('X-and-O', "Player O's Winning")
        DisButton()

    elif count > 8:
        tkinter.messagebox.showinfo('X-and-O', 'No one winning. Try again!')
        DisButton()

Click = True
count = 0

def Clickbut(btn):
    global Click , count
    if btn['text'] == '' and Click == True:
        btn['text'] = 'X'
        Click = False
        count += 1
        CheckForWin()

    elif btn['text'] == '' and Click == False:
        btn['text'] = 'O'
        Click = True
        count += 1
        CheckForWin()
    
    else:
        tkinter.messagebox.showinfo('X-and-O', 'Button already Clicked!')


bt1 = Button(MainWindow, text = '' ,font = 'Impact' ,bg = 'Dark gray' ,fg = 'red' ,height = 6 ,width = 12 ,command = lambda: Clickbut(bt1))
bt1.grid(row = 0, column = 0)

bt2 = Button(MainWindow, text = '' ,font = 'Impact' ,bg = 'Dark gray' ,fg = 'red' ,height = 6 ,width = 12 ,command = lambda: Clickbut(bt2))
bt2.grid(row = 0, column = 1)

bt3 = Button(MainWindow, text = '' ,font = 'Impact' ,bg = 'Dark gray' ,fg = 'red' ,height = 6 ,width = 12 ,command = lambda: Clickbut(bt3))
bt3.grid(row = 0, column = 2)

bt4 = Button(MainWindow, text = '' ,font = 'Impact' ,bg = 'Dark gray' ,fg = 'red' ,height = 6 ,width = 12 ,command = lambda: Clickbut(bt4))
bt4.grid(row = 1, column = 0)

bt5 = Button(MainWindow, text = '' ,font = 'Impact' ,bg = 'Dark gray' ,fg = 'red' ,height = 6 ,width = 12 ,command = lambda: Clickbut(bt5))
bt5.grid(row = 1, column = 1)

bt6 = Button(MainWindow, text = '' ,font = 'Impact' ,bg = 'Dark gray' ,fg = 'red' ,height = 6 ,width = 12 ,command = lambda: Clickbut(bt6))
bt6.grid(row = 1, column = 2)

bt7 = Button(MainWindow, text = '' ,font = 'Impact' ,bg = 'Dark gray' ,fg = 'red' ,height = 6 ,width = 12 ,command = lambda: Clickbut(bt7))
bt7.grid(row = 2, column = 0)

bt8 = Button(MainWindow, text = '' ,font = 'Impact' ,bg = 'Dark gray' ,fg = 'red' ,height = 6 ,width = 12 ,command = lambda: Clickbut(bt8))
bt8.grid(row = 2, column = 1)

bt9 = Button(MainWindow, text = '' ,font = 'Impact' ,bg = 'Dark gray' ,fg = 'red' ,height = 6 ,width = 12 ,command = lambda: Clickbut(bt9))
bt9.grid(row = 2, column = 2)

#DEV_INTOUCH KHURWONG
MainWindow.mainloop()
