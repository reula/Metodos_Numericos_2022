## Instrucciones de como acceder a la instancia de jupyterhub de FaMAF

En la Facultad tenemos instalado (gracias a Nicolás Wolovick) un servidor de jupyterhub. 
Para acceder a el se necesita: 

1. tener una cuenta en la computadora `atom` la cual será provista a todos los alumnos del curso.

2. tener un cliente de ssh (secure shell) en su computador personal. En linux viene por defecto, para Windows se puede usar uno llamado Putty.exe (https://www.putty.org/)
3. Tener un browser.

Una vez que tenga su `usuario` y `contraseña` deberá ingresar a la computadora `atom@famaf.unc.edu.ar` por una conexión con tunel 
(es decir una conexión donde todo servicio de web se hace a travéz de un puerto de comunicación seguro).

Desde linux el comando para establecer dicha conexión es:

`mi computadora> ssh -L 8000:localhost:8000 usuario@atom.famaf.unc.edu.ar`

Una vez que lo ejecute le aparecerá la solicitud de contraseña y una vez que la haya ingresado con éxito aparecerá una terminal donde 
podrá ingresar comandos en la computadora remota (`atom`). Pero eso no será momentáneamente necesario.

A continuación habra su browser e ingrese la dirección:

http://localhost:8000

Le deberá aparecer una pantalla del jupyterlab remoto en esa página. Desde allí podrá trabajar con Julia.



