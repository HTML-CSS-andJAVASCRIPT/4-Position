# 4 Position
La propiedad position nos permite posiccionar los elementos. Hay algunos conceptos que debeís conocer.
 - Flujo de renderizado -> Por norma general los elemntso se dibujan de izquierda a derecha y de arriba abajo. En el punto 0.0 de los elementos, por norma genera, es la esquina superior izquierda.

 - Espacio reservado -> Es el espacio que tiene un elemento asignado en el navegador.

 - Elemento posicionado -> Esto significa que el elemento tiene la propiedad `position ='static'`, que es el valor por defecto
 -Stackin context -> Contexto de apilamiento. Es el orden en el que se apilarán las cajas que se superponen. En el mismo contenedor

Al posicionar un elemento se habilitan 5 propiedades que podemos utilizar para mover en los 3 ejes.
 - top -> El elemento se moverá desde la parte superior la distancia que le hayamos indicado.
 - right -> El elemento se moverá desde la parte derecha la distancia que le hayamos indicado.
 - bottom -> El elemento se moverá desde la parte inferior la distancia que le hayamos indicado
 - left -> El elemento se moverá desde la parte izqioerda la distancia que le hayamos indicado
 - z-index -> Nos permite mover el elemento en el contexto de apilamiento (eje Z)

Nota: Si a un elemento le declaramos la propiedad top y/o left, las propiedades bottom y/o right no funcionarán

Los posibles valores que le podemos dar a position son:
 - Static-Z Es el valor por defecto.
 - Relative -> El elemnto mantendrá su posición y medidas en el flujo de renderizado y mantendrá su espacio reservado. Si lo movemos lo hará usando su posición en el html como punto de referencia.
 - Absolute -> El elemento perdeŕa sus medidas y su espacio reservado. Si lo movemos usará el elemento padre posicionado como referencia. Si no tiene ninguno, usará el elemento html de referencia.
 - Fixed -> El elemento perdeŕa sus medidas y su espacio reservado. Si lo movemos usará el elemento html de refernecia, y además se quedará fijo en esa posicion aunque hagamos scroll.
 - Sticky ->  Es una mezcla de position relative y fixed. Con este tipo de posicionamiento los valores top, left, bottom y right no sirven para mover el elemento, sino para indicarle enq ue punto pasaŕa a tener un comportamiento de posicionamiento fixed, hasta llegar a ese punto se comportará como si estuviera relative.

