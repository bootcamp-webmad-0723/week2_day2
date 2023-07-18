# `data-` attributes in DOM
Los atributos `data-` son atributos de HTML que permiten incluir informaciones variadas que no se ajustan a ninguno de los atributos estándar disponibles en etiquetas:
````html
<div id="first" data-color="red">...</div>
<div id="second" data-age="81">...</div>
````
Su estructura se basa en un prefijo `data-` seguido de un sufijo a elección, cuyo valor es accedido a través de Javascript mediante la propiedad `.dataset` y el sufijo elegido:

````javascript
const colorValue = document.querySelector('#first').dataset.color   // red
const ageValue = document.querySelector('#second').dataset.age    // 81
````
