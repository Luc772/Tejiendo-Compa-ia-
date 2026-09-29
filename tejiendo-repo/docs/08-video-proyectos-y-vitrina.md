# 8. Video de fondo, selección de proyecto y vitrina comunitaria

Esta actualización agrega tres mejoras grandes al prototipo, pensadas para hacerlo más atractivo y más completo funcionalmente.

## Video de fondo persistente
El video institucional ya no aparece solo en la portada: ahora vive detrás de toda la aplicación, visible (atenuado con un panel translúcido y desenfoque) mientras se navega por cualquier pantalla. Esto le da una identidad visual continua a la experiencia, sin sacrificar la legibilidad del texto, que sigue cumpliendo los estándares de alto contraste para personas mayores.

## Selección de proyecto en "Mi tejido"
Antes de llegar a la calculadora o al contador de vueltas, ahora hay un paso intermedio: **"¿Qué te gustaría tejer hoy?"**, con cuatro opciones ilustradas (Gorro, Bufanda, Chaleco, Manta). El proyecto elegido:
- Queda visible como una etiqueta dentro de "Mi tejido" y dentro de la calculadora.
- Ajusta automáticamente la base de cálculo de puntos: cada tipo de proyecto tiene su propia tabla de puntos por talla (una manta requiere muchos más puntos que un gorro, por ejemplo).
- El botón "atrás" desde "Mi tejido" devuelve a esta pantalla, para facilitar cambiar de proyecto sin volver al inicio.

## Vitrina comunitaria
Se agregó una sección social nueva, visible **antes** de entrar a cualquiera de los cuatro módulos principales, con una vista previa en el Home ("Lo que están tejiendo") que muestra publicaciones de otras personas usuarias.

Al entrar a la vitrina completa, cada publicación incluye:
- Foto del proyecto terminado
- Nombre de quien lo compartió y una descripción corta
- Botón de "me gusta", que reacciona visualmente al tocarlo
- Comentarios existentes de otras personas
- Un campo para dejar un mensaje propio, que se agrega a la publicación al instante

Esta sección busca reforzar el pilar de socialización del proyecto: no solo tejer, sino mostrar el resultado y recibir reconocimiento de otras personas de la comunidad, replicando la validación social que normalmente ocurre en un taller presencial.

## Nota técnica
En esta versión del prototipo, el video y las fotos de las publicaciones están incrustados directamente dentro del archivo `index.html` (como datos codificados), para que todo funcione en un solo archivo sin depender de rutas externas. Esto simplifica la publicación en GitHub Pages, a cambio de un archivo más pesado (~6 MB). En una versión de producción, estos archivos se servirían por separado desde un almacenamiento en la nube.
