# c_odigo
import math
def relativa(x1,y1,x2,y2):
    return math.sqrt((x2-x1)**2+(y2-y1)**2)
def aceleracion(re1):
    return 1/re1**2
def posicion(x0,v0,t,ac):
    v=v0+ac+t
    return v,x0+v0*t+0.5*ac*t*t
x0=0
v0=0.5
t=0.1
x1=float(input("Ingrese posicion x1: "))
y1=float(input("Ingrese posicion y1: "))
x2=float(input("Ingrese posicion x2: "))
y2=float(input("Ingrese posicion y2: "))
ac=aceleracion(relativa(x1,y1,x2,y2))
print("La aceleracion es: ",ac)
print("La nueva velocidad y posicion son: ", posicion(x0,vo,t,ac))
