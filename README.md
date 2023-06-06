# Me-voy-a-quedar-calvo-por-este-estres
El dia de hoy realizaremos el reto 12 de la clase de programacion. Antes de comenzar el dato inneceseario de el dia va a ser:
#### Dato innecesario del dia 

[![Dato-inecesario-del-dia.png](https://i.postimg.cc/BQjwqQX9/Dato-inecesario-del-dia.png)](https://postimg.cc/Xp0gLWfQ)

Despues del estupendo pero innecesario dato del dia o del reto, empezaremos ahora si con lo que nos piden.
# Primera parte
1. Consulte que hacen los siguientes métodos de strings en python: endswith, startswith, isalpha, isalnum, isdigit, isspace, istitle, islower, isupper.
##### Endswith
El endswith es un método que devuelve True si la cadena termina con el valor especificado, de lo contrario, False.
```python
txt = "Hello, welcome to my world."

x = txt.endswith(".")

print(x)
```
#### Startswith 
El startswith es un método que devuelve True si la cadena comienza con el valor especificado; de lo contrario, False.
```python
txt = "Hello, welcome to my world."

x = txt.startswith("Hello")

print(x)
```
#### Isalpha 
El isalpha es un método que devuelve True si todos los caracteres son letras del alfabeto (az).
```python
txt = "CompanyX"

x = txt.isalpha()

print(x)
```
#### Isalnum
El isalnum es un método que devuelve True si todos los caracteres son alfanuméricos, es decir, letras del alfabeto (az) y números (0-9).
```python
txt = "50800"

x = txt.isdigit()

print(x)
```
#### Isdigit
El isdigit es un método que devuelve True si todos los caracteres son dígitos, de lo contrario, False.
```python
txt = "   "

x = txt.isspace()

print(x)
```
#### Isspace 
El isspace es un método que devuelve True si todos los caracteres de una cadena son espacios en blanco; de lo contrario, False.
```python
txt = "Hello, welcome to my world."

x = txt.endswith(".")

print(x)
```

#### Istitle 
El istitle es un método que devuelve True si todas las palabras en un texto comienzan con una letra mayúscula, Y el resto de la palabra son letras minúsculas; de lo contrario, False.
```python
txt = "Hello, And Welcome To My World!"

x = txt.istitle()

print(x)
```
#### Islower
El islower es un método que devuelve True si todos los caracteres están en minúsculas, de lo contrario False.
```python
txt = "hello world!"

x = txt.islower()

print(x)
```

#### Isupper
El isupper es un método que devuelve True si todos los caracteres están en mayúsculas, de lo contrario False.
```python
txt = "THIS IS NOW!"

x = txt.isupper()

print(x)
```
2.Procesar el <a href="https://drive.google.com/file/d/1lGmlAz157fIDp2zk95KInTSJguZusI91/view?usp=sharing">archivo</a> y extraer:
 - Cantidad de vocales
 ```python
 file = open ( 'Archivo.text') # Importo el archivo de texto
texto= (file.read()) # El archivo de texto lo deposito en una variable
texto=texto.lower() # Vuelvo todo el texto en minusculas
lista=["a","e","i","o","u"] # Lista de las vocales
vocales= 0 # Variable vocales que sera igual a 0
for j in range (0,len(lista)): # Recorro la lista desde el incio hasta el final
    vocales += (texto.count(lista[j])) # Las vocales = la cantidad de palabras que hay en el texto y que hay en la lista
print("La cantidad de consonantes en el texto son: " +str(vocales)) # Imprimimos
  ```
 - Cantidad de consonantes
 ```python
 file = open ( 'Archivo.text') # Importo el archivo de texto
texto= (file.read()) # El archivo de texto lo deposito en una variable
texto=texto.lower() # Vuelvo todo el texto en minusculas
lista=["b", "c", "d", "f", "g", "h", "j", "k", "l", "m", "n", "ñ", "p", "q", "r", "s", "t", "v", "x", "z", "w", "y"] # Lista de consonantes
consontante= 0 # Variable consonante que sera igual a 0 
for j in range (0,len(lista)): # For donde se recorre cada letra que hay en la lista
    consontante += (texto.count(lista[j])) # La consonante = la cantidad de palabras que hay en el texto y que hay en la lista
print("La cantidad de consonantes en el texto son: " +str(consontante)) # Imprimimos 
  ```
 - Listado de las 50 palabras que más se repiten
 - Listado de destinatarios con cantidad de mensajes recibidos
 - Cantidad de mensajes enviados por cada día
