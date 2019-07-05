# Programacion-BASIC
# PROGRAMACION BASICA PYTHON 

## ¿Que es python?
Python es un lenguaje de programación, creado por Guido Van Rossum a principios de los 90 cuyo nombre esta inspirado en el grupo de los cómicos ingleses "Monty Python". Es un lenguaje muy similar al C pero con un sintaxis muy limpia y que favorece un código legible. 



## Lenguaje Interpretado o de script 
Un lenguaje interpretado o de script es aquel que se ejecuta utilizando un programa intermediario que se llama **interprete** en lugar de compilar el código a lenguaje de maquina (lenguajes compilados).

### Interprete
Script: Print(Hola)

Interprete: 101101

Terminal: Hola

### Compilado 

Script:Print(Hola)

Interprete: 10110011

Ejecutable: Exe

Terminal: Hola

Programar una computadora es una habilidad que se aprende mejor mediante la experiencia de la practica por lo que es muy importante gastar en la pc poniendo en practica la teoría.

## Sentencia import 
La sentencia import se utiliza para importar un módulo. Usted puede usar cualquier archivo de código Python como un módulo ejecutando esta sentencia en otro archivo de código Python.

**import math**

**import turtle**


#Tipo de variable 
String: 'Oscar' Se usa para una cadena de texto

Intger: '33' Número 

### Concatenear 
Unir variables del tipo string en una sola para concatenear un número es una **,** (coma) una letra.

**'\n'** salto de linea

**'\+'** tabulación 

**()** para salir exit 

**'#'**Para agregar un comentario 

**Las variables no llevan espacio**

**cd** Abre archivos 

**dir** Directorio 

**Ejemplo**


*print('Whats your name')*


*nombre = input()*


*print('Hello',  nombre)*


Una variable de tipo flotante es una variable que puede guardar datos numéricos con punto decimal. Para forzar una variable que sea flotante sera 

**float ()** Número decimal 

**int ()** Número entero

w=float(input('Ingrese su peso:'))
g=float(input('Ingrese su altura:'))


p=w*75


q=g*112

peso=p+q

print('El peso total de su pedido es:',peso, 'gramos')

 
## Tipos de datos
Números: **3 (entero o integer)**,  **1.75 (Punto flotante o float)**, 

Para poder conocer el tipo de dato de una variable usaremos la instrucción **type ()**

Otro tipo de dato básico es python son las cadenas de texto, ejemplo:

"Hola mundo" (Cadena de texto)

Como se puede notar a diferencia de otros lenguajes en python no se declara el tipo de variable al crearla. Para resumir en python se puede representar en números enteros, números reales, números complejos.

### Operador aritmético
**+**	Suma,  r=3+2

**-**	Resta, r=7-3


**-** Negación, r=-5

**x**Multiplicación, r=5x2

** Exponente, r=2*9

**/** División, r=6.5/2

**//** División entera, r=3.5//2 

**%** Módulo, r=7%2

Igual que == 

Distinto de != 

Menor que < 

Menor o igual que <= 

Mayor que > 

Mayor o Igual que >=  

**Ejemplo**

*largo= float(input('Inserta el largo de tu habitacion:'))*

*ancho= float(input('Inserta el ancho de tu habitacion:'))*

area= largo*ancho

*print('El Area de tu habitacion es:', area , 'm2')*

#Condicional if y else
Algunas veces en nuestros programas es necesario que tomemos algunas “decisiones”, esto en el sentido de que necesitamos decidir si ejecutar una pieza en especial de codigo o no, o tal vez dadas ciertas condiciones tendríamos varias alternativas de código que ejecutar.

Para esto tenemos una sentencia llamada **if** y otra llamada **else**.

La sentencia If evalúa básicamente una operación lógica, es decir una expresión que de como resultado verdadero o false (true o false), y ejecuta la pieza de código siguiente siempre y cuando el resultado sea verdadero.

1
#!/usr/bin/python
2
 
3
a = 7
4
 
5
if ( a  > 5) : print "La variable es mayor a 5!"
6
 
7
print "fin"


La orden else, que indica a Python que el bloque que viene a continuación se tiene que ejecutar cuando la condición no se cumpla (es decir, cuando sea falsa). Esta línea también debe terminar siempre por dos puntos (:). La línea con la orden else no debe incluir nada más que el else y los dos puntos.


 
03
a = 10
04
 
05
if ( a  !=  10) :

06
       print "La variable es diferente de 10!"

07
else:
08
      print "La variable es igual a 10!"
09
 
10
print "fin"


## Elif
"elif" sirve para enlazar varios "else if", sin tener que aumentar las tabulaciones en cada nueva comparación. 

x = int(input("Dame un numero: "))

if x < 0:

    x = 0
    print('Negativo... convertido en cero')
elif x == 0:

    print('Cero')
elif x == 1:

    print('Uno')
else:

    print('Otro')

## Bucle while 
Un bucle while permite repetir la ejecución de un grupo de instrucciones mientras se cumpla una condición (es decir, mientras la condición tenga el valor True).

numero = int(input("Escriba un número positivo: "))

while numero < 0:

    print("¡Ha escrito un número negativo! Inténtelo de nuevo")

    numero = int(input("Escriba un número positivo: "))

print("Gracias por su colaboración")


## Bucle for 
En ocasiones, tenemos que repetir varias veces una determinada tarea hasta conseguir nuestro objetivo. En Python esto se realiza con el comando for

 
 coches = (‘Ferrari’, ‘Tesla’, ‘BMW’, ‘Audi’)

 for coche in coches:

     print(coche)

Ferrari
Tesla
BMW
Audi
1
2
3
4
5
6
7
8
 coches = (‘Ferrari’, ‘Tesla’, ‘BMW’, ‘Audi’)

 for coche in coches:

    print(coche)
 
Ferrari
Tesla
BMW
Audi

#Módulo turtle
La "tortuga" es un cursor al que se le pueden dar órdenes de movimiento (avance, retroceso o giro) y que puede ir dejando un rastro sobre la pantalla. Moviendo adecuadamente la tortuga se pueden conseguir dibujar todo tipo de figuras.

**Código orientado a objetos**: import turtle 

La ventana de dibujo: setup() y title()
El módulo turtle dibuja en una ventana distinta a la ventana de IDLE. Esta ventana de dibujo se crea al ejecutar un programa y se mantiene al acabar la ejecución del programa, pero se destruye al volver a ejecutar el programa).

La función setup(ancho, alto, posicionX, posicionY) permite definir el tamaño y la posición inicial de la ventana. Los cuatro argumentos de la función son (en píxeles):

ancho: ancho de la ventana.
alto: alto de la ventana.
posicionX: posición horizontal de la ventana. Los valores positivos se miden desde el borde izquierdo de la pantalla, los negativos desde el borde derecho de la pantalla.
posicionY: posición vertical de la ventana. Los valores positivos se miden desde el borde superior de la pantalla, los negativos desde el borde inferior de la pantalla.

![Ejemplo](/imagenes/Captura.png)

**showturtle()**: Esta función muestra el cursor de la tortuga 

**goto()**: Muestra la posicion final del dibujo 

**pendown()**: Esto es igual a bajar y levantar el lápiz del papel

**pensize()**: Modifica lo grueso del trazo

**pencolor()**: Modifica el color de la linea dibujada 






## Modulo
Un módulo le permite a usted organizar lógicamente su código Python. Agrupando código relacionado dentro de un módulo hace el código mas fácil de entender y usar. Un módulo es un objeto de Python con atributos con nombres arbitrarios que puede enlazar y hacer referencia.

Simplemente, un módulo es no es otra cosa sino un archivo con extensión .py. Un módulo puede definir funciones, clases y variables, también puede incluir código ejecutable. 

class Coche(object): 
    def __init__(self, gasolina):
        self.gasolina= gasolina

    def arrancar(self):
        if self.gasolina > 0: 
            print('Arranca')
        else:
            print('No arranca')

    def conducir(self):
        if self.gasolina > 0:
            self.gasolina = self.gasolina - 1
            print('Quedan', self.gasolina, 'litros')
        else:
            print('No se mueven')

vocho = Coche(5)
tsuru = Coche(3)

vocho.arrancar()
vocho.conducir()
vocho.conducir()
vocho.conducir()
vocho.conducir()
vocho.conducir()
vocho.conducir()

### Def

Definir funciones a esto se le agrega un nombre descriptivo seguido de paréntesis de apertura y cierre. Como toda estructura de control en Python, la definición de la función finaliza con dos puntos (:) y el algoritmo que la compone, irá identado con 4 espacios. 
