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
# Aqui es donde todo se desborono... Momentos mas dificiles de mi etapa como programador
Aqui en este instante es cuando todo se cayo a pedazos y mi cerebro no aguanto, me quede sin ideas no sabia como hacer los ultimos 3 subpuntos de taller y el tiempo no me ayudaba, tambien entiendo que deje todo para el final pero no tenia otra opcion que dejar esto como ultimo, puesto que lo demas eran los parciales finales y tenia que estudiar. A la falta de tiempo surgio la deseperacion y ante situaciones desesperadas soluciones desesperadas y tome una decision la cual fue pasarme al lado oscuro.

[![Captura-de-pantalla-2023-06-05-211700.png](https://i.postimg.cc/25yYmfR1/Captura-de-pantalla-2023-06-05-211700.png)](https://postimg.cc/w1CZcZBz)

Asi es tuve que copiar codigo de mis compañeros y utilizar chat.gpt para realizarlo se que esto no es la mejor opcion pero no tenia de otra soy muy lento programando en los primeros 2 puntos me gaste mis buenas horitas pensandolo bien, puesto que no soy muy fan de robar codigo ni de utilizar chat.gpt, pero la situacion lo amerito y no tuve otra opcion, sin embargo entendi los codigos aunque no los halla realizado por mi cuenta y por ultimo pero no menos importante se lo prometo que este reto lo realizare despues y mirare la forma de resolverlo por mis medios.

 - Listado de las 50 palabras que más se repiten
 ```python
file = open ( 'Archivo.text') # Importo el archivo de texto
texto= (file.read()) # El archivo de texto lo deposito en una variable
texto = texto.lower() # Dejo el archivo todo en minusculas
texto = texto.replace('.',' ').replace('?',' ').replace('!',' ').replace(',',' ') # Remplazo los caracteres

palabras = texto.split() # Divide el texto en palabras individuales

cont = {} # Crea un diccionario que se utilizara mas tarde

for x in palabras: # primer for que recorrera las palabras que hay en el texto

    # Si x osea la palabra ya se encuentra en el diccionario cont le suma 1 sino lse añade al diccionario
    if x in cont:
        cont[x] += 1
    else:
        cont[x] = 1

# Obtener las palbras mas comunes, ordenando el diccionario en funcion de los valores y se toman las 50 palabras
PLC = sorted(cont.items(), key=lambda j: j[1], reverse = True)[:50]

# Crea un bucle con rango PLC en j, p
for x, y in PLC:
    print(f"{x}: {y}")
 ```
 - Listado de destinatarios con cantidad de mensajes recibidos
 ``` python
 def contar_mensajes_diarios(texto: str):
    mensaje = []  # Lista para almacenar informacion con datos de fecha 
    palabras = texto.split()  # Separar las palabras del texto 

    for x in range(len(palabras)):
        if palabras[x] == "Received:":  
            segmento = []
            while palabras[x] != "-0500" and palabras[i] != "(GMT)": # Lista de palabras desde "Received" hasta "(GMT)" o "-0500".
                segmento.append(palabras[x])
                x += 1
            mensaje.append(segmento)

    mensaje_dia = {}  # Diccionario que contien el dia y el numero de mensajes enviados 

    for segmento in mensaje:
        indice = segmento.index('Jan')  # Índice de la palabra "Jan".
        dia = int(segmento[indice - 1])  # Extraer el día basado en el índice de "Jan".
        if dia in mensaje_dia:
            mensaje_dia[dia] += 1
        else:
            mensaje_dia[dia] = 1

    return mensaje_dia


with open ( 'Archivo.text') as file:
    mensaje_dia = contar_mensajes_diarios(file.read())
    for dia in mensaje_dia:
            print(f"Se enviaron {mensaje_dia[dia]} mensajes enviados el {dia} de enero, 2008")
 ```
 - Cantidad de mensajes enviados por cada día
 ``` python
 def destino(texto:str): # Definimos la funcion
    palabra  = texto.split() # Dividimos las palabras 
    destinatario = {} # Diccionario que contiene la dirreccion de email y los mensajes enviados a esta misma 
    for i in range(0, len(palabra)): # Primer for que recorrera todas las palabras
        if ([i] == "by" or palabra[i] == "BY") and "." in palabra[i-1]: # El string que esta en fente de BY o by contien un destinatario 
            if palabra[i+1] in destinatario: # Se bloquea el codigo para llenar el diccionario 
                destinatario[palabra[i+1]] += 1
            else:
                destinatario[palabra[i+1]] = 1  

    listado = list(destinatario.items()) # Lista de tuplas que contiene el destinatario y los mensajes dados a el 

    return listado

with open ( 'Archivo.text') as file:
    nombre = destino (file.read())
    for i in range(len(nombre)):
        lenstr = len(nombre[i])
        print(*nombre[i], sep=(3*" "),end="\n") #Imprime el destinatario y el nuemro de mensajes que se le han enviado separado por 3 espacios 
 ```
 # Fin
 Gracias por ver todo, y si leyo todo esto profesor disculpeme por hacer trampa se que eso no me ayuda a mi formacion pero no sabia que mas hacer sin embargo yo realizare este reto asi ya se acabe el semestre o no me afecte en la nota pero lo realizare de nuevo con mas calma y tiempo. 
