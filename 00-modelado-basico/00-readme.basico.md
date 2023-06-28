# laboratorio 01 - modelado

## caso básico

![imagen](./content/pantallazo.pdf)


He creado tres colecciones para completar los requerimientos del modelado inicial: curso, temática y autor. Dicha división
la considero justificada por los siguientes puntos:

El primer enunciado *"Queremos mostrar los últimos cursos publicados"* se satisface añadiendo el campo **fecha** para poder sacar rápidamente los que se hayan publicado más recientemente y poder mostrarlo en el apartado de novedades (o similar) en la página de incio. Se ha añadido fecha también al campo **cursos**, descendiente de la colección **temática**, para que aparezcan ordenados por fecha en la página de inicio, sin tener que abrir la colección de **curso**.

El segundo enunciado *"Queremos mostrar cursos por área (devops / front End ...)"* se satisface añadiendo una colección con el nombre 
**temática**, donde vienen listados los cursos, los cuales se pueden ordenar por fecha, y se puede ampliar información accediento a la colección de **curso**.

El tercer enunciado *"Queremos mostrar un curso con sus videos"* se satisface con la colección de **curso**, donde viene descrito en detalle, se puede acceder a los videos y a los autores de cada curso.

El cuarto y último enunciado *"En un video queremos mostrar su autor*" se satisface añadiendo el campo **autor** a cada lección, donde pueden ver una descripción corta de dicho autor. Si se desea ampliar información, se ha creado una colección aparte donde aparezca toda la información necesaria, sin sobrecargar el *Working Set*.