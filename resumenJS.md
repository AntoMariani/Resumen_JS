# Resumen Javascript

## Variables
- `var` crea una variable global, puede re-asignarse y puede no asignarse un valor (a.k.a crearse vacía).
-  `let` crea una variable local, puede re-asignarse y puede no asignarse un valor (a.k.a crearse vacía).
-  `const` es una variable local, pero es constante, lo que significa que debe asignarse un valor si o si al ser creada y no puede ser reasignada bajo ninguna circunstancia en el resto del 
programa.


## Consola
Según [MDN web docs](https://developer.mozilla.org/es/docs/Tools/Web_Console "Consola Web") la consola web:
1. Muestra la informacion asociada con los Logs de la pagina Web: cualquier solicitud de red, JavaScript, CSS, y errores de seguridad y advertencias, asi como tambien, advertencias, mensajes informativos explicitamente generados por Javascript en tiempo de ejecucion dentro del contexto de la pagina.
2. te permite interactuar con la pagina ejecutando expresiones Javascript en el contexto de la página.

La manera de interactuar con ésta es a través del método `console.log()` por ejemplo

```
var miNombre = "Anto"
console.log(miNombre)
```

Una vez tenemos abierto nuestro html en el navegador podemos acceder a ella. En Chrome la manera rápida es apretando la tecla **F12**. La segunda solapa que encontraremos es _"Console"_.

En nuestro caso, debido al ejemplo anterior, veremos el valor **"Anto"** impreso en ella.

![Ejemplo console.log](./ejemplosCodigo/consolelogAnto.png)

## El Operador de Asignación "="
El signo igual `=` en Javascript se utiliza para asignar el valor de una variable a la variable en si.

```
var x = 5 + 4;
```
Asigna el valor que resulta de la suma de `5 + 4` a la variable `x`. Entonces si hacemos un print de pantalla

## Tipos de Datos
### Primitivos
- **Undefined**: Cuando se crea una variable pero no se le asigna un dato.
```
var variableUndefined
```
- **Null**: El "null" es directamente un tipo de dato en sí mismo.
```
var variableNula = null
```
- **String**: Una cadena de caracteres alfanuméricos. Se define entre comillas.
```
var variableCadena = "Hola, todo bien? Tengo 22 años."
```
- **Number**: Numeros enteros
```
var variableNumero = 16
```
- **Boolean**: El "null" es directamente un tipo de dato en sí mismo. Tiene solo dos valores: _verdadero_ y _falso_. Sirve para cuando se necesiten variables donde los valores deban ser _SI_ / _NO_ - _ON_ / _OFF_ - _TRUE_ / _FALSE_.
```
var variableBooleanaVerdadera = true
```
```
var variableBooleanaFalsa = false
```
- **Number**: Numeros enteros
```
var variableNumero = 16
```

### Tipo Objeto
El objeto es un tipo de variable que se inicializa con un nombre y una coleccion de propiedades, las cuales pueden ser modificadas, agregar nuevas y eliminar ya existentes.
Mas adelante en el resumen veremos como acceder a las propiedades y más información sobre los objetos. 

Existen dos maneras de crear un objeto en JS. 
```
var person = new Object();
persona.nombre = "John";
persona.apellido = "Doe";
persona.edad = 50;
persona.colorDeOjos = "azul";
```
```
var persona = {
    nombre:"John",
    apellido:"Doe",
    edad:50,
    colorDeOjos:"azul"};
```

También se puede crear vacío de la siguiente manera
```
var persona = {};
```
### ¿Cómo saber el tipo de dato de una variable?
Con el método `typeof` o `typeOf()` de la siguientes dos maneras
```
console.log(typeOf(variable))
```
```
console.log(typeOf variable)
```

Siguiendo con el ejemplo de la variable `miNombre`:
```
var miNombre = "Anto"
console.log(miNombre)
console.log(typeof(miNombre))
```
![Ejemplo typeOfVariableconsola](./ejemplosCodigo/typeOfVariableconsola.png)

También se puede consultar un tipo de dato de manera literal, por ejemplo:
```
console.log(typeOf (42))
```

![Ejemplo typeOfVariableconsola](./ejemplosCodigo/typeOf42consola.png)

### Cosas a tener en cuenta sobre tipos de datos
- JavaScript trata string vacios `("")`, al `0` , `undefined` y `null` como `false`. Todo el resto es `true`.
- 

