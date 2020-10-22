# FAQ a revisar antes de ser publicadas

#### <a name="FAQ-A-4"></a>A.4 Alegaciones sobre privacidad y seguridad de RadarCovid.
 
**A.4.1 El Pais avisa 22/10/2020** de "una brecha de seguridad" en Radar Covid: "si hay subida al servidor implica que el usuario es positivo. Quien tenga acceso al tráfico, por tanto, sabe quién lo es" [enlace](https://elpais.com/tecnologia/2020-10-22/la-app-radar-covid-ha-tenido-una-brecha-de-seguridad-desde-su-lanzamiento.html)

Le contesta [en tuit @imartinezortiz](https://twitter.com/imartinezortiz/status/1319201482407923714): La noticia es  alarmista. Amazon Web Services puede conocer la interacción, al igual que el proveedor de internet del usuario del teléfono ya que: 1) la resolución DNS por defecto no está cifrada, 2) las conexiones TLS, por defecto, también pueden saber el servidor de destino. Los datos enviados son anónimos y requerirían colaboración  para asignar un nombre a la IP origen (aunque hay otras maneras). Para eso existen los contratos con los proveedores de la nube, para que no miren la tubería, si no tendríamos los servidores debajo de la mesa. Los datos son anónimos y la comunicación está cifrada. El sustrato sobre el que se construye RadarCovid es el mismo que se utiliza en el resto de aplicaciones europeas.

También contesta [en tuit @pvieito](https://twitter.com/pvieito/status/1319224757619916800) Es totalmente cierto que el titular es alarmista (¿brecha de seguridad?) pero también que el protocolo DP3T se diseñó con el concepto de subidas de diagnóstico falsas precisamente para mitigar esta posibilidad y Radar COVID no las hacía hasta hace poco.



Actualizado: 22/10/2020 version 12


