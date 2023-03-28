# Reto7
Solución planteamientos en el reto 7

### 1. Imprimir un listado con los números del 1 al 100 cada uno con su respectivo cuadrado.
```
    a:int=1
    while a<=100:
        print(str(a)+ " y su cuadrado es " + str(a**2))
       a +=1
```

### 2. Imprimir un listado con los números impares desde 1 hasta 999 y seguidamente otro listado con los números pares desde 2 hasta 1000.
```
x:int=1

y:int=0
while x<=999:
    print(str(x)+ " es impar")
    x +=2
while y<=1000:
    print(str(y)+ " es par")
    y+=2
```

### 3. Imprimir los números pares en forma descendente hasta 2 que son menores o iguales a un número natural n ≥ 2 dados.
```
n=int(input("ingrese un numero"))
while n>=2: 
    z=n%2
    if z==0:
        print(str(n))
        n-=2
    if z!=0:
        n-=1
```

### 4. En 2022 el país A tendrá una población de 25 millones de habitantes y el país B de 18:9 millones. Las tasas de crecimiento anual de la población serán de 2% y 3% respectivamente. Desarrollar un algoritmo para informar en que año la población del país B superará a la de A.
```
PaisA=int=25000000
PaisB=int=18900000
Año=int=1
while PaisB<PaisA:
    PaisA*=1.02# esto ya que se le esta sumando deuna el 2% extra a la pobracion que se tenia anteriormente
    PaisB*=1.03# esto ya que se le esta sumando deuna el 2% extra a la pobracion que se tenia anteriormente
    Año+=1
print("para el año "+ str(Año)+" la pobracion de B("+str(PaisB)+") sera mayor que la pobracion de A("+str(PaisA)+")")
```

### 5. Imprimir el factorial de un número natural n dado.
```
n=int(input("ingrese un numero al que le quiera sacar su factorial"))
x=int=n
while x>1:
    x-=1
    n*=x

print (n)
```

### 6. Implementar un algoritmo que permita adivinar un número dado de 1 a 100, preguntando en cada caso si el número es mayor, menor o igual.
```
a=int(input("numero del 1 al 100"))
b=50
while a!=b:
   if b<a:
      b +=1
   else:
      b-=1
print("el numero es "+str(b))
```

### 7. Implementar un programa que ingrese un número de 2 a 50 y muestre sus divisores.
```
a=int(input("ingrese un numero del 2 al 50"))
x=1
while x<=a:
    if a%x==0:
        print(str(x))
    x+=1
```

### 8. Implementar el algoritmo que muestre los números primos del 1 al 100. nota: use funciones
```
def numeros_primos(n : int,):
        i = int(2) 
        if n == 2 : 
             print(n)
        while i < n :
            if n%i == 0: 
                break 
            elif i == n-1: 
                print(n) 
            i += 1 

if __name__ == "__main__" :
    a = int(2) 
    Lim= 100 
    while a < Lim: 
        a = numeros_primos(a) 
        a += 1 
```
