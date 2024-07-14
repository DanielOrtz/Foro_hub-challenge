# Foro_hub-challenge
Se les presenta mi Foro Hub la cual es un Web API  creado en Java Spring, que se basa en REST siendo de importancia para la finalizacion del curso #alura
<h1>Tablas de la base de datos</h1>

Esta aplicacion se conecta a una base de datos MySQL, la cuàl contiene una serie de tablas:

<ul>
  <li>Tabla course: Contiene los cursos que se imparten en el foro.</li>
  <li>Tabla status: Contiene el estado de los tópicos </li>
  <li>Tabla profile: Contiene los diferentes tipos de perfiles de los usuarios </li>
  <li>Tabla user: Contiene los usuarios que crean tópicos, respuestas a esos tópicos.</li>
  <li>Tabla topic: Es la parte fundamental del challenge, crea el foro o la consulta que tiene un usuario en el sistema.</li>
  <li>Tabla responses: Contiene las respuestas a cada de los tópicos del sistema.</li>
  
</ul>
<h1>REQUERIMIENTOS PREVIOS PARA UTILIZAR EL FORO </h1>
<ul>
  <li>  Java 17 JDK </li>
  <li>Maven</li>
  <li>Spring Boot</li>
  <li>Spring Security con JWT</li>
  <li>Spring JavaDoc Swagger</li>
  <li>Base de datos MySQL (nombre del esquema: forohub)</li>
  <li>Herramientas de desarrollo (IntelliJ IDEA) </li>
  <li>Insomnia </li>
  <li> MySQL Workbench para gestión de bases de datos</li>
</ul>
<H1>OBJETIVO EN DIAGRAMA</H1>
<img src="https://github.com/DanielOrtz/Foro_hub-challenge/blob/main/Imagenes%20readme/diagrama_base_de_datos_forohub.png">

<H1>EJECUCION</H1>
Después de ejecutar la aplicación localmente, tienes la oportunidad de acceder a la documentación de Swagger UI en http://localhost:8080/swagger-ui/index.html#/. para obtener detalles sobre los endpoints de la API 
<H1>ENDPOINTS</H1>
<H3>Controlador de Usuarios</H3>
<ul>
 <li>GET /users: Obtiene una lista de 10 usuarios.</li>
 <li>PUT /users/{id}: Actualiza la información del usuario proporcionando el ID del usuario junto con el nombre o el correo electrónico actualizado.</li>
 <li>GET /users/{id}: Obtiene los detalles de un usuario por ID.</li>
</ul>
<H3> Controlador de Temas </H3>
<ul>
 <li>GET /topics: Obtiene una lista de temas.</li>
 <li>POST /topics: Crea un nuevo tema proporcionando título, mensaje, estado, ID de usuario y curso.</li>
 <li>GET /topics/{id}: Obtiene un tema por ID.</li>
   <li> DELETE /topics/{id}: Elimina un tema por ID.</li>
</ul>

<H3> Controlador de Respuestas </H3>
<ul>
<li>POST /responses: Publica una respuesta (comentario) a un tema proporcionando solución, ID de usuario y ID de tema.</li>
<li>GET /responses: Obtiene una lista de respuestas.</li>
<li>GET /responses/{id}: Obtiene una respuesta por ID.</li>
<li>PUT /responses/{id}: Modifica una respuesta por ID.</li>
<li>DELETE /responses/{id}: Elimina una respuesta por ID.</li>
</ul>

<H3> Controlador de Registro </H3>
<ul>
<li>POST /register: Crea un nuevo usuario para el registro.</li>
</ul>
<H3> Controlador de Autenticación </H3>
<ul>
<li>POST /authenticate: Autentica el inicio de sesión del usuario con Spring Security y JWT. Para acceder a la mayoría de los endpoints, necesitas autenticarte con un token Bearer obtenido del endpoint /authenticate.</li>
</ul>
<H3>Ejemplo</H3>
<img src="https://github.com/DanielOrtz/Foro_hub-challenge/blob/main/Imagenes%20readme/ejemplo.JPG">
<h3>Ejecucion del programa
</h3>
<img src="https://github.com/DanielOrtz/Foro_hub-challenge/blob/main/Imagenes%20readme/ejecucion.JPG">
<h1>INDICACIONES FINALES</h1>
<ul>
 <li>Clona este repositorio.</li>
 <li>Configura tu base de datos y ajusta las configuraciones de conexión en application.properties.</li>
 <li>Por seguridad usa variables de entorno.</li>
 <li>Compila y ejecuta la aplicación Spring Boot.</li>
</ul>
<H1>INSIGNIA</H1>
<img src="https://github.com/DanielOrtz/Foro_hub-challenge/blob/main/Badge-Spring.png">
