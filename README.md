# David-Hoyos-Reto4
##1. Dado un número entero, determinar si ese número corresponde al código ASCII de una vocal minúscula.
```
x= int(input("Ingrese el numero: "))

vocal = chr(x)

if vocal == "a" or vocal == "e" or vocal == "i" or vocal == "o" or vocal == "u":
    print(f"El numero {x} corresponde al codigo ASCII de una vocal minúscula")

else:
    print(f"El numero {x} NO corresponde al codigo ASCII de una vocal minúscula")
```

##2.Dada una cadena de longitud 1, determine si el código ASCII de primera letra de la cadena es par o no.
```
x = str(input("Ingresa un caracter"))
y = x[0]
if ord(y) % 2 == 0:
    print("El codigo ASCII de la primera letra es par")
else: 
    print("El codigo ASCII de la primera letra no es par")
```

##3.Dado un carácter, construya un programa en Python para determinar si el carácter es un dígito o no.
```
x = input("Ingresa un unico digito:")
if x in ("1", "2", "3", "4", "5", "6", "7", "8", "9", "0"):
    print("Si es un digito")
else: 
    print("No es un digito")
```

##4.Dado un número real x, construya un programa que permita determinar si el número es positivo, negativo o cero. Para cada caso de debe imprimir el texto que se especifica a continuación:
```
x = float(input("Ingrese un numero real"))
if x < 0:
    print("El número x es negativo")
elif x > 0:
    print("El número x es positivo")
else:
    print("El número x es el neutro para la suma")
```

##5. Dado el centro y el radio de un círculo, determinar si un punto de R2 pertenece o no al interior del círculo.

```
centroX = float(input("Ingrese la coordenada del centro en x: "))
centroY = float(input("Ingrese la coordenada en y: "))
radio = float(input("Ingrese el radio del circulo: "))
x = float(input("Ingrese la coordenada del punto en y: "))
y = float(input("Ingrese la coordenada del punto en y: "))
PI = 3.14159
area= PI * radio**2
distancia = (x - centroX)**2 + (y- centroY)**2
if  distancia < area:
    print("El punto se encuentra dentro del circulo")
else:
    print("El punto no se encuentra dentro del circulo")
```

##6. Dadas tres longitudes positivas, determinar si con esas longitudes se puede construir un triángulo.

```
c1= int(input("Ingrese la longitud del primer cateto "))
c2 = int(input("Ingrese la longitud del segundo cateto "))
h= int(input("Ingrese la longitud de la hipotenusa "))

if c1**2 + c2**2 == h**2:
    print("Con las 3 longitudes se puede formar un triangulo rectangulo.")
elif c1 + c2 == h and c2 + h > c1 and h + c1 > c2:
    print("Con las 3 longitudes se puede formar un triangulo.")
else:
    print("Con las 3 longitudes no se puede formar un triangulo.")
```
