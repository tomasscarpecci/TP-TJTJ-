# Propuesta TP DSW

## Grupo
### Integrantes
* 50955 - Scarpecci, Tomás Agustín
* 51434 - Vuelta, Tomás Manuel
* 50462 - Aquilante, Jazmín
* 51013 - Rodriguez, Maria Julieta

### Repositorios
* [frontend app](https://github.com/tomasscarpecci/frontend-app)
* [backend app](https://github.com/tomasscarpecci/backend-app)

## Tema
### Descripción
Nuestro Software se basa en una aplicación que funciona como un portal de noticias. Los usuarios podrán suscribirse a la plataforma aceptando un plan de pago, que puede variar de acuerdo al tipo de suscripcion (unipersonal, familiar, business). En la app se podrán visualizar noticias de diferentes editoriales asociadas a la plataforma y así poder tener diferentes puntos de vista sobre un mismo hecho. Lo innovador es que se podrán leer noticias completas de varios diarios (nacionales e internacionales) contratando una sola suscripcion, sin tener que registrarse en la pagina de cada editorial.

### Modelo
[Draw.io]([https://mermaid.js.org](https://drive.google.com/file/d/1vNt57zkz5b0-Ddx8Oxv6-CXo2ww_BEuQ/view?usp=sharing)) 

## Alcance Funcional 
|Req|Detalle|
|:-|:-|
|CRUD simple|1. CRUD Categoria<br>2. CRUD Usuario<br>3. CRUD Editorial<br>4. CRUD Tipo Suscripcion|
|CRUD dependiente|1. CRUD Noticia {depende de} CRUD CategoriaNoticia<br>2. CRUD Suscripción {depende de} CRUD TipoSuscripcion<br>3. CRUD PrecioSuscripcion {depende de} CRUD TipoSuscripcion |
|Listado<br>+<br>detalle| 1. Listado de noticias filtrado por categoría, muestra título, fecha y editorial => detalle muestra datos de la noticia y la editorial<br> 2. Listado de suscriptores filtrado por tipo suscripción, muestra nombre, usuario, mail, edad ⇒ detalle CRUD Suscriptor<br>3. Listado de noticias filtrado por suscriptor, muestra categoría de la noticia |
|CUU/Epic|1. Realizar suscripción de categoría para poder ver la noticia completa.<br>2.Anular suscripción si desea no continuar con esa categoría.|

