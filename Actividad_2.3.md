# Tarea 1: La tabla de predicciones

Completa la tabla justificando cada respuesta con base en la teoría de la unidad.

| Identificador | ¿Qué imprimirá la consola? | Justificación teórica |
| --- | --- | --- |
| Log A | `undefined` | La declaración con `var` se eleva mediante *hoisting*. La variable existe antes de su línea de declaración, pero todavía no tiene asignado un valor, por lo que su valor inicial es `undefined`. |
| Log B | `Teclado Mecánico` | La declaración se eleva mediante *hoisting* y, cuando se ejecuta el registro en consola, la variable ya tiene asignado el valor `Teclado Mecánico`. |
| Log C | `25` | El valor corresponde a la variable accesible en ese ámbito. Las variables declaradas dentro de un bloque pueden tener un ámbito de bloque y ser distintas de variables con el mismo nombre declaradas fuera de él. |
| Log D | `10` | Se imprime el valor de la variable accesible desde el ámbito en el que se ejecuta la instrucción. El ámbito de bloque puede hacer que una declaración interna no sustituya a otra externa. |
| Log E | ¡Error! | La variable no está disponible en el ámbito desde el que se intenta acceder; por ello, se produce un error de referencia. |
| Log F | ¡Error! | Se accede a una variable declarada con `let` o `const` antes de su inicialización. La variable está en la Zona Muerta Temporal (*Temporal Dead Zone*, TDZ), por lo que se produce un error de referencia. |

# Tarea 3

El uso de `var` permite acceder a una variable antes de su línea de declaración debido al *hoisting*. En ese momento, su valor es `undefined`, lo que puede provocar errores difíciles de detectar. En aplicaciones extensas, la falta de control del ámbito de las variables puede afectar a la estabilidad y la mantenibilidad del proyecto.



