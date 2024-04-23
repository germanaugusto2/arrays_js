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

## Accediendo a la informacion de un array

### Propiedad length
- Devuelve la cantidad de elementos del array 

### Operador [pos]
- Permite acceder para leer o modificar el elemento pos del array 

### Metodo at(pos)
- Devuelve el elemento de la posicion pos. El parametro admite valores negativos lo que significa que empiezan a contar por el final del array.

```Javascript
const letters = ["A", "B", "C"];
console.log(letters.length);
console.log(letters[2]);
console.log(letters[5]);
```

## Añadir o eleminar elementos
- push(elel, ele2): añade uno o varios elementos al final del array. Devuelve el tamaño del array.

```Javascript
let miArray = [1, 2, 3];
miArray.push(4); // Agrega el elemento 4 al final del array
console.log(miArray);
```

- pop(): Devuelve el ultimo elemento del array y lo emimina 
```Javascript
let miArray = [1, 2, 3];
miArray.pop(); // Elimina el ultimo elemento del array
console.log(miArray);
```

- unshift(ele1, ele2): añade uno o varios elementos al inicio, devolviendo el tamaño del array despues de añadidos
array y lo emimina 
```Javascript
let miArray = [1, 2, 3];
miArray.unshift(0); // Agrega el elemento 0 al inicio del array
console.log(miArray);
```
- shift(): Devuelve el primer elemento del array by lo elimina 
```Javascript
let miArray = [1, 2, 3];
miArray.shift(); // Elimina el primer elemento del array 
console.log(miArray);
```

- concat(elel1, ele2): concatena dos arrays
```Javascript
let miArray = [1, 2, 3];
let miArray = [4, 5];
let nuevoArray = miArray.concat(miOtroArray);
console.log(miArray);
console.log(miOtroArray);
console.log(minuevoArray);
```

- split(separador): a partir de una cadena 
```Javascript
let miString ="Hola como estas?";
let miArray = miString.split.split(" "); 
console.log(miArray);
```

- join(separador): a partir de un array, crea una cadena separando cada elemento con el separador. 
```Javascript
let miArray = ["Hola,", "¿como", "estas?"];
let miString = miArray.split.join(" "); 
console.log(miString);
```

## Busqueda de elementos en un array

- includes(elemento): Devuelve true o false si el elemento existe o no dentro del array
- indexOf(elemento): devuelve la posicion de la primera aparicion del elemento. Si no existe, devuelve -1.
- lastIndexOf(elemento): devuelve la posicion de la ultima aparicion del elemento. S no existe, devuelve -1.

## Modificar el array o crear fragmentos
- slice(inicio, fin); devuelve un array con los elementos desde la posicion inicio hasta la posicion fin, ambos excluidos.

## Ordenar elementos de un array
- reverse(): invierte el orden del elementon del array
- sort(): ordena el array alfabeticamente
- sort(crriterio): ordena el array con el criterio determinado por funcion criterio.

## Boorar elementos de un array 
- Se pueden borrar el contendo de un elemento de un arrar poniendo su valor null o asignando una cadena vacia " ".
- Pra eliminar completamente un elemento del array se utiliza el operador delete.

## Recorrido de un array 
1. Recorrer con un bluce clasico pasando por todos los elementos
```Javascript
var dias = ["lunes", "martes", "miercoles", "jueves", "viernes", "sabado", "domingo"];
for(i=0;<dias.lengt;i++)
{
    console.log(dias[i]);
}
```
2. Recorrer con un while, pasando por todos los elementos.
```Javascript
var dias = ["lunes", "martes", "miercoles", "jueves", "viernes", "sabado", "domingo"];
var i = 0
for(i=0;<dias.lengt;i++)
{
    console.log(dias[i]);
    i++;
}
```
3. usando la sentencia for..in.
```Javascript
var dias = ["lunes", "martes", "miercoles", "jueves", "viernes", "sabado", "domingo"];
for(let index in dias)
{
    console.log(dias[index]);
}
```

## Array multidimensionales
```Javascript
const matrix = [
    [1,2,3],
    [4,5,6],
    [7,8,9]
]:
```
- Recorrer una matriz utilizando bucles anidados.
```Javascript
var dias = ["lunes", "martes", "miercoles", "jueves", "viernes", "sabado", "domingo"];
for(i=0;<matriz.lengt;i++)
{
    for(let j=0;matriz[i].length; j++)
    {
         console.log(dias[i]);
    }
    
}
```
# Ejercicios

1. Dada una lista de numeros separados por coma, calcular la suma,el mayor,el menor y la media de todos.

2. Introducir dos cadenas con elementos separados por coma, y con un boton concatenar las dos cadenas y mostrarlas en pntalla.

3. Introducir uno a uno los elementos en un array a través de un boton. Con otro botón se va eliminado el último elemento. Siempre que se pulse alguno de los botones de debe mostrar el contenido del array.

4. Introducir un conjunto de números separados por comas. Cuando se pulsa el botón "Pares" cargar una tabla con los números introducidos y luego crear otra que solo incluya los números pares y mostrarla.