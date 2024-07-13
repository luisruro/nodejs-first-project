## ¿Qué es el filesystem (fs) en Node.js y para qué se utiliza?

Te permite interactuar con el sistema de archivos de la computadora. Así que puedes leer lo que hay dentro de un archivo, 
escribir nuevos archivos, crear archivos o directorios y borrarlos

## ¿Qué es un middleware en Express y cuál es su propósito?

Es como un ayudante que hace algo específico mientras una solicitud o request esta en proceso,
por ejemplo un middleware puede leer la información que viene en la solicitud y modificarla si es necesario,
también verificar si la solicitud cumple ciertos requisitos, por ejemplo si el usuario esta autorizado y realizar acciones adicionales como
guardar información en un archivo o en una base de datos. Básicamente el proposito es manejar diferentes partes del proceso por el que pasa una solicitud desde que llega hasta que se
envía una respuesta y se asegura de que todo este bien antes de que la solicitud continúe su camino.

## ¿Qué es un endpoint en una API RESTful y cuál es su función?

Un endpoint es un lugar específico al que se puede ir para hacer una acción particular. Cada endpoint tiene una URL y te dice exactamente qué puedes hacer allí.
por ejemplo GET/juguetes Deja ver todos los juguetes disponibles, POST/juguetes este agrega un nuevo juguete, PUT/juguetes/1 este permite actualizar la información de un juguete en específico
DELETE/juguetes/1 este te elimina el juguete número uno. Básicamente la función es recibir una solicitud (request) y devolver una respuesta (response).

## ¿Qué son los verbos HTTP y cuáles son los más comunes?

Los verbos HTTP son métodos o reglas que le indican la acción que queremos que la API haga. Los verbos más comunes son GET= es para ver la información, POST= es para agregar información,
PUT= es para actualizar algo que ya existe, PATCH= es solamente para cambiar algo en especifico, y DELETE= es para eliminar.


## ¿Qué es JSON y por qué es utilizado en las API RESTful?

Es un formato de texto que usa pares de clave:valor para organizar la información, en las API RESTful es muy utilizado porque es facil de leer y escribir,
es ligero ya que no ocupa mucho espacio, así que es rápido de enviar y recibir a través de la red, también es compatible porque funciona bien con muchos lenguajes de programación
y es estructurado, tiene una estructura clara lo que lo hace más organizado y facilita el acceso a la información.

***En lo que respecta al envio de datos a lo largo de los verbos http responde:***

## ¿Qué es el body de una petición?

El body es el contenido, es la parte donde se pone la información detallada que quieres enviar, con el body no utilizamos los verbos GET y DELETE ya que el primero
solo pide información y segundo solo necesita saber que eliminar sin enviar datos adicionales.

## ¿Qué es el body de una respuesta?

Es donde se ve la respuesta que contiene la información que el servidor está enviando de vuelta, luego de hacer la petición o también mostrar mensajes de error.

## ¿Qué es el query de una petición?

Son como las instrucciones especificas que se agregan a la solicitud. Se coloca al final de la URL y empieza con una signo de interrogación, seguido de pares de clave=valor, 
separador por el símbolo "&". Es muy útil porque da precisión ya que se pide exactamente lo que uno necesita, es eficiente ya que reduce la cantidad de datos que se envían.

## ¿Qué es el params de una petición?

Los params o parámetros de ruta son partes especificas de la URL que indican recursos individuales dentro de una colección por ejemplo
GET/juguetes/123 aquí estaria pidiendo informaciónsolo sobre el juguete con el ID 123

***En lo que respecta al verbo POST responde:***

## ¿Qué es un verbo POST y cuál es su propósito?

Se utiliza para enviar datos al servidor para su procesamiento y se envián en el cuerpo de la solicitud, normalmente se utiliza para enviar formularios, cargar archivos y otras operaciones
que requieren enviar datos al servidor

## ¿Cuándo se utiliza un verbo POST?

Cuándo quieres enviar datos al servidor para crear un nuevo recurso

## ¿En qué se diferencia un verbo POST de los otros verbos HTTP como GET, PUT y DELETE?

Cada verbo tiene su función especifica en la interaccion de la API, entonces el POST crea nuevos recursos y evía datos al servidor, GET trae los datos sin hacer cambios, PUT actualiza los recursos
existentes reemplazandolos y DELETE elimina los recursos del servidor

## ¿Como se envian datos en un verbo POST?

Hay varias maneras, dependiendo de cómo esté configurada la API

***En lo que respecta al verbo GET responde:***

## ¿Qué es un verbo GET y cuál es su propósito?

Se utiliza para traer información del servidor y el servidor devuelve el contenido del recurso solicitado en la respuesta.

## ¿Cuándo se utiliza un verbo GET?

Cuando quiero traer información del servidor sin modificarla.

## ¿En qué se diferencia un verbo GET de los otros verbos HTTP como POST, PUT y DELETE?

Cada verbo tiene su función especifica en la interaccion de la API, entonces el POST crea nuevos recursos y evía datos al servidor, GET trae los datos sin hacer cambios, PUT actualiza los recursos
existentes reemplazandolos y DELETE elimina los recursos del servidor

***En lo que respecta al verbo PUT responde:***

## ¿Qué es un verbo PUT y cuál es su propósito?

Se utiliza para actualizar un recurso del servidor ya existente.

## ¿Cuándo se utiliza un verbo PUT?

Cuándo quiero actualizar un recurso del servidor ya existente y los datos se envían en el cuerpo de la solicitud y el servidor actualiza el recurso con los datos proporcionados en el body

## ¿En qué se diferencia un verbo PUT de los otros verbos HTTP como POST, GET y DELETE?

Cada verbo tiene su función especifica en la interaccion de la API, entonces el POST crea nuevos recursos y evía datos al servidor, GET trae los datos sin hacer cambios, PUT actualiza los recursos
existentes reemplazandolos y DELETE elimina los recursos del servidor

***En lo que respecta al verbo DELETE responde:***

## ¿Qué es un verbo DELETE y cuál es su propósito?

Se utiliza para eliminar un recurso en el servidor

## ¿Cuándo se utiliza un verbo DELETE?

Cuándo quiero eliminar un recurso específico en el servidor

## ¿En qué se diferencia un verbo DELETE de los otros verbos HTTP como POST, GET y PUT?

Cada verbo tiene su función especifica en la interaccion de la API, entonces el POST crea nuevos recursos y evía datos al servidor, GET trae los datos sin hacer cambios, PUT actualiza los recursos
existentes reemplazandolos y DELETE elimina los recursos del servidor

## ¿Qué es un status code y cuáles son los más comunes?

es un número o código que el servidor envía en la respuesta HTTP para indicar el resultado de una solicitud, cada código tiene un significado específico y ayuda a entender
si la solicitud fue exitosa o ocurrió algun error. los códigos mas comunes son:
***Éxito son los 2***

 - 200 OK, se proceso correctamente
 - 201 Created se creo un recurso correctamente
 - 204 No content la solicitud se completó, pero no hay contenido que
   devolver.

***Redirección los 3***

 - 301 Moved Permanently el recurso solicitado se ha movido a una nueva URL permanente
 - 302 Found el recurso se ha encontrado, pero se debe acceder a él
   temporalmente en otra URL

***Código de error del cliente los 4*** 

 - 400 Bad Request la solicitud no se puede procesar debido a un error
   del cliente (por ejemplo datos faltantes)
 - 401 Unauthorized se requiere autenticación para acceder al recurso
 - 403 Forbidden el acceso al recurso está prohibido, incluso con
   autenticación
 - 404 Not Found el recurso solicitado no se pudo encontrar en el
   servidor

***Código de error del servidor los 5*** 

 - 500 Internal Server Error ocurrio un error inesperado en el servidor 
 - 503 Service Unavailable el servidor no está disponible temporalmente,
   generalmente por mantenimiento.

## ¿Cuales son los status code mas comunes para el verbo POST?

200, 201, 204, 400, 401, 403, 409 Conflict ocurre un conflicto al procesar la solicitud, como intentar crear un recurso que ya existe. 
los códigos 201 Created y 400 Bad Request son especialmente relevantes, ya que indican si la creación del recurso fue exitosa o si hubo problemas con la solicitud.

## ¿Cuales son los status code mas comunes para el verbo GET?

200, 204, 301, 302, 400, 401, 403, 404
los códigos 200 OK y 404 Not Found son los más relevantes, indicando si la solicitud fue exitosa o si el recurso no se encontró

## ¿Cuales son los status code mas comunes para el verbo PUT?

200, 204, 201, 400, 401, 403, 404, 409
los códigos 200 OK, 204 No Content, y 404 Not Found son especialmente relevantes, indicando el éxito de la actualización o si el recurso no existe.

## ¿Cuales son los status code mas comunes para el verbo DELETE?

200, 204, 400, 401, 403, 404, 409
los códigos 204 No Content y 404 Not Found son especialmente relevantes, indicando el éxito de la eliminación o si el recurso no existe.