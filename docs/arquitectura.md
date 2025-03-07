
## Para la seleccion del tech stack se tuvo en cuenta lo siguiente:

- La aplicacion debe ser flexible para introducir cambios
- La interfaz de usuario debe contener la mayor cantidad de facilidades posibles para el usuario. Lo más simple y eficientemente posible 
- Los usuarios serán muy pocos 
- Se espera un trafico nulo-bajo
- El equipo de desarrolladores consta de una sola persona, con la remota posibilidad de incluir a alguien de manera esporadica, por lo que tiene que ser facil para ponerse al corriente
- Los desarrolladores tienen poca y nula experiencia desarrollando aplicaciones web. Solo aplicaciones de escritorio, sin frameworks (con patron mvc), scripts de exploracion y visualizacion de datos, una pequeña introduccion a APIs y muy poco contacto con bases de datos (solo contenido teorico).  

Las consideraciones fueron las siguientes despues de una investigacion parra tener al menos una introduccion a la decision a abordar:

### Posibles tech stacks

 - *Frontend*:
	 - HTML, CSS
  - *Frameworks*: 
	- Javascript:
		  - React 
		  - React native
		  - Angular 
	- Java:
		- Spring Boot 
	- Python:
		- Flask 
	- C++:
		- Qt

### Posibles arquitecturas
- Server side aproach:
	- Microservices 
	- Monolith 
	- Serverless
- Client side aproach:
	- Single-page application 
	- Multi-page application 
	- Progresive web application 
	- Micro frontend

## Algunos recursos utilizados: 
Architecture:
https://medium.com/tradeling/how-to-design-software-architecture-c39eb5481a07
https://www.reddit.com/r/developersIndia/comments/187eulq/if_not_mern_then_what/?rdt=56293
https://www.youtube.com/watch?v=LSEYdU8Dp9Y
https://www.youtube.com/watch?v=yB4n_K7dZV8&t=3315s
https://www.researchgate.net/figure/Framework-schematics-Framework-is-based-on-a-server-client-model-where-the-server_fig1_341199552
https://medium.com/slalom-blog/web-development-architecture-patterns-and-when-to-use-them-9037c1eef5a0
https://www.digiteum.com/web-application-architecture/

El recurso más relevante terminó por ser https://medium.com/slalom-blog/web-development-architecture-patterns-and-when-to-use-them-9037c1eef5a0, y dialogando con IA's, se terminó por seleccionar una arquitectura *Monolitica* para el mvp, donde el modelo esté contentrado en el lado del servidor aunque teniendo en cuenta la proyeccion o el redireccionado a una arquitectura de *microservicios* en un futuro.
Tambien se optó por una presentacion del producto en una "single-page aplication" para intentar obtener una interaccion con los usuarios lo mas simplificada y suave posible.
Y por ultimo se busca desarrollar priorizando abstracciones entre las distintas capas de la arquitectura para simplificar la relacion entre estos y poder mantener una capa de reutilizacion y flexibilidad.