from tkinter import *

top=Tk()
top.title("Calculator By Aman")
top.geometry("300x250")
top.resizable(0,0)
c=Canvas(top,bg="grey",height="270",width="320")
c.pack()
value=""
def btn1():
    global value
    value=value + "1"
    scvalue.set(value)

def btn2():
    global value
    value=value + "2"
    scvalue.set(value)

def btn3():
    global value
    value=value + "3"
    scvalue.set(value)

def btn4():
    global value
    value=value + "4"
    scvalue.set(value)

def btn5():
    global value
    value=str(eval(value))
    scvalue.set(value)

def btn6():
    global value
    value=value+"+"
    scvalue.set(value)

def btn7():
    global value
    value=value+"-"
    scvalue.set(value)

def btn8():
    global value
    value=value+"*"
    scvalue.set(value)

def btn9():
    global value
    value=value+"/"
    scvalue.set(value)

def btn10():
    global value
    value=value + "5"
    scvalue.set(value)


def btn11():
    global value
    value=value + "6"
    scvalue.set(value)

def btn12():
    global value
    value=value + "7"
    scvalue.set(value)

def btn13():
    global value
    value=value + "8"
    scvalue.set(value)

def btn14():
    global value
    value=value + "9"
    scvalue.set(value)

def btn15():
    global value
    value=value + "0"
    scvalue.set(value)

def btn16():
    global value
    value=value + "."
    scvalue.set(value)

def btn17():
    global value
    value=value + "("
    scvalue.set(value)

def btn18():
    global value
    value=value + ")"
    scvalue.set(value)

def btn19():
    global value
    value=""
    scvalue.set(value)

def btn20():
    global value
    list1=list(value)
    list1.pop()
    value="".join(list1)
    scvalue.set(value)

    
scvalue=StringVar()

e1=Entry(top,textvariable=scvalue).place(x="80",y="20")

b1=Button(top,text="1",padx="8",command=btn1).place(x=50,y=50)
b2=Button(top,text="2",padx="8",command=btn2).place(x=90,y=50)
b3=Button(top,text="3",padx="8",command=btn3).place(x=130,y=50)
b4=Button(top,text="4",padx="8",command=btn4).place(x=170,y=50)


b7=Button(top,text="-",padx="8",command=btn7).place(x=210,y=170)
b8=Button(top,text="*",padx="8",command=btn8).place(x=170,y=130)
b9=Button(top,text="/",padx="8",command=btn9).place(x=170,y=170)

b10=Button(top,text="5",padx="8",command=btn10).place(x=50,y=90)
b11=Button(top,text="6",padx="8",command=btn11).place(x=90,y=90)
b12=Button(top,text="7",padx="8",command=btn12).place(x=130,y=90)
b13=Button(top,text="8",padx="8",command=btn13).place(x=170,y=90)

b14=Button(top,text="9",padx="8",command=btn14).place(x=50,y=130)
b15=Button(top,text="0",padx="8",command=btn15).place(x=90,y=130)
b16=Button(top,text=".",padx="8",command=btn16).place(x=130,y=130)

b17=Button(top,text="(",padx="8",command=btn17).place(x=90,y=170)
b18=Button(top,text=")",padx="8",command=btn18).place(x=130,y=170)
b19=Button(top,text="C",padx="8",command=btn19).place(x=50,y=170)
b20=Button(top,text="bp",padx="7",command=btn20).place(x=210,y=130)

b6=Button(top,text="+",pady="21",padx="10",command=btn6).place(x=210,y=50)
b5=Button(top,text="=",padx="10",command=btn5).place(x=210,y=170)
top.mainloop()
