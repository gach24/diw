# GRID LAYOUT

## Que es

Sistema de rejillas en dos dimensiones (a diferencia de flexbox que solo actua sobre una dimensión, la horizontal o la vertical, pero solo una)

## Que tiene de diferente

1. Voy a poder colocar los items donde quiera... pero habrá items que se coloquen solos (AUTO-PLACEMENT)
2. Puedo hacer lo mismo de muchas formas... pero no todas hacen lo mismo
3. Controlo las dos dimensiones, no es flexbox
4. La colocación de los items es muy libre, no es una tabla
5. Tiene una extensa sintaxis
6. Nos va a volver un poco locos, pero es muy potente

## Conceptos básicos

![Grid Line](./doc/img/grid-concepts.svg)

1. Las lineas (marcadas en rojo)
2. Los tracks. Espacios entre líneas (marcadas en colores rosa y azul)7
3. Las celdas (marcadas en verde)
4. Las áreas (marcadas en amarillo)

## display grid

En cuanto declaro **display: grid** o **display: inline-grid** los hijos directos de ese elemento pasan a ser grid items

## Definiendo tracks en el grid

Debemos crear el grid explicitamente, es decir, al contenedor grid le indico como deben ser las filas y las columnas (existen múltiples sintaxis y formas de hacerlo)

## Posicionamiento de los grid-items

La enorme potencia de **Grid Layout** en parte viene dada porque una vez generada la regilla, puedo colocar los items donde quiera dentro de esta (Defino un grid donde luego puedo colocar items)

## Líneas nombradas

Dentro del posicionamiento de los grid-items podemos utilizar líneas nombradas, esto es una gran ventaja por:

1. Me ayudan a recordar como van los tracks en layouts complejos
2. En responsive me evitan sobreescribir la colocación de algunos items
3. Si cambia el número de tracks **no tengo que reposicionar elementos**

## Algoritmo de autoplacement

- Reglas que controlan dónde se colocan los items cuando no establecemos su posición o por otro, pierde su sitio natural
- Aunque no les dé información de donde colocarse, ellos buscarán sitio en celdas libres o crearán los tracks necesarios para hacerlo
- Lo primero que determina como funciona autoplacement es el valor de la propiedad **grid-auto-flow**

### Propiedad grid-auto-flow

Determina dos aspectos:  

- Dirección: Define la dirección en la que el grid va a crecer si necesita colocar items por auto-placement
  - Row (por defecto)
  - Column
- Modo: Determina si el algoritmo intentará rellenar huecos vacíos para colocar items por auto-placement
  - sparse (por defecto)
  - dense

## Indice de ejemplos

1. [Conceptos básicos](./0901-EJ/)
2. [Definiendo grid explícitamente](./0902-EJ/)
3. [Utilizando la unidad de medida FR (Fraction Unit)](./0903-EJ/)
4. [Definiendo el tamaño de las celdas implicitas con **grid-auto-row**](./0904-EJ/)  
5. [Repitiendo filas y columnas mediante la función **repeat**](./0905-EJ/)
6. [Definiendo el tamaño mínimo y máximo de las celdas mediente **minmax**](./0906-EJ/)
7. [Ajuste automático mediante autofill y autofit](./0907-EJ/)
8. [Diferencias entre autofill y autofit](./0908-EJ/)
9. [Ejemplo de error y solución a un desbordamiento con la propiedad **grid-auto-row**](./0909-EJ/)
10. [Posicionamiento de items](./0910-EJ/)
11. [Ejercicio con psudoelementos](./0911-EJ/)
12. [Ejercicio de repaso](./0912-EJ/)
13. [Líneas nombradas](./0913-EJ/)
14. [Líneas nombradas con nombres múltiples](./0914-EJ/)
15. [Líneas nombradas con nombres repetidos](./0915-EJ/)
16. [Áreas nombradas](./0916-EJ/)
17. [Ejemplo holy grail layout desde mobile first](./0917-EJ)
18. [Magic Lines](./0918-EJ/)
19. [Líneas nombradas con nombres de área](./0919-EJ/)
20. [Alineación de los items](./0920-EJ/)
21. [Alineación de los tracks](./0921-EJ/)
22. [Ejemplo de crecimiento automático en columnas **grid-auto-flow: column**](./0922-EJ/)
23. [Funcionamiento del algoritmo de autoplacement](./0923-EJ/)
24. [Más ejemplos del funcionamiento del algoritmo de autoplacement](./0924-EJ/)
25. [Normas que sigue el algoritmo de autoplacement](./0925-EJ/)
26. [Más ejemplos del algoritmo de autoplacement](./0926-EJ/)
27. [Ejercicio repaso](./0927-EJ/)
28. [Ejercicio repaso](./0928-EJ/)
