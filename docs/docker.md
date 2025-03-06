
1. Para crear una imagen con el Dockerfile: ´docker build -t gya-image .´
*Asegurarse de que docker esta como servicio corriendo de fondo en el SO paa cada comando a ejecutar*

2. Con la imagen creada ya se pueden levantar contenedores con servicios encima usando el comando: ´docker run --name "nombre del contenedorr nuevo a levantar" -it gya-image´
*Se puede tambien no usar el "-it" y el contenedor quedará corriendo de fondo sin necesidad de interactuar con el*
*Para cerrar el proceso escribir "exit" en el terminal bash del contenedor*

3. Para volver a levantar el contenedor no hace falta volver a construir la imagen, solo corer el comando 'docker start "nombre del conenedor creado en el paso 2"' 