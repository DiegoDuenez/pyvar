# pyvar

Libreria de Python para checar el tipo de dato de una variable.

Esta libreria esta basada en funciones que pueden detectar el valor que reciben y retornar un valor booleano (true o false) dependiendo si el valor/variable dado cumple con la condición.

## Instalación 🛠

```
git clone https://github.com/DiegoDuenez/pyvar.git
```

## Importación 📦

Importa el archivo en tu codigo de Python.

<pre>import pyvar</pre>

## Empezando 🚀

A continuación se veran ejemplos del uso de esta libreria.

### Funciones

### ¿Cómo funcionan?
Todas las funciones (hasta ahora) trabajan en base a dos parametros.

El primer parametro es el **valor** y el segundo es el **mensaje** (opcional).

**valor** es la la variable o el valor que pasamos a la funcion para identificar su tipo de dato.

**mensaje** es un parametro booleano opcional, por defecto su valor es verdadero y no es necesario de especificarlo cuando intanciamos la función.

Forma innecesaria:

```

v = 5

pyvar.isInt(5, True) ❌

```

Lo que permite este parámetro es que cuando sea verdadero, aparecerá un mensaje en la consola como este:

```

v = "hello!"

pyvar.isInt(v)

```

```

* * * The values hello! is not an Int * * *

```

Para evitar que estos mensajes salgan, todo lo que tiene que hacer es poner ** mensaje ** como Falso y la función seguirá funcionando igual pero no aparecerá nada en la consola.

isInt()

- Esta función comprueba si el valor dado es un número entero.


```

v = 5

pyvar.isInt(v)

```

isFloat()

- Esta función comprueba si los valores dados son flotantes.

```

v = 5.1

pyvar.isFloat(v)

```


isString()

- Esta función comprueba si los valores dados son una cadena.

```

v = "hello!"

pyvar.isString(v)

```

isBool()

- Esta función comprueba si los valores dados son booleanos.

```

v = True

pyvar.isBool(v)

```

isNumericBool()

- Esta función comprueba si los valores dados son un booleano numérico (0 o 1)

```

v = 1

pyvar.isBool(v)

```

isList()

- Esta función comprueba si los valores dados son una lista.

```

v = ["diego", "dueñez"]

pyvar.isList(v)

```

isTuple()

- Esta función comprueba si los valores dados son una tupla.

```

v = ("diego", "dueñez")

pyvar.isTuple(v)

```

isDict()

- Esta función comprueba si los valores dados son un diccionario.

```

v = {"name":"diego", "lastname":"dueñez"}

pyvar.isDict(v)

```

isComplex()

- Esta función comprueba si los valores dados son complex.

```

v = complex(1,4)

pyvar.isComplex(v)

```

### Con condicionales (Ejemplo)

Puedes poner las funciones con condicionales como este:

```

v = 5

if pyvar.isInt(v):
  print("Yes, this value is an Integer")

```
Retorno (si la condicional es verdadera):

```

Yes, this value is an Integer

```

_si los valores son diferentes a Int_:

```

v = "hello!"

if pyvar.isInt(v):
  print("Yes, this value is an Integer")

```

Retorno:

```

* * * The values hello! is not an Int * * *

```


