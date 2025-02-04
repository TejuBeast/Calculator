from tkinter import *
window=Tk()
window.title("Teju's calculator")
window.geometry("442x490")
def bt(n):
    global equation
    equation=equation+str(n)
    userl.set(equation)
def eqn():
    global equation
    if equation=="":
            equation="type smtg lilkid"
            userl.set(equation)
    else:
        try:
            l=eval(equation)
            userl.set(l)
            equation=str(l)
        except SyntaxError:
            equation=''
            userl.set("syntax error")
def clr():
    global equation
    equation=""
    userl.set(equation)
def de():
    global equation
    if equation!="":
        l=list(equation)
        del l[-1]
        equation="".join(l)
        userl.set(equation)
equation=""
userl=StringVar()
userl.set("")
label=Label(window,textvariable=userl,font=("CenturyGothic",50),fg="black",bg="white",height=2)
label.grid(row=0,column=0,columnspan=4,sticky="ew")
frame=Frame(window)
frame.grid(row=1, column=0, sticky="w")
bt1=Button(frame,text="1",font=("CenturyGothic",20),fg="white",bg="black",height=2,width=4,command=lambda: bt(1))
bt1.grid(row=0,column=0)
bt2=Button(frame,text="2",font=("CenturyGothic",20),fg="white",bg="black",height=2,width=4,command=lambda: bt(2))
bt2.grid(row=0,column=1)
bt3=Button(frame,text="3",font=("CenturyGothic",20),fg="white",bg="black",height=2,width=4,command=lambda: bt(3))
bt3.grid(row=0,column=2)
bt4=Button(frame,text="4",font=("CenturyGothic",20),fg="white",bg="black",height=2,width=4,command=lambda: bt(4))
bt4.grid(row=1,column=0)
bt5=Button(frame,text="5",font=("CenturyGothic",20),fg="white",bg="black",height=2,width=4,command=lambda: bt(5))
bt5.grid(row=1,column=1)
bt6=Button(frame,text="6",font=("CenturyGothic",20),fg="white",bg="black",height=2,width=4,command=lambda: bt(6))
bt6.grid(row=1,column=2)
bt7=Button(frame,text="7",font=("CenturyGothic",20),fg="white",bg="black",height=2,width=4,command=lambda: bt(7))
bt7.grid(row=2,column=0)
bt8=Button(frame,text="8",font=("CenturyGothic",20),fg="white",bg="black",height=2,width=4,command=lambda: bt(8))
bt8.grid(row=2,column=1)
bt9=Button(frame,text="9",font=("CenturyGothic",20),fg="white",bg="black",height=2,width=4,command=lambda: bt(9))
bt9.grid(row=2,column=2)
bt0=Button(frame,text="0",font=("CenturyGothic",20),fg="white",bg="black",height=2,width=4,command=lambda: bt(0))
bt0.grid(row=3,column=0,columnspan=3,sticky="ew")
plus=Button(frame,text="+",font=("CenturyGothic",20),fg="white",bg="grey",height=2,width=4,command=lambda: bt("+"))
plus.grid(row=0,column=3)
minus=Button(frame,text="-",font=("CenturyGothic",20),fg="white",bg="grey",height=2,width=4,command=lambda: bt("-"))
minus.grid(row=1,column=3)
multiply=Button(frame,text="x",font=("CenturyGothic",20),fg="white",bg="grey",height=2,width=4,command=lambda: bt("*"))
multiply.grid(row=2,column=3)
div=Button(frame,text="/",font=("CenturyGothic",20),fg="white",bg="grey",height=2,width=4,command=lambda: bt("/"))
div.grid(row=0,column=4)
dec=Button(frame,text=".",font=("CenturyGothic",20),fg="white",bg="grey",height=2,width=4,command=lambda: bt("."))
dec.grid(row=1,column=4)
b1=Button(frame,text="(",font=("CenturyGothic",20),fg="white",bg="grey",height=2,width=4,command=lambda: bt("("))
b1.grid(row=3,column=3)
b2=Button(frame,text=")",font=("CenturyGothic",20),fg="white",bg="grey",height=2,width=4,command=lambda: bt(")"))
b2.grid(row=3,column=4)
d=Button(frame,text="del",font=("CenturyGothic",20),fg="white",bg="grey",height=2,width=4,command=lambda: de())
d.grid(row=3,column=5)
equal=Button(frame,text="=",font=("CenturyGothic",20),fg="black",bg="orange",height=2,width=4,command=lambda: eqn())
equal.grid(row=2,column=4,columnspan=2,sticky="ew")
clear=Button(frame,text="clr",font=("CenturyGothic",20),fg="white",bg="black",height=2,width=4,command=lambda: clr())
clear.grid(row=0,rowspan=2,column=5,sticky="ns")
window.mainloop()
