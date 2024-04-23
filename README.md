# Arrays

- Un array es una zona de alamcenamiento continuo, donde se pueden introducir varios valores cada uno de ellos ubicado por la posicion que ocupa en el array tambien son denominados arreglos o vectores, y cuando son de dos dimensiones son llamados matrices

- Los arrays son brindan la capacidad de almacenar una coleccion de elementos y acceder a ellos de manera individual.
- Cda elemento se identifica midnate su posicion el el array denominada **indice**, y estos indices son siempre secuenciales.
- En Javascript son altamente flexibles en terminos de  los diferentes tipos de datos que podemos almacenar en cada posicion del array.

## Crear un array

1. Declarando un array con elementos en linea.

```Javascript
let miArray = [1, 2, 3];
console.log(miArray);
```   

2. Declarando un array con la sintaxis **new Array()**

```Javascript
let miArray = new Array(1, 2, 3);
console.log(miArray);
```   

3. Declarando un array con un tamaño especifico utilizando la sintaxis **new Array** y asignando valores despues:

```Javascript
let miArray = new Array(3);
miArray[0] = 1;
miArray[1] = 2;
miArray[2] = 3;
console.log(miArray);
``` 

4. Declarando un array con elementos de diferentes tipos de datos 

```Javascript
let miArray4 = [1, "dos", true, {nombre:    "Juan", edad: 30}];
console.log(miArray);
```