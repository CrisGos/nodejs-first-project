1. **¿Qué es el filesystem (fs) en Node.js y para qué se utiliza?**
   Es un módulo nativo de Node.js, node:fs permite interactuar con el sistema de archivos por medio del modelo de funciones POSIX, este permite realizar operaciones de leer, escribir, actualizar, borrar y manipular archivos y directorios.

2. **¿Qué es un middleware en Express y cuál es su propósito?**
   Son funciones que tienen acceso al object (req), y al response object (res), y la siguiente función de middleware en el ciclo de request-response. Dentro de sus propósitos están ejecutar cualquier código, hacer cambios al request y el response objects, finalizar el ciclo request-response y llamar la siguiente función middleware de la pila.

3. **¿Qué es un endpoint en una API RESTful y cuál es su función?**
   Un endpoint de API es la ubicación de la API en la que un sistema interactúa con una API web. También es el punto de comunicación entre dos sistemas, es la URL específica a la que se puede enviar una solicitud para realizar alguna operación en los recursos del servidor. Su función es definir el punto de acceso para realizar una operación especifica en un recurso particular.

4. **¿Qué son los verbos HTTP y cuáles son los más comunes?**
   Estos verbos indican la acción que se desea realizar para un determinado recurso en un servidor web, los más comunes son: GET (Recuperar o solicitar un recurso), POST (envía una entidad a un recurso especifico), PUT (reemplaza), DELETE (borra un recurso), etc.

5. **¿Qué es JSON y por qué es utilizado en las API RESTful?**
   JavaScript Object Notation o JSON es un formato de texto ligero para el intercambio de datos, es utilizado en la API REST debido a que es un formato de datos universal, su compatibilidad con JavaScript y además de que es ligero, fácil de leer, escribir y parsear por humanos y maquinas.

6. **En lo que respecta al envío de datos a lo largo de los verbos http responde:**
   - **¿Qué es el body de una petición?**
     Es la sección de la solicitud que contiene los datos que se envían al servidor, comúnmente van acompañados de los verbos HTTP.
   - **¿Qué es el body de una respuesta?**
     El body de una respuesta HTTP es la parte de la respuesta enviada desde el servidor al cliente que contiene los datos solicitados. Puede incluir HTML, JSON, XML, texto plano, archivos, etc.
   - **¿Qué es el query de una petición?**
     El query de una petición HTTP son los parámetros que se envían en la URL después del símbolo? Estos parámetros se utilizan para pasar datos al servidor de manera más simple, como filtros, paginación, o búsqueda.
   - **¿Qué es el params de una petición?**
     Los params (parámetros de ruta) de una petición HTTP son partes variables de la ruta de la URL que se utilizan para identificar recursos específicos. Estos parámetros se definen en la ruta de la URL y se capturan en el servidor para procesarlos.

7. **En lo que respecta al verbo POST responde:**
   - **¿Qué es un verbo POST y cuál es su propósito?**
     Es un método HTTP que permite enviar datos al servidor para crear un nuevo recurso.
   - **¿Cuándo se utiliza un verbo POST?**
     Se usa cuando se necesita crear recursos y enviar datos complejos.
   - **¿En qué se diferencia un verbo POST de los otros verbos HTTP como GET, PUT y DELETE?**
     Mientras el propósito de POST es crear un nuevo recurso en el servidor, el propósito de GET es recuperar datos de un recurso en el servidor, el propósito de PUT es actualizar un recurso existente en el servidor y DELETE permite eliminar un recurso existente en el servidor.
   - **¿Cómo se envían datos en un verbo POST?**
     Se envían en el body de la petición HTTP.

8. **En lo que respecta al verbo GET responde:**
   - **¿Qué es un verbo GET y cuál es su propósito?**
     Es un método HTTP utilizado para solicitar datos de un servidor, su principal propósito es recuperar información de un recurso especifico sin modificar el estado de este.
   - **¿Cuándo se utiliza un verbo GET?**
     Se utiliza cuando es necesario recuperar datos y/o leerlos sin modificarlos.
   - **¿En qué se diferencia un verbo GET de los otros verbos HTTP como POST, PUT y DELETE?**
     GET no utiliza body en la solicitud, es idempotente (múltiples peticiones al mismo recurso no cambian el estado de este) y lo propósito es recuperar un recurso, PUT modifica, POST agrega y DELETE elimina.

9. **En lo que respecta al verbo PUT responde:**
   - **¿Qué es un verbo PUT y cuál es su propósito?**
     Es un método HTTP utilizado para actualizar un recurso existente en el servidor o lo crea si esta no existe.
   - **¿Cuándo se utiliza un verbo PUT?**
     Se utiliza cuando se necesita actualizar un recurso o crear un recurso en el servidor.
   - **¿En qué se diferencia un verbo PUT de los otros verbos HTTP como POST, GET y DELETE?**
     El propósito del PUT es actualizar o crear un nuevo recurso, a diferencia del POST el PUT también permite actualizar.

10. **En lo que respecta al verbo DELETE responde:**
    - **¿Qué es un verbo DELETE y cuál es su propósito?**
      Es un método HTTP que permite eliminar un recurso especifico en el servidor.
    - **¿Cuándo se utiliza un verbo DELETE?**
      Se útil cuando se necesite eliminar un recurso del servidor.
    - **¿En qué se diferencia un verbo DELETE de los otros verbos HTTP como POST, GET y PUT?**
      DELETE permite eliminar recursos, mientras que los demás métodos permiten ya sea crear o interactuar con los existentes.

11. **¿Qué es un status code y cuáles son los más comunes?**
    Es una respuesta numérica que indica el resultado de una solicitud HPPT, cada código pertenece a una respuesta especifica, los más comunes son:
    1xx: Informacional
    2xx: Éxito
    3xx: Redirección
    4xx: Error del cliente
    5xx: Error del servidor

12. **¿Cuáles son los status code más comunes para el verbo POST?**
    201 Created: Indica que la solicitud ha tenido éxito y se ha creado un nuevo recurso como resultado.
    400 Bad Request: La solicitud no pudo ser entendida por el servidor debido a una sintaxis incorrecta o una solicitud que no debería repetirse.
    401 Unauthorized: Indica que se requiere autenticación para acceder al recurso.
    403 Forbidden: El servidor entiende la solicitud, pero se niega a autorizarla.
    422 Unprocessable Entity: La solicitud está bien formada pero no se puede procesar debido a errores semánticos.

13. **¿Cuáles son los status code más comunes para el verbo GET?**
    200 OK: La solicitud ha tenido éxito.
    400 Bad Request: La solicitud no pudo ser entendida por el servidor debido a una sintaxis incorrecta o una solicitud que no debería repetirse.
    401 Unauthorized: Indica que se requiere autenticación para acceder al recurso.
    404 Not Found: El servidor no pudo encontrar el recurso solicitado.
    500 Internal Server Error: Indica un error genérico en el servidor que no se puede clasificar.

14. **¿Cuáles son los status code más comunes para el verbo PUT?**
    200 OK: La solicitud ha tenido éxito.
    201 Created: Indica que la solicitud ha tenido éxito y se ha creado un nuevo recurso como resultado.
    400 Bad Request: La solicitud no pudo ser entendida por el servidor debido a una sintaxis incorrecta o una solicitud que no debería repetirse.
    404 Not Found: El servidor no pudo encontrar el recurso solicitado para actualizar.
    409 Conflict: Indica que la solicitud no se pudo completar debido a un conflicto con el estado actual del recurso.

15. **¿Cuáles son los status code más comunes para el verbo DELETE?**
    200 OK: La solicitud ha tenido éxito.
    204 no Content: La solicitud se ha procesado con éxito y el servidor no devuelve ningún contenido.
    404 Not Found: El servidor no pudo encontrar el recurso solicitado para eliminar.
    401 Unauthorized: Indica que se requiere autenticación para acceder al recurso.
    403 Forbidden: El servidor entiende la solicitud, pero se niega a autorizarla.
