# Portafolio de Fundamentos de Programación
En este portafolio observaremos todo nuestro conocimiento y aprendizaje acerca de lo adquirido en el transcurso del primer semestre en la materia de programación.

## ¿Qué es Python?
Es un lenguaje de programación de tipo interpretado por su forma de ejecución, muchos en su extensión lo definen como un “lenguaje de programación versátil” debido a su interpretación legible para cualquier persona con conocimientos básicos de programación en donde se destaca su código legible y limpio.

[![python.png](https://i.postimg.cc/brbzxtLd/python.png)](https://postimg.cc/YLrKkj5w)

## ¿Qué es una variable?
Es un espacio en la memoria en donde se guardan los datos que utiliza un programa, en el cual cada una de las variables empleadas debe tener un nombre propio, con el cual se la podrá identificar, durante el desarrollo del mismo.
Como, por ejemplo:
```python
vacunas = 29
pelotas = 20
niños = 15
chicas = 21
```
### Nombrando una variable
Cuando estamos nombrando una variable a su vez la estamos creando es decir estamos solicitando a python aquel espacio de memoria que nos servirá para el desarrollo del programa en el futuro.

Sin embargo antes de empezar con este proceso debemos tener en cuenta ciertos aspectos:
1.	Nunca debemos iniciar la variable con un número o esta última será rechazada. 
```python
1chica = 2
```
2.	No podemos usar palabras reservadas del lenguaje (en nuestro caso Python).
```python
sum
range
application
```
3.	Para nombrar variables con más de una palabra debemos usar “_” .
```python
vacunas_aplicadas_en_marzo = 30
```
4. Una vez comprendidas todas estas reglas podemos empezar a nombrar las variables que necesitásemos para nuestro programa de manera correcta.
```python
niños_inscritos_en_el_sistema = 20
niñas_inscritos_en_el_sistema = 10
profesores = 15
adolescentes = 500
```  
### Asignando valores a una variable
Al colocar valores en las variables de Python lo que estamos haciendo realmente es introducir algún tipo de dato en aquel espacio de memoria que se creó con el nombre que nosotros mismos le hayamos asignado.
Como se muestra a continuación:
```python
nombre = 'Danny'
edad = 18
curso = 'Sistemas1 Matutino'
```
### Operadores básicos

#### Suma
Aquel operador que como su nombre lo indica suma números enteros, reales o una combinación de ambos. Se opera mediante el signo más  
“ + ”.

Como veremos en el siguiente ejemplo podremos realizar una suma común y corriente creando una variable llamada suma
```python
suma = 2 + 5
print(suma)
[output] 7
```
e imprimirlo por consola. 
```python
print(suma)
[output] 7
```
A su vez podemos solicitar valores al usuario:
```python
numero1 = int(input("Ingrese un numero"))
numero2 = int(input("Ingrese un numero"))
numero3 = int(input("Ingrese un numero"))
suma = numero1 + numero2 + numero3
print('Los valores ingresados suman un total de' ,suma)
```
Así como también podremos sumar variables con valores asignados en programas un poco más grandes u complejos:
```python
carros_azules = 23
carros_rojos = 12
carros_negros = 15
suma = carros_azules + carros_negros + carros_negros
print("Existen",suma, "carros en la concesionaria")
```
En donde se produce una entrada o ingreso de datos:
```python
carros_azules = 23
carros_rojos = 12
carros_negros = 15
```
Otro donde ocurre el procesamiento del programa
```python
suma = carros_azules + carros_negros + carros_negros
```
Y finalmente donde acurre la salida o la solución del programa, el cual nos imprimirá la consola.
```python
print("Existen",suma, "carros en la concecionaria")
[output] Existen 53 carros en la concesionaria
```
Procesos de entrada, procesamiento y salida de datos los cuales sucederán de la misma manera con los demás operadores en programas simples u complejos dependiendo del caso.

#### Resta
Aquel operador que se encarga de sustraer números enteros, reales o una combinación de ambos. Se opera mediante el signo menos “ - ”.

A continuación, observamos una simple resta creada mediante una variable:
```python
resta = 4500 - 2465
print(resta)
[output] 2035
```
También podríamos haberla ejecutado mediante el print sin necesidad de crear una variable: 
```python
print("La resta es" , 4500 - 2465)
[output] La resta es 2035
```
En donde el programa leerá la orden y la ejecutará
```python
print("La resta es" , 4500 - 2465)
```
Y la imprimirá por consola
```python
[output] La resta es 2035
```
#### Multiplicación
Aquel operador encargado de multiplicar lo propiamente dicho: números enteros, reales o una combinación de ambos. Se opera mediante un asterisco " * ".

Al igual que como sucede con los otros operadores tenemos nuestra respectiva operación:
```python
multiplicacion  = 10 * 10
print(multiplicacion)
[output] 100
```
En donde se seguirá el mismo patrón de programa para ejecutar de las otras operaciones con la diferencia del signo que deberá ser cambiado, además de realizar lo mismo con las variables en caso de ser solicitadas:
```python
numero1 = int(input("Ingrese un numero"))
numero2 = int(input("Ingrese un numero"))
numero3 = int(input("Ingrese un numero"))
multiplicacion = numero1 * numero2 * numero3
print('Los valores ingresados multiplicados hacen un total' , multiplicacion)
``` 
Y el programa procederá a aplicar los mismos métodos de solución de los anteriores operadores con la diferencia de que ahora los multiplicará:
```python
multiplicacion = numero1 * numero2 * numero3
``` 
#### División
Operador encargado de realizar la división de números reales, enteros u la combinación de ambos. Se opera mediante “ / ".

A continuación, tenemos un pequeño programa básico que nos realizara división normal de cualquier numero que ingresemos en pantalla:
```python
division = int(6/3)
print("La division es", division)
[output] 2
```
Colocaremos alado del igual el tipo de dato en el que queremos que nos arroje el resultado ya sea entero(int) o decimal(float)
```python
division = int(6/3)
```
Pero tenemos que tener en cuenta que la división posee ciertas restricciones aritméticas ya que la división a cero no está definida y el cero/cero es indeterminado.

Por lo cual al procesar estos valores en cero nos arrojarían errores en la consola.

Para la cual si se desea hacer un programa completo en el que se le indique al usuario que sucede con los valores divididos a cero tendríamos que crear uno similar al ejemplo de a continuación:
```python
a = int(input("Ingrese el dividendo"))
b = int(input("Ingrese un divisor"))
if a > 0 and b == 0:
    print("No definido")
elif a == 0 and b==0:
    print("Inderteminado") 
else:
    print(a/b) 
```
Como podemos verificar en este programa tenemos las 2 restricciones matemáticas de la división en donde:
1. Ningun numero puede ser dividido a cero: 
```python
if a > 0 and b == 0:
    print("No definido")
```
2. La división cero a cero es indeterminada:
```python
elif a == 0 and b== 0:
    print("Inderteminado")
```
3. Y por último afuera de estas restricciones tenemos la realización de una división normal la cual se ejecutará si no se cumplen ninguna de las 2 restricciones anteriores:
```python
else:
    print(a/b) 
```
#### Módulo


## Tipos de datos en Python

### Integer
Son aquellos datos que únicamente representan números enteros es decir netamente números positivos y negativos incluyendo el cero.
```python
dato1 = 15
dato2 = 0
dato3 = -425
```

### Float
Son aquellos datos que únicamente representan valores de números reales con partes decimales.
Nota: Al escribir un dato de este tipo no se utiliza la coma sino el punto.
```python
dato4 = 2.5
dato5 = 3.14 
```

### String
Son aquellos datos que representan cadenas de caracteres que permiten procesar letras, números y símbolos, los cuales se escriben obligatoriamente en comillas dobles u simples siempre y cuando tanto el inicio como el final tengan estas mismas. 
```python
nombre = "Danny"
```
o también  
```python
nombre = 'Danny'
```
Nota: Si queremos representar un número como un carácter debemos encerrarlo en comillas dobles o simples de lo contrario el programa asumirá que es un dato de tipo entero.
```python
dato6 = '890'
```
### Casting en Python
Cuando hablamos de casting en Python nos referimos a convertir un tipo de dato a otro.

Por ejemplo:

Tenemos a las variables "X" y "Y" con datos de tipo flotante(float) y carácter(str)
```python
x = 8.5
y = "10"
```
Si queremos llevar estas variables a un tipo entero(int) por así decirlo, pues tenemos que reescribirlas y escribir el tipo de dato al que queremos transformarlas a lado de estas últimas.
Como se muestra a continuación:
```python
x = int(8.5)
y = int("10")
```
Por último, la consola arrojara los datos convertidos al usuario según como los haya pedido.
### List
Las listas son estructuras de datos que nos permiten almacenar distintos valores y elementos, al ser estructuras dinámicas están sujetas a mutaciones. Cabe destacar que a las listas se las definen entre corchetes “[]”.

Como veremos en el siguiente ejemplo:
```python
lista1 = ["Maria", "Lucia", "Antonio", "Jose" ]
print(lista1)
```
### Tuple
Una tupla es un conjunto ordenado e inmutable de elementos del mismo o diferente tipo, es similar a una lista en términos de indexación, objetos anidados y repetición. Las cuales se representan escribiendo los elementos entre paréntesis y separados por comas.
```python
(1,2,4,5,6,7,8,9)
("Hola", "soy", "Danny")
```
### Dictionary
Un Diccionario es una estructura y un tipo de datos con características especiales que nos permite almacenar cualquier tipo de valor como enteros, cadenas, listas e incluso otras funciones. Estos diccionarios nos permiten además identificar cada elemento por una clave (Key).
```python
#Primeramente tenemos que definir hacia donde ira orientado nuestro diccionario 
#Una vez hecho esto colocamos nuestra ideas sobre el mismo en donde el listado de valores se encierran entre llaves y las parejas de clave y valor se separan con comas,por lo cual la clave y el valor se separan con dos puntos.
diccionario = {"azul":"blue", "amarillo":"yelow", "rojo":"red"}
#Colocamos el elemento del diccionario al que deseamos acceder mediante la clave de este ultimo. 
print(diccionario["amarillo"])
#Como punto final tenemos que este elemento se terminara imprimiendo dependiendo de la orden que el usuario le proporcione.
```
## Tomando decisiones
Cuando hablamos de la toma de decisiones en programación nos referimos a los caminos que tendrá que seguir el propio programa para llegar al objetivo final impuesto por el programador quien lo comanda, esto ultimo lo conseguirá mediante ciclos y sentencias como veremos a continuación:
### Sentencia if
Aquella sentencia se usa para tomar decisiones, esta evaluá básicamente una operación lógica, es decir una expresión que da como resultado True o False, y ejecutara la pieza de código siguiente siempre y cuando el resultado sea verdadero.

Como se muestra a continuación en el siguiente ejemplo:
```python
#Primeramente le pediremos al usuario que ingrese un valor.
num = int(input("ingrese numero:"))
#Luego gracias a las sentencias if/else el programa determinara si aquel numero ingreasdo es par o impar. 
if (num%2==0):
    print("El numero es par",)
    print(num,"es par")
else:
    print("El numero es impar") 
#Y por ultimo lo imprimira en consola.
```
### Ciclo For
El bucle for se utiliza para recorrer los elementos de un objeto iterable y ejecutar un bloque de código. En cada paso de la iteración se tiene en cuenta a un único elemento del objeto iterable, sobre el cuál se pueden aplicar una serie de operaciones.

Como se demuestra en el siguiente ejemplo:

```python
#Ejercicio en el cual nos piden calcular la suma y la media aritmetica de N numeros reales ademas de solicitar el valor de n al usuario en cada uno de los N números reales.
n = int(input("Ingrese los números que desee: "))
suma= 0
for i in range(n):
    nota =int(input('Ingrese el número' + str (i+1) +  ':'))
    suma += nota
    
promedio = suma/n 
print("promedio:", promedio)
```
### Ciclo While
La sentencia o bucle while en Python es una sentencia de control de flujo que se utiliza para ejecutar un bloque de instrucciones de forma continuada mientras se cumpla una condición determinada.
```python
#En este ejemplo dependiendo del numero que el usuario ingrese este ultimo sera ejecutado o a su vez podra ser descontinuado o rechazado
num=11

while num<10 or num >20 or num%2!=0:
    num=int(input("ingrese numero:"))

print("se fue")
```
### Break
La sentencia break nos permite alterar el comportamiento de los bucles while y for. Concretamente, permite terminar con la ejecución del bucle, esto significa que una vez se encuentra la palabra break, el bucle se habrá terminado.

Como se muestra a continuación:

En donde el ciclo for se ve interrumpido gracias al break.
```python
j=0
for i in range (10):
    j+=2
    print ("i;",i,"j:",j)
    if j==10:
        break
```
### Continue
El uso de continue al igual que el break, nos permite modificar el comportamiento de  los bucles while y for. Concretamente, continue se salta todo el código restante en la iteración actual y vuelve al principio en el caso de que aún queden iteraciones por completar.
La diferencia entre el break y continue es que el continue no rompe el bucle, si no que pasa a la siguiente iteración saltando el código pendiente.

Como observaremos en el siguiente ejemplo:

