# Sobre la "brecha de seguridad" de Radar COVID

## P - ¿Es verdad que Amazon u otras empresas tiene o ha tenido acceso a esta información? 
**TL;DR**: No. Al menos, no en ninguna forma práctica.

Esa afirmación está bastante sacada de contexto:

Los servidores de Radar COVID están efectivamente en dominio de Amazon Web Services, AWS, (Amazon en adelante), a quien se le alquilan estos equipos, como muchos otros proyectos tecnológicos pertenecientes a empresas privadas o al ámbito público.

Amazon, al ser los dueños de estos equipos, tienen la capacidad de ver la información que hay en ellos. Es como si alguien almacena fotos en tu PC, podrías verlas si quisieses.

Sin embargo, tal acción violaría la GDPR por parte de Amazon, y sería un escándalo en si mismo. **No hay ninguna prueba ni indicio de que tal cosa haya ocurrido ni vaya a ocurrir**.

Por otro lado, Amazon solo podría ver unas etiquetas que son aleatorias (ver "como funciona este fallo"), y unas direcciones de internet que, afinando en el peor de los casos, determinan a una casa entera, no a un individuo. En casos más realistas, Amazon tendría que trabajar con una empresa de servicio de internet para poder cruzar estos datos, lo cual sería una vez más una violación de varias leyes.

Para terminar, ninguna otra empresa es dueña de estos servidores, y las unicas otras entidades que podrían ver este flujo de datos son los proveedores de internet. Que se encontrarían con menos información aun, dado que no pueden leer la "etiqueta" del positivo.

Por tanto, **ninguna empresa ha visto estos datos, ni podrían hacer nada con ello si lo hicieran**.

----
----
## P - ¿Como funciona este fallo?

La aplicación se comunica con sus servidores para comunicar un positivo del usuario, y  para descargar los nuevos positivos, de forma que se puede averiguar si el usuario ha estado en contacto con alguno de ellos.

Estas comunicaciones se hacen de forma segura, y es imposible leer "que pone" en esas comunicaciones.

Sin embargo, *era posible* diferenciar entre una comunicación de positivo del usuario y una comunicación de "actualizar los positivos que ha habido".

De esta forma, si alguien consigue ver que se ha hecho una comunicación de positivo, entonces se puede saber que ese usuario es positivo.

Como se puede apreciar, el único ataque a la privacidad factible es de un individuo a otro, y no desde una empresa, ya que el proceso ocurre cerca del individuo positivo.

----

Alguien con suficientes conocimientos puede "ver" esa comunicación, pero se han de cumplir los siguientes requisitos:
- El atacante tiene que estar en la misma red que el positivo. Por ejemplo, el wifi de casa, o el de algún restaurante. Por reiterar, alguien **fuera de la red WiFi** (o en una red distinta, como en las oficinas grandes) tampoco vería esta comunicación. O, por ejemplo, si se reportó usando los datos móviles (3g,4g...), también sería "invisible" para un atacante.

- El atacante tiene que estar "escuchando" en la red **durante el momento exacto** que se comunica el positivo. Antes o después no se puede detectar nada.

- La comunicación que se ve en la red **identifica a un dispositivo** en ella, **no a una persona**. El atacante tiene que poder identificar al usuario del dispositivo para obtener su identidad, cosa más o menos fácil dependiendo del numero de dispositivos y gente en la red.

----
----
## P - ¿Puedo averiguar si alguien sabe si yo he dado positvo mediante este fallo?
Lamentablemente, a posteriori es imposible saberlo.

Sin embargo, el fallo abre una ventana muy pequeña de tiempo y con unas condiciones muy concretas para que alguien haya podido aprovecharlo de forma realista (ver pregunta anterior).

Dado que además este fallo no era público, combinado con lo poco que tiene que ganar un posible atacante, hace que en la realidad es extremadamente poco probable que nadie lo haya sufrido.

**Si se ha mantenido en redes privadas o datos móviles al dar el positivo en la app, es muy probable que nadie haya podido emplear este ataque contra usted**

----
----
## P - ¿El problema sigue activo?
No, la aplicación se ha actualizado para fingir comunicaciones de "positivo" al servidor, de forma que ahora es immposible adivinar si es verdad o no para un atacante.