# Radar COVID – Documentación
## Respuesta a Preguntas Frecuentes (FAQ)
 
_Proyecto de la [Unidad Tecnológica de Voluntariado](http://utv.com.es)._
 
## Objeto

Dar respuesta a las consultas que se formulan sobre la aplicación Radar COVID tanto sobre su funcionamiento cómo su arquitectura más técnica. Va dirigida a las personas que no encuentan información oficial suficiente. Responde también a preguntas sobre el proyecto Radar STATS.

## Índice

- [**Preguntas frecuentes**](#preguntas-frecuentes)
  * [**A. Instalación de Radar COVID**](#FAQ-A)
    * [A.1. ¿En qué móviles se puede instalar?](#FAQ-A-1)
    * [A.2. ¿Cónsume mucha batería Radar COVID?](#FAQ-A-2)
    * [A.3. ¿Tiene fallos de seguridad o privacidad Radar COVID?](#FAQ-A-3)
    * [A.4. Alegaciones sobre privacidad y seguridad de Radar COVID.](#FAQ-A-4)
    * [A.5 Rebaja por consumo de datos en Radar COVID en algunas operadoras.](#FAQ-A-5)
  * [**B. Funcionamiento de Radar COVID**](#FAQ-B)
    * [B.1. ¿Se puede instalar Radar COVID después de que me den el resultado positivo en un test?](#FAQ-B-1)
    * [B.2. ¿A qué horas calcula mi móvil las notificaciones si un usuario de un móvil próximo ha comunicado un test positivo?](#FAQ-B-2)
    * [B.3. ¿Si vivo en una Comunidad Autónoma (CCAA) que no proporciona código para comunicar un positivo ¿puedo recibir notificaciones de contacto alto?](#FAQ-B-3)
    * [B.4. Nuevas versiones de Radar COVID](#FAQ-B-4)
    * [B.5. ¿Qué ocurre a Radar COVID después de que se comunica un diagnóstico positivo?](#FAQ-B-5)
    * [B.6. Radar COVID ha considerado una exposición pero no la ha catalogado como significativa.](#FAQ-B-6)
  * [**C. Errores de Radar COVID**](#FAQ-C)
    * [C.1. Radar COVID no funciona correctamente en Android: “Ahorro de energía activado. Debes desactivarlo para que Radar COVID funcione correctamente.”](#FAQ-C-1)
    * [C.2. Radar COVID no funciona correctamente en Android: “Error al cargar nuevos datos de infección”](#FAQ-C-2)
  * [**D. Información sobre Radar STATS**](#FAQ-D)
    * [D.1. ¿Qué hace Radar STATS?](#FAQ-D-1)
    * [D.2. La interoperabilidad de las aplicaciones europeas y la pérdida de detalle estadístico.](#FAQ-D-2)
  * [**E. Información técnica sobre Radar COVID**](#FAQ-E)
     * [E.1. ¿Cómo puedo ver el listado de comprobaciones de exposición en Android?](#FAQ-E-1)
     * [E.2. ¿Cómo puedo ver el listado de comprobaciones de exposición en iOS?](#FAQ-E-2)
     * [E.3. ¿Qué es una comprobación de exposición?](#FAQ-E-3)
     * [E.4. Funcionamiento técnico de Radar COVID](#FAQ-E-4)
     * [E.5. Funcionamiento técnico de Radar COVID 2. El servidor de verificación.](#FAQ-E-5)
  * [**F. Internacional**](#FAQ-F)
    * [F.1. Aplicaciones similares a Radar COVID en otros países](#FAQ-F-1)
    * [F.2. Documentación sobre el acuerdo de Google-Apple para intercambio a través de Bluetooth](#FAQ-F-2)
    * [F.3. Las aplicaciones de diferentes países ¿son compatibles? ¿Un suizo de vacaciones por España, si da positivo y lo mete en SwissCovid, comunica su positivo a quienes tienen la aplicación española?](#FAQ-F-3)
  * [**Z. Implantación en Comunidades Autónomas**](#FAQ-Z)
    * [Z.1. Comunidades Autónomas (CCAA) cuyo sistema sanitario proporciona el código de 12 cifras para comunicar un diagnóstico positivo](#FAQ-Z-1)
    * [Z.2. Cómo comunican las Comunidades Autónomas el código de 12 digitos](#FAQ-Z-2)
- [**Enlaces oficiales**](#enlaces-oficiales)
- [**Glosario**](#glosario)
- [**Reglas de estilo**](#reglas-de-estilo)
- [**Contacto y colaboradores**](#contacto)
- [**Versión**](#versión)

## Preguntas frecuentes

### <a name="FAQ-A"></a>A. Instalación de Radar COVID

#### <a name="FAQ-A-1"></a>A.1. ¿En qué móviles se puede instalar?

- En los móviles con Android 6.0 o posterior.
- En los móviles iPhone requiere un sistema 13.5 o posterior.
 
No se puede instalar en:  
 
- Móviles con versiones de Android anterior a la 6.0.  
- Móviles Huawei y Honor de última generación sin Google Play Services.  
- Cualquier móvil de otros fabricantes que no tengan Google Play.

| Estado | Actualización | Fuentes |
| --- | --- | --- |
| Aprobado | 06/10/2020 | [Xataka](https://www.xataka.com/basics/que-moviles-puedes-no-puedes-instalar-app-radar-covid), [App Store](https://apps.apple.com/es/app/radar-covid/id1520443509), [Twitter (@SEDIAgob)](https://twitter.com/SEDIAgob/status/1295277894424551424) |
 
#### <a name="FAQ-A-2"></a>A.2. ¿Cónsume mucha batería Radar COVID?

No.

[@YoryoBass](https://twitter.com/YoryoBass/status/1312445670922489857):

> "En general, el protocolo Bluetooth es muy robusto y el rendimiento no se degrada demasiado a menos que haya cientos de dispositivos en una proximidad cercana."
>
> …
>
> La evidencia del acierto de la elección de Bluetooth de baja energía (BLE) para ser usado en aplicaciones de rastreo de contactos es apabullante.

Hemos hecho el siguiente experimento. De su naturaleza no pueden obtenerse conclusiones pero puede dar indicios.

Hemos tomado una Galaxy S7 Edge con Android 8.0. Durante 24 horas no ha hecho ni recibido llamadas. Ha tenido conexión con servicios Internet (WhatsApp, Twitter y Email) Ha estado en la calle 90 minutos. Tiene Radar COVID instalada. Y hemos hecho dos pruebas durante 24 horas cada una: a) con Bluetooth y Ubicación activadas y b) con Bluetooth y Ubicación desactivadas.

- a) La batería ha pasado de una carga del 100% a una carga del 80%.
- b) La batería ha pasado de una carga del 100% a una carga del 80% (coincide con a).


| Estado | Actualización | Fuentes |
| --- | --- | --- |
| Aprobado | 26/10/2020 | [Twitter (@YoryoBass)](https://twitter.com/YoryoBass/status/1312445670922489857) |

#### <a name="FAQ-A-3"></a>A.3. ¿Tiene fallos de seguridad o privacidad Radar COVID?

Parece que no tiene fallos de seguridad o privacidad. Diversos expertos han examinado el código y no consta que haya resquicios de seguridad. Como ejemplo incluimos un informe de la [Organización de Consumidores y Usuarios](https://www.ocu.org/tecnologia/telefono/noticias/radar-covid#) transmitido por la agencia [Europa Press](https://www.europapress.es/asturias/noticia-ocu-confirma-aplicacion-radar-covid-no-registra-datos-personales-segura-20201007124451.html).

Ha suscitado dudas que en Android obliga a tener activada la localización o ubicación. En este [enlace de Xataka](https://www.xataka.com/aplicaciones/que-radar-covid-no-funciona-gps-activo-android-hace-iphone) se indica que Android necesita tener los servicios de localización activos para que funcione la conexión de móviles por Bluetooth pero que Radar COVID no registra esta ubicación. En este [enlace del soporte de Google](https://support.google.com/googleplay/answer/9888358?hl=es) se indica que con Android 11 "no es necesario activar los ajustes de ubicación".

| Estado | Actualización | Fuentes |
| --- | --- | --- |
| Aprobado | 08/10/2020 | [OCU](https://www.ocu.org/tecnologia/telefono/noticias/radar-covid#), [Europa Press](https://www.europapress.es/asturias/noticia-ocu-confirma-aplicacion-radar-covid-no-registra-datos-personales-segura-20201007124451.html), [Xataka](https://www.xataka.com/aplicaciones/que-radar-covid-no-funciona-gps-activo-android-hace-iphone) |

#### <a name="FAQ-A-4"></a>A.4 Alegaciones sobre privacidad y seguridad de Radar COVID.
 
**A.4.1 El Pais avisa 22/10/2020** de "una brecha de seguridad" en Radar COVID: "si hay subida al servidor implica que el usuario es positivo. Quien tenga acceso al tráfico, por tanto, sabe quién lo es" [enlace](https://elpais.com/tecnologia/2020-10-22/la-app-radar-covid-ha-tenido-una-brecha-de-seguridad-desde-su-lanzamiento.html)

Le contesta [en tuit @imartinezortiz](https://twitter.com/imartinezortiz/status/1319201482407923714): 
> La noticia es alarmista. Amazon Web Services puede conocer la interacción, al igual que el proveedor de internet del usuario del teléfono ya que: 1) la resolución DNS por defecto no está cifrada, 2) las conexiones TLS, por defecto, también pueden saber el servidor de destino. Los datos enviados son anónimos y requerirían colaboración  para asignar un nombre a la IP origen (aunque hay otras maneras). Para eso existen los contratos con los proveedores de la nube, para que no miren la tubería, si no tendríamos los servidores debajo de la mesa. Los datos son anónimos y la comunicación está cifrada. El sustrato sobre el que se construye Radar COVID es el mismo que se utiliza en el resto de aplicaciones europeas.
>

También contesta [en tuit @pvieito](https://twitter.com/pvieito/status/1319224757619916800) 
> Es totalmente cierto que el titular es alarmista (¿brecha de seguridad?) pero también que el protocolo DP3T se diseñó con el concepto de subidas de diagnóstico falsas precisamente para mitigar esta posibilidad y Radar COVID no las hacía hasta hace poco.

La **Unidad Tecnológica de Voluntariado, @UTVoluntariado** [en este tuit](https://twitter.com/UTVoluntariado/status/1319552214776664071) y en esta nota [¿Es verdad que Amazon u otras empresas tienen o han tenido acceso a la información generada por Radar COVID?](https://github.com/utvoluntariado/radar-covid-docs/blob/prensa/20201022%20%5BEl%20Pais%5D.md) ha tratado de arrojar luz sobre la noticia publicada por El Pais.

**Ricardo Aguilar** (Ricardo Aguilar Twitter @MrBrickerr) escribe este artículo en **Xataka**
[Qué ha pasado con la vulnerabilidad de Radar COVID y el supuesto acceso de Amazon a los datos de los usuarios](https://www.xatakamovil.com/aplicaciones/que-ha-pasado-vulnerabilidad-radar-covid-supuesto-acceso-amazon-a-datos-usuarios/amp) "Amazon tan solo podría conocer de dónde a dónde se están enrutando los datos. Es decir, tener constancia de que alguien se está comunicando con el servidor, pero no quién ni de qué manera."
 

| Estado | Actualización | Fuentes |
| --- | --- | --- |
| Aprobado | 27/10/2020 | Enlace de El Pais y tuits citados |

#### <a name="FAQ-A-5"></a>A.5 Rebaja por consumo de datos en Radar COVID en algunas operadoras.

Las principales operadoras de telefonía,  @movistar_es @vodafone_es @orange_es @o2es @tuenties @Amena se comprometen a no repercutir el consumo de datos de Radar COVID a sus usuarios

[Nota de prensa de La Moncloa](https://www.lamoncloa.gob.es/serviciosdeprensa/notasprensa/asuntos-economicos/Paginas/2020/221020-radarcovid.aspx)

La noticia no indica nada de Pepephone, MasMóvil, Yoigo, Simyo, Lowi y algunas otras

La comunicación, que diariamente se hace varias veces al día (ver B.2) entre el servidor y nuestro móvil, supone al día menos de 100 Kb. de datos (1024 Kb = 1 Mb)

| Estado | Actualización | Fuentes |
| --- | --- | --- |
| Aprobado | 25/10/2020 | [Tuit oficial](https://twitter.com/desdelamoncloa/status/1319716470150946817)|


### <a name="FAQ-B"></a>B. Funcionamiento de Radar COVID

#### <a name="FAQ-B-1"></a>B.1. ¿Se puede instalar Radar COVID después de que me den el resultado positivo en un test?

 Sí, pero los contactos estrechos anteriores a la instalación no recibirán ningún aviso.

[@pvieito](https://twitter.com/pvieito/status/1311026303643062272):

> Recordemos que Radar COVID tiene que estar instalada y activada días antes del diagnóstico para que al compartirlo en la app, haya TEKs (Clave de exposición temporal o identificador generado diariamente en el dispositivo) de días previos que subir al servidor. Si la instalación se hace a posteriori no sirve para avisar a los contactos de riesgo.

| Estado | Actualización | Fuentes |
| --- | --- | --- |
| Aprobado | 03/10/2020 | [Twitter (@pvieito)](https://twitter.com/pvieito/status/1311026303643062272) |

#### <a name="FAQ-B-2"></a>B.2. ¿A qué horas calcula mi móvil las notificaciones si un usuario de un móvil próximo ha comunicado un test positivo?

 La notificación a mi móvil no se produce en cuanto mi contacto ha comunicado su positivo, sino cuando el servidor envía las actualizaciones a los móviles, y eso sucede varias veces al día:

Desde diciembre de 2020 las actualizaciones de los TEK a los móviles, tanto Android como iPhone, se producen varias veces al día, casi siempre entre 4 y 6 veces. Una actualización típica es ésta:

```
Fecha/hora/descarga/TEK descargados
2021-01-22 23:02	937
2021-01-22 19:01	14930
2021-01-22 14:58	974
2021-01-22 09:32	13430
2021-01-22 04:17	146	
2021-01-22 00:16	16211
```
La FAQ "_He tenido contacto con una persona que ha dado positivo ¿cuánto tiempo pasa hasta que recibo la alerta en la aplicación?_" [Radar COVID](https://radarcovid.gob.es/faq-alertas-por-exposicion-la-covid-19) sigue indicando en 30/01/2021:

 - Entre las 6h y las 18h
 - Entre las 18h y las 6h

| Estado | Actualización | Fuentes |
| --- | --- | --- |
| Aprobado | 30/01/2021 | [Twitter (@AppRadarCovid)](https://twitter.com/AppRadarCovid/status/1310517441752182784) |

#### <a name="FAQ-B-3"></a>B.3. Si vivo en una Comunidad Autónoma (CCAA) que no proporciona código para comunicar un positivo ¿puedo recibir notificaciones de contacto alto?

Sí. Si usted ha estado en contacto con una persona que vive en otra CCAA que proporciona códigos a los positivos y esa persona lo ha comunicado recibirá notificaciones de contacto alto.

| Estado | Actualización | Fuentes |
| --- | --- | --- |
| Borrador | | |

#### <a name="FAQ-B-4"></a>B.4. Nuevas versiones de Radar COVID

 En las direcciones de descarga de Google y Apple, en la parte inferior, aparece el número de versión que estamos descargando.

20/12/2020 Android 1.2.0

- Actualización versión DP-3T.
- Vista de Estadísticas Radar COVID.
- Vista de información del estado de la aplicación.
- Recordatorio de apertura de la aplicación.
- Contador confinamiento.
- Compartir enlace para facilitar descarga.
- Añadido idioma Francés.
- Introducción de código desde SMS.
- Mejoras de accesibilidad:
. Aumento de tamaño de texto y contraste.
. Cambio en el estilo de los enlaces.
. Etiquetado de elementos en pantalla.
. Incorporación de encabezados.

Fuente: https://play.google.com/store/apps/details?id=es.gob.radarcovid&hl=es

20/12/2020 iPhone 1.2.0

* Se añade contador informativo de días pendientes de cuarentena para los contactos de riesgo.
* Vista de Estadísticas de Radar COVID.
* Vista de información de la aplicación con información relevante para el chequeo del funcionamiento de la aplicación.
* Se añade recordatorio periódico de apertura de la aplciación.
* Se incorpora idioma Francés.
* Introducción de código desde SMS.
* Incorporación de alerta de BT desactivado.
* Actualización a versión 2.0.0 de DP3T.
* Mejoras de accesibilidad.
* Colectivo con discapacidad visual con resto funcional:
* Aumento del contraste entre texto y fondo.
* Cambio en el estilo de los enlaces.
* Posibilidad de ampliar el tamaño de la fuente adaptándose a la pantalla
* Colectivo con discapacidad visual sin resto funcional:
* Etiquetado de botones.
* Etiquetado de imágenes.
* Etiquetado de enlaces.
* Etiquetado de pestañas.
* Incorporación de encabezados.
* Listado de ítems en el selector de los idiomas.
* Listado de ítems en el selector de las comunidades autónomas.
* Modificación de las casillas del código diagnóstico por un cuadro de texto.
* Creación de botones “Cancelar” o “Cerrar” para facilitar la salida de las pantallas.
* Cambio en el orden de los textos.
* Solución en las casillas de verificación de la pantalla de Privacidad.
* Modificación del nº de pantallas de “Mi diagnóstico”.
* Colectivo con discapacidad auditiva:
* Etiquetado de botones.
* Etiquetado de imágenes.
* Etiquetado de enlaces.
* Etiquetado de pestañas.
* Listado de ítems en el selector de los idiomas.
* Listado de ítems en el selector de las comunidades autónomas.
* Colectivo con discapacidad cognitiva:
* Incorporación del encabezado Radar COVID.
* Cambio del pictograma de “home” por un radar.
* Modificación de literales.
* Etiquetado de las pestañas del menú.
* Bugfixing.

Fuente: https://apps.apple.com/es/app/radar-covid/id1520443509
 
  19/11/2020 iPhone 1.1.2
 
- Preparación de versión para próxima actualización de versión del API de tracing.
- Establecimiento de compartir claves con Europa como opción por defecto.
- Corrección de incidencias.
 
 
 29/10/2020
 
 iPhone 1.1.1, Android 1.1.0
 
 (añadidos en las dos plataformas)
 
- Implementación de funcionalidades para la interoperabilidad con otras aplicaciones europeas.
- Implementación de funcionalidad de cambio de idioma.
- Implementación de funcionalidad de revisión de nuevas políticas de privacidad y/o términos de uso.
- Mejoras de accesibilidad y seguridad.
- Corrección de bugs.

 
 A día 09/10/2020 en Android es 1.0.7 y en iOS 1.0.8:

[@AppRadarCovid](https://twitter.com/AppRadarCovid/status/1314476417946660864):

>  - Habilita la introducción de fecha de inicio de síntomas o de diagnóstico tras hacerte el PCR
>  - Actualiza la versión de #DP3T
>  - Introduce implementaciones en materia de accesibilidad
>  - Resuelve algunos problemas de funcionamiento
>  - La app ahora enviará de forma automática positivos ficticios al servidor
>  - De esa manera, será imposible distinguir qué positivos son reales en caso de ataque
>  - Al comunicar tu positivo nunca nadie podrá saber que fuiste tú

| Estado | Actualización | Fuentes |
| --- | --- | --- |
| Aprobado | 30/10/2020 | [Twitter (@AppRadarCovid)](https://twitter.com/AppRadarCovid/status/1314476417946660864) |

#### <a name="FAQ-B-5"></a> B.5. ¿Qué ocurre a Radar COVID después de que se comunica un diagnóstico positivo?

Al comunicar un positivo, Radar COVID deja de intercambiar identificadores aleatorios con otros móviles porque se asume que se está confinado. [AppRadarCovid lo indica en un tuit](https://twitter.com/AppRadarCovid/status/1317148304711376897).

La app informa de que el [diagnóstico ha sido enviado](resources/b05.jpg) y que Radar COVID ha quedado desactivada. Para reactivarla hay que desinstalar y volverla a instalar.

Esta desactivación se produce incluso cuando se utiliza un código de 12 dígitos ficticio utilizado para las probar la app y que aconsejamos no utilizar. [Códigos ficticios en Radar COVID FAKE_CODE](https://github.com/RadarCOVID/radar-covid-backend-verification-server/commit/2958d3d13203ed2373eb032281ef4d67ab6e3e59)


| Estado | Actualización | Fuentes |
| --- | --- | --- |
| Aprobado | 17/10/2020 | https://twitter.com/AppRadarCovid/status/1317148304711376897 |

### <a name="FAQ-B-6"></a>B.6. Radar COVID ha considerado una exposición pero no la ha catalogado como significativa.

Al entrar en Radar COVID aparece:

_REGISTRO DE EXPOSICIÓN A LA COVID-19 ahora
Actualización semanal
Tu dispositivo ha identificado 6 posibles exposiciones esta semana y las ha compartido con la app Radar COVID_

_Sin contactos de riesgo identificados. Te informaremos de un posible contacto de riesgo._

[Ver Pantalla de Radar COVID exposición sin contacto de riesgo](resources/b6_registros_exposicion.jpg)

Lo que indica esa alerta es que esa semana se han encontrado dos claves de infectados coincidentes con las que tienes almacenadas el teléfono y se han notificado a Radar COVID. Si no le ha saltado la alerta de contagio es porque Radar COVID no ha catalogado la exposición como significativa (es decir, no cumple una exposición acumulada >= 15 minutos a menos de dos metros de distancia en el mismo día).

| Estado | Actualización | Fuentes |
| --- | --- | --- |
| Aprobado | 15/01/2021 | [Twitter 1 de @AppRadarCovid](https://twitter.com/AppRadarCovid/status/1356875757738487809)|
| Aprobado | 15/01/2021 | [Twitter 2 de @AppRadarCovid](https://twitter.com/AppRadarCovid/status/1356875993101852672)|

### <a name="FAQ-C"></a>C. Errores de Radar COVID

#### <a name="FAQ-C-1"></a>C.1. Radar COVID no funciona correctamente en Android: “Ahorro de energía activado. Debes desactivarlo para que Radar COVID funcione correctamente.”

 Solución: Ir a Ajustes > Mantenimiento dispositivo > Batería

 - Modo de Ahorro de Energía. DESACTIVADO
 - Apps sin supervisión / Control de energía de aplicaciones: señalar Radar COVID (estas aplicaciones pueden usar tanta batería como requieran sin que el control de energía lo impida) ([ver captura](/resources/201.jpg)).

| Estado | Actualización | Fuentes |
| --- | --- | --- |
| Aprobado | 05/10/2020 | [Business Insider](https://www.businessinsider.es/configurar-radarcovid-app-rastreo-contactos-no-tan-facil-504213) |

#### <a name="FAQ-C-2"></a>C.2. Radar COVID no funciona correctamente en Android: “Error al cargar nuevos datos de infección”

([ver captura de pantalla](/resources/c2_al_cargar_infeccion.jpg))

Una o varias de estas soluciones han funcionado:

 - a) Desactivar y volver a activar las notificaciones de exposición
 - b) Apagar y encender el teléfono.
 - c) Actualizar Google Play 
 - d) Limpiar la caché de las apps (en Android: Ajustes > Mantenimiento dispositivo > Almacenamiento > Aplicaciones > Radar COVID > Almacenamiento > Borrar Caché)

| Estado | Actualización | Fuentes |
| --- | --- | --- |
| Aprobado | 05/11/2020 | [Twitter (@AppRadarCovid)](https://twitter.com/AppRadarCovid/status/1311959104731189250) |

### <a name="FAQ-C"></a>D. Información sobre Radar STATS

#### <a name="FAQ-D-1"></a>D.1. ¿Qué hace Radar STATS?

Radar STATS es un proyecto desarrollada por @pvieito que publica sus resultados en Twitter en la cuenta [@RadarCOVIDSTATS](https://twitter.com/RadarCOVIDSTATS) cada hora.

Estima cuántos pacientes han comunicado su diagnóstico positivo ("Shared Diagnoses"), cuántos identificadores efímeros -simplificando- intercambiados por móviles se han subido por los que comunicaron positivo ("Uploaded TEKs") y cuál es el porcentaje de los infectados que han comunicado su positivo ("Usage Ratio"). Lo calcula para el último dia y los últimos 14 días tanto en el nivel europeo como en el español.

[Ejemplo](https://twitter.com/RadarCOVIDSTATS/status/1355321567589396486)

```
#RadarCOVID – 2021-01-30@01

Source Countries: 11 🇪🇺

Today (Partial):
- Uploaded TEKs: 106 (+106 last hour)
- Shared Diagnoses: ≤70
- Usage Ratio: ≤0.09%

Last 14 Days:
- Usage Ratio: ≤4.07%
- Usage Ratio (Spain): ≤2.17%

Info: https://github.com/pvieito/Radar-STATS#documentation
```

Radar STATS es un proyecto de código abierto. Contiene un histórico de los datos y documentación sobre el significado de las estadísticas.

Existe una [aplicación para iOS](https://github.com/Radar-STATS/Radar-STATS-iOS) para visualizar las estadísticas de Radar STATS.

| Estado | Actualización | Fuentes |
| --- | --- | --- |
| Aprobado | 30/01/2021 | [Radar STATS](https://github.com/Radar-STATS/Radar-STATS#documentation), [Radar STATS – iOS](https://github.com/Radar-STATS/Radar-STATS-iOS) |


#### <a name="FAQ-D-2"></a>D.2. La interoperabilidad de las aplicaciones europeas y la pérdida de detalle estadístico.

El 28/01/2021 [el servicio de Twitter de @AppRadarCovid](https://radarcovid.gob.es/estadisticas/descargas-radar) ha anunciado los paises que comparten la Interoperabilidad Europea. Un usuario puede recibir alertas de contacto de riesgo con independencia del país en el que esté y la app que use.

El 30/10/2020 Radar COVID ya está conectada al nodo de interoperabilidad de la Comisión Europea según [informa @AppRadarCovid](https://twitter.com/AppRadarCovid/status/1322142080483864577) 

Radar COVID ha integrado sus servidores de positivos (TEK) con algunos paises europeos: Alemania, Italia, Letonia o Irlanda. Si hemos estado cerca de un italiano y este comunica un diagnóstico positivo, nosotros, en España, recibiremos la notificación de Exposición alta"

En las próximas semanas se irán uniendo apps de más países adheridos al nodo de interoperabilidad.

La relación completa de los paises integrados es la [web de la Comisión Europea](https://ec.europa.eu/info/live-work-travel-eu/health/coronavirus-response/travel-during-coronavirus-pandemic/mobile-contact-tracing-apps-eu-member-states_en). 

En esta tabla generada por [@pvieito](https://twitter.com/pvieito) en [@RadarStatsCovid](https://github.com/pvieito/Radar-STATS#documentation) **Multi-Backend Summary Table** calcula el porcentaje de TEK (ver [Glosario](https://utvoluntariado.github.io/radar-covid-docs/#glosario)) del servidor A de un pais (backend A) que están presentes en el servidor B de otro pais (backend B).

> En cuanto activen la integración con la EFGS (eu-federation-gateway-service) el ratio de uso se calculará respecto a la suma de los casos de los países integrados (source countries) pero claro, ya será un ratio de uso agregado para las aplicaciones de la UE, y no concreto o específico de Radar COVID.

Lamentablemente, perdemos las estadísticas de uso a nivel de España que venían siendo publicadas en [@RadarCOVIDSTATS](https://twitter.com/RadarCOVIDSTATS). Ahora esos recuentos se hacen para los paises que se han integrado. El porcentaje de casos que comunicaron su positivo ("Usage ratio") ha subido del 1% de los últimos dias de octubre a más del 4%. [@UTVoluntariado](http://utv.com.es) ha pedido al equipo de desarrollo de Radar COVID que [añada estadísticas](https://github.com/RadarCOVID/radar-covid-backend-dp3t-server/issues/8#issue-734461489), a semejanza de otras aplicaciones europeas, para estimular su uso.

Al comunicar un nuevo positivo en Radar COVID, nos pregunta, tras indicar la fecha de diagnóstico, si queremos "Compartir con personas usuarias de Radar COVID" o "Compartir con personas usuarias de Radar COVID y aplicaciones europeas" [@UTVoluntariado ha pedido que se cambie la respuesta por defecto](https://github.com/RadarCOVID/radar-covid-ios/issues/39#issue-733986441).

| Estado | Actualización | Fuentes |
| --- | --- | --- |
| Aprobado | 07/11/2020 | [Desarrollo de EFGS](https://github.com/eu-federation-gateway-service/efgs-federation-gateway/issues/209)|



### <a name="FAQ-E"></a>E. Información técnica sobre Radar COVID

#### <a name="FAQ-E-1"></a>E.1. ¿Cómo puedo ver el listado de comprobaciones de exposición en Android?

En Android con 8.0.0:

Ajustes > Google > Notificaciones de exposición al COVID-19 > [Comprobaciones de exposición](resources/401a.jpg) ([resultado](resources/401b.jpg) o [detalle de la exposición](resources/401d.jpg)).

En la parte superior derecha de la pantalla, pulsando [Exportar comprobaciones de exposición](resources/401c.jpg) se pueden enviar por correo electrónico a una dirección. Adjuntan un fichero similar a `all-exposure-checks20.json`. Este fichero se puede abrir en cualquier editor de texto.
 
Una "Comprobación de exposición" es similar a:

```
{
    "timestamp": "5 de octubre de 2020 19:36",
    "keyCount": 39,
    "matchesCount": 0,
    "appName": "Radar COVID",
    "hash":"Q+gOQWeHzTSWtsks2JBzV2o8BUfY0nRBXBECi105HfM="
}
```

#### <a name="FAQ-E-2"></a>E.2. ¿Cómo puedo ver el listado de comprobaciones de exposición en iOS?

En iPhone con iOS 13.7:

Ajustes > Notificaciones de exposición > [Activo](resources/402a.png) (pulsar etiqueta) > [Comprobaciones de exposición](resources/402b.png) > Introducir el código del iPhone ([resultado](resources/402c.jpg) o [detalle de la exposición](resources/402d.jpg)).

En la parte inferior la pantalla de Comprobaciones de exposición, pulsando **Exportar comprobaciones de exposición** se pueden enviar por correo electrónico a una dirección. Adjuntan un fichero similar a `all-exposure-checks20.json`. Este fichero se puede abrir en cualquier editor de texto.. Una "Comprobación de exposición" es similar a:

```
"Files" : [
 {
   "Hash" : "F2153E75EBFCDFBED3DA363EB0BECDBD810FEB05E8B691FA1F1FE6858B224208",
   "MatchCount" : 0,
   "KeyCount" : 235,
   "AppBundleIdentifier" : "es.gob.radarcovid",
   "Timestamp" : "2020-10-06 00:40:22 +0200"
 }
]
```

#### <a name="FAQ-E-3"></a>E.3. ¿Qué es una comprobación de exposición?

 Es la comprobación de si alguno de los identificadores aleatorios que mi móvil ha captado de otros móviles cercanos corresponde a alguien que ha comunicado su contagio después de haber estado cerca de mi móvil. Las preguntas E.1 y E.2 muestran cómo puedo ver el listado de **comprobaciones de exposición**. La pregunta E.4 (apartado 2) indica cómo se calculan estas comprobaciones y muestra un ejemplo de comprobaciones tras una descarga de diagnósticos positivos del servidor de diagnósticos positivos. 

| Estado | Actualización | Fuentes |
| --- | --- | --- |
| Borrador | 12/10/2020 |  |

#### <a name="FAQ-E-4"></a>E.4. Funcionamiento técnico de Radar COVID

1. Cada móvil con Radar COVID instalado y Bluetooth activado genera, cada 10 minutos aproximadamente, identificadores aleatorios que se intercambian con otros móviles que están activados y a menos de 2 metros. Cada móvil almacena durante 14 días sus propios identificadores aleatorios y los de los móviles que han estado cerca.

    Hasta donde sabemos, no podemos ver si un móvil cercano nos ha enviado sus identificadores ni ver qué identificadores, propios o de terceros, tenemos almacenados. Por tanto, no podemos saber si nuestros móviles tienen bien instalada Radar Covid y tampoco podemos saber si nuestro vecino, desde una ventana cercana a la nuestra o desde el piso de arriba está intercambiando identificadores con nosotros.

2. Varias veces al día (ver B.2) mi móvil descarga, del servidor de diagnósticos positivos, los identificadores aleatorios que se han subido recientemente a ese servidor por quienes han comunicado su diagnóstico positivo. Mi móvil compara esos identificadores aleatorios con los que he almacenado en dias previos provenientes de otros móviles y si encuentra alguna coincidencia la marca como "matchCount" en las Notificaciones de Exposición (ver preguntas E.1 y E.2). En ese caso mi móvil habrá estado cerca de un positivo y me lo comunicará ("**Riesgo alto. Tu exposición es alta**"). Si no encuentra coincidencia, Radar COVID indicará "**Riesgo bajo. Sin contactos de riesgo identificados**". En el fichero adjunto ([hoja de cálculo](resources/comprobaciones_exposicion.xlsx), [pantallazo](resources/comprobaciones_exposicion.jpg)) se ilustran las **comprobaciones de exposición** que se han generado tras cada descarga.

    Por tanto, si me comunican "Riesgo alto" ninguna autoridad ni ningún servidor me está enviando un mensaje. Es mi propio móvil quien genera las notificaciones, con la información descargada del servidor y los identificadores aleatorios de terceros que mi móvil tenia almacenados.

    Por este motivo, las autoridades no pueden saber cuantas notificaciones de "Riesgo alto" han sido hechas.

3. Cuando un usuario de la aplicación Radar COVID comunica su positivo, los identificadores aleatorios propios que tiene almacenados se cargan en el servidor de diagnósticos positivos que serán descargados por otros usuarios tal como se indica en el apartado 2.

    Cabe indicar que según se indica en la pregunta I.7 de este [documento](https://www.mscbs.gob.es/profesionales/saludPublica/ccayes/alertasActual/nCov/documentos/Preguntas_y_respuestas_RADAR-COVID.pdf) "los identificadores aleatorios generados por ese dispositivo durante los 5 días previos a ese momento se etiquetan como positivos y se lanzan a la nube con consentimiento del usuario". Es decir, no se lanzan a la nube mis identificadores de los 14 días sino algunos menos.

 **NOTA**

- A los identificadores aleatorios se les suele llamar ID aleatorios, ID efímeros o Rolling Proximity Identifier (RPI, Identificador de proximidad móvil).
- Al descargar (como se indica en el apartado 2) realmente no se descargan los identificadores aleatorios sino un identificador diario (TEK, Clave de exposición temporal o Temporary Exposure Key en inglés) a partir de los cuales se calculan los identificadores aleatorios.

| Estado | Actualización | Fuentes |
| --- | --- | --- |
| Borrador | 11/10/2020 | [Ministerio de Salud](https://www.mscbs.gob.es/en/profesionales/saludPublica/ccayes/alertasActual/nCov/documentos/Preguntas_y_respuestas_RADAR-COVID.pdf), [Google Support](https://support.google.com/googleplay/answer/9888358?hl=es), [Radar COVID](https://radarcovid.gob.es/politica-de-privacidad), [Apple](https://covid19-static.cdn-apple.com/applications/covid19/current/static/contact-tracing/pdf/ExposureNotification-CryptographySpecificationv1.2.pdf) |

#### <a name="FAQ-E-5"></a>E.5. Funcionamiento técnico de Radar COVID 2. El servidor de verificación.

Radar COVID utiliza dos servidores: el **servidor de verificación** y el **servidor de diagnósticos positivos** (ver FAQ E.3).

El servidor de verificación valida el código de diagnóstico positivo que han dado las autoridades sanitarias y es introducido por el ciudadano en su móvil. Este servidor verifica el estado del código (si ha sido usado o no lo ha sido, si ha caducado por no haber sido usado durante el período de validez). 

Si el código es correcto el servidor responde con un ticket (en inglés "_certificate issued for temporary exposure keys_") en el que se puede incluir información extra. En esta información pudiera estár incluida el código de CCAA que pudiera servir para ver cuantos códigos de diagnóstico positivo se han [enviado desde cada CCAA](https://radarcovid.gob.es/estadisticas/codigos-introducidos-a-casos-confirmados).

La información técnica puede encontrarse aquí [https://developers.google.com/android/exposure-notifications/verification-system](https://developers.google.com/android/exposure-notifications/verification-system). A continuación se muestra un trozo de esa información. 

```
The epi (epi: el sanitario que comunica el positivo) requests a Verification Code (VC) using the web interface provided by a verification 
server, which generates the VC and sets the time limit for it, and provides it to the epi. 
Optionally, the epi provides details about the diagnosis that will be associated with the requested VC. 
This information is stored by the verification server linked to the issued VC. 
The verification server can later include the diagnosis information in the certificate issued for 
the Temporary Exposure Keys (TEKs) of the corresponding user.
```

| Estado | Actualización | Fuentes |
| --- | --- | --- |
| Aprobado | 15/01/2021 | [https://developers.google.com/android/exposure-notifications/verification-system](https://developers.google.com/android/exposure-notifications/verification-system)|


### <a name="FAQ-F"></a>F. Internacional

#### <a name="FAQ-F-1"></a>F.1. Aplicaciones similares a Radar COVID en otros países

| País | Aplicación | Enlaces Relacionados |
| --- | --- | --- |
| Alemania | [Corona-Warn-App](https://www.coronawarn.app/en/) | [Documentación](https://github.com/corona-warn-app/cwa-documentation/blob/master/README.md), [Arquitectura](https://github.com/corona-warn-app/cwa-documentation/blob/master/solution_architecture.md) |
| Croacia | [Stop-COVID-19](https://github.com/Stop-COVID-19-Croatia) | |
| Italia | [Inmuni](https://www.immuni.italia.it/) | [Estadísticas de uso en español](https://www.immuni.italia.it/dashboard.html) [Preguntas y respuestas en español](https://www.immuni.italia.it/faq.html) |
| Irlanda | [CovidTracker](https://covidtracker.gov.ie/how-the-app-works/) | |
| Letonia | [apturicovid](https://www.apturicovid.lv/) | [FAQ en inglés](https://www.apturicovid.lv/biezak-uzdotie-jautajumi) |
| Portugal | [StayawayCOVID](https://stayawaycovid.pt/funcionamento/) | |
| Suiza | [SwissCovid](https://www.bag.admin.ch/bag/en/home/krankheiten/ausbrueche-epidemien-pandemien/aktuelle-ausbrueche-epidemien/novel-cov/swisscovid-app-und-contact-tracing.html) | [Estadísticas](https://www.experimental.bfs.admin.ch/expstat/en/home/innovative-methods/swisscovid-app-monitoring.html) |

La relación completa de los paises que cuentan con una aplicación de rastreo de contactos es la [web de la Comisión Europea](https://ec.europa.eu/info/live-work-travel-eu/health/coronavirus-response/travel-during-coronavirus-pandemic/mobile-contact-tracing-apps-eu-member-states_en). 

Tambien se puede encontrar pulsando la imagen de cada pais en la página de [Radar COVID](https://radarcovid.gob.es/estadisticas/descargas-radar).

La Comisión Europea informa que ha comenzado a funcionar la [pasarela de interoperabilidad](https://ec.europa.eu/commission/presscorner/detail/es/ip_20_1904). En ese documento se detallan los paises que tienen una [aplicación de contactos](https://ec.europa.eu/info/live-work-travel-eu/health/coronavirus-response/travel-during-coronavirus-pandemic/how-tracing-and-warning-apps-can-help-during-pandemic_en) con descripciones técnicas sobre la protección de datos y cómo aseguran la interoperabilidad. Puede encontrarse más información en D.2.

| Estado | Actualización | Fuentes |
| --- | --- | --- |
| Aprobado | 30/01/2021 | |
| Aprobado | 20/10/2020 | https://ec.europa.eu/commission/presscorner/detail/es/ip_20_1904 |
| Aprobado | 20/10/2020 | https://ec.europa.eu/info/live-work-travel-eu/health/coronavirus-response/travel-during-coronavirus-pandemic/how-tracing-and-warning-apps-can-help-during-pandemic_en |

#### <a name="FAQ-F-2"></a>F.2. Documentación sobre el acuerdo de Google-Apple para intercambio a través de Bluetooth

Documentos técnicos que describen el intercambio de identificadores efímeros entre teléfonos Android e iPhone, intercambio basado en el protocolo DP-3T (Rastreo de proximidad descentralizado para preservar la privacidad):

##### Google
 - [Documento de referencia del diseño de la solución](https://github.com/google/exposure-notifications-android)
 - [Especificación de la emisión de Bluetooth](https://www.blog.google/documents/70/Exposure_Notification_-_Bluetooth_Specification_v1.2.2.pdf)
 - [Especificación de la generación de identificadores](https://blog.google/documents/69/Exposure_Notification_-_Cryptography_Specification_v1.2.1.pdf)
 - [API (librerías) para programar el intercambio](https://developers.google.com/android/exposure-notifications/exposure-notifications-api)
 - [FAQ sobre las notificaciones de exposición](https://www.blog.google/documents/63/Exposure_Notification_-_FAQ_v1.0.pdf)
 - [Formato de los ficheros de exposición](https://developers.google.com/android/exposure-notifications/exposure-key-file-format)

##### Apple

 - [Documento de referencia del diseño de la solución](https://covid19.apple.com/contacttracing)
 - [Especificación de la emisión de Bluetooth](https://covid19-static.cdn-apple.com/applications/covid19/current/static/contact-tracing/pdf/ExposureNotification-BluetoothSpecificationv1.2.pdf)
 - [Especificación de la generación de identificadores](https://covid19-static.cdn-apple.com/applications/covid19/current/static/contact-tracing/pdf/ExposureNotification-CryptographySpecificationv1.2.pdf)
 - [API (librerías) para programar el intercambio](https://developer.apple.com/documentation/exposurenotification)
 - [FAQ sobre las notificaciones de exposición](https://covid19-static.cdn-apple.com/applications/covid19/current/static/contact-tracing/pdf/ExposureNotification-FAQv1.2.pdf)

##### Protocolo DP-3T

 - [Descripción del protocolo](https://github.com/DP-3T/documents/blob/master/DP3T%20-%20Data%20Protection%20and%20Security.pdf)
 - [Documentación](https://github.com/DP-3T/documents/)
 - [Buenas prácticas para la seguridad operacional en el rastreo de proximidad. Equipo DP-3T, Carmela Troncoso](https://github.com/DP-3T/documents/blob/master/DP3T%20-%20Best%20Practices%20for%20Operation%20Security%20in%20Proximity%20Tracing.pdf) 
 - [Visión general de protección de datos y seguridad, Carmela Troncoso y otros](https://github.com/DP-3T/documents/blob/master/DP3T%20-%20Data%20Protection%20and%20Security.pdf)

| Estado | Actualización | Fuentes |
| --- | --- | --- |
| Aprobado | 26/10/2020 | |

#### <a name="FAQ-F-3"></a>F.3. Las aplicaciones de diferentes países ¿son compatibles? ¿Un suizo de vacaciones por España, si da positivo y lo mete en SwissCovid, comunica su positivo a quienes tienen la aplicación española?

Según indica el servicio de soporte de Twitter @AppRadarCovid en este [tuit](https://twitter.com/AppRadarCovid/status/1317050752439812097):

> - Radar COVID se incorpora a las pruebas del marco de interoperabilidad de la Comisión Europea.
> - Las pruebas se extenderán unas tres semanas (a partir del 16/10).
> - Una vez superadas, las apps de los Estados miembros adheridos serán compatibles.

@pvieito intuye, en este [tuit](https://twitter.com/pvieito/status/1317185321428287502), que esas pruebas de interoperabilidad han comenzado.

La Comisión Europea informa que ha comenzado a funcionar la [pasarela de interoperabilidad](https://ec.europa.eu/commission/presscorner/detail/es/ip_20_1904). En ese documento se detallan los paises que tiene una [app de contactos](https://ec.europa.eu/info/live-work-travel-eu/health/coronavirus-response/travel-during-coronavirus-pandemic/how-tracing-and-warning-apps-can-help-during-pandemic_en)

Las app Corona-Warn-App (Alemania) e Immuni (Italia) han sido actualizadas para funcionar con la interoperabilidad europea según se indica en 20/10/2020 [aquí.](https://twitter.com/pvieito/status/1318593010200924160)

Se puede ver en una de las ayudas de iPhone (Ajustes > Notificaciones de exposición > Cómo funcionan las notificaciones de exposición > Más información > Notificaciones de exposición y la privacidad, párrafo 7)

_Aunque puedes autorizar notificaciones de exposición de más de una autoridad de salud pública, solo puedes tener activas las de una región simultáneamente. Recibirás notificaciones de posibles exposiciones conforme a los parámetros establecidos por la autoridad de salud pública de tu región activa. Para seleccionar o cambiar tu región activa, ve a Ajustes > Notificaciones de exposición_


| Estado | Actualización | Fuentes |
| --- | --- | --- |
| Borrador | 17/10/2020 | Twitter indicados, Información en Radar COVID-iPhone |
| Aprobado | 20/10/2020 | https://ec.europa.eu/commission/presscorner/detail/es/ip_20_1904 |
| Aprobado | 20/10/2020 | https://ec.europa.eu/info/live-work-travel-eu/health/coronavirus-response/travel-during-coronavirus-pandemic/how-tracing-and-warning-apps-can-help-during-pandemic_en |


### <a name="FAQ-Z"></a>Z. Implantación en Comunidades Autónomas

#### <a name="FAQ-Z-1"></a>Z.1. Comunidades Autónomas (CCAA) cuyo sistema sanitario proporciona el código de 12 cifras para comunicar un diagnóstico positivo

Las Comunidades Autónomas que han entregado códigos [códigos introducidos por cada comunidad autónoma](https://radarcovid.gob.es/estadisticas/codigos-introducidos-a-casos-confirmados)

Lo siguiente se considera OBSOLETO a partir de 29/01/2021. No se retira por si en algún momento fueran necesarios los datos que se ofrecen.

La siguiente tabla contiene las comunidades que entregan el código necesario (al menos en el 50% de los casos) para comunicar que diagnósticos positivos en Radar COVID:

| Comunidad Autónoma | Activo | Fuente | Fecha de actualización |
| --- | --- | --- | --- |
| Andalucía | Sí | [Xataka Móvil](https://www.xatakamovil.com/aplicaciones/dia-d-para-radar-covid-espana-que-comunidades-autonomas-funciona-app-rastreo-contactos-covid-19) | 03/10/2020 |
| Aragón | Sí | Diversos medios indican informalmente que a partir del 15/10/2020 o del 16 en casi todo Aragón se darán los códigos. | 15/10/2020 |
| Asturias |    |   | 03/10/2020 |
| Baleares | Sí | [Xataka Móvil](https://www.xatakamovil.com/aplicaciones/dia-d-para-radar-covid-espana-que-comunidades-autonomas-funciona-app-rastreo-contactos-covid-19) | 03/10/2020 |
| Canarias | Sí | [Xataka Móvil](https://www.xatakamovil.com/aplicaciones/dia-d-para-radar-covid-espana-que-comunidades-autonomas-funciona-app-rastreo-contactos-covid-19) | 03/10/2020 |
| Cantabria | Sí | [Xataka Móvil](https://www.xatakamovil.com/aplicaciones/dia-d-para-radar-covid-espana-que-comunidades-autonomas-funciona-app-rastreo-contactos-covid-19) | 03/10/2020 |
| Castilla la Mancha |    |   | 03/10/2020 |
| Castilla y León |    |   | 03/10/2020 |
| Cataluña | Sí | [Nota del Canal Salut de la Generalitat de Catalunya](https://canalsalut.gencat.cat/ca/salut-a-z/c/coronavirus-2019-ncov/ciutadania/eines-aplicacions-covid-19/radar-covid/) | 28/10/2020 |
| Ceuta |    |   | 03/10/2020 |
| Comunidad Valenciana |  Si  | [Nota de prensa de la Generalitat Valenciana](https://www.gva.es/es/inicio/area_de_prensa/not_detalle_area_prensa?id=899409) | 29/10/2020 |
| Extremadura | Sí | [Divulgación de Salud Extremadura](https://saludextremadura.ses.es/filescms/web/uploaded_files/Documentos/Infografia%20RADAR-Covid.pdf)  | 05/11/2020 |
| Galicia | Sí | [La Voz de Galicia](https://www.lavozdegalicia.es/noticia/sociedad/2020/09/17/tienes-coronavirus-teclea-tu-movil-codigo-da-sergas-avise-tus-contactos-estrechos/00031600351167433512383.htm) | 18/09/2020 |
| Madrid | Sí | [El Confidencial](https://www.elconfidencial.com/tecnologia/2020-10-08/madrid-radar-covid-aplicacion-rastreo-contactos_2781579/), [El Diario](https://www.eldiario.es/tecnologia/madrid-activa-hoy-app-rastreo-contactos-radar-covid_1_6279298.html) | 09/10/2020 |
| Melilla |    |   | 03/10/2020 |
| Murcia | Sí | [Xataka Móvil](https://www.xatakamovil.com/aplicaciones/dia-d-para-radar-covid-espana-que-comunidades-autonomas-funciona-app-rastreo-contactos-covid-19) | 03/10/2020 |
| Navarra |    |   | 03/10/2020 |
| Pais Vasco | Sí | [El Correo](https://www.elcorreo.com/sociedad/salud/directo-rueda-prensa-20200928153045-nt.html) | 03/10/2020 |
| La Rioja |    |   | 03/10/2020 |

Jordi Perez Colome ofreció datos de uso y alcance en [15/11/2020 en El Pais](https://elpais.com/tecnologia/2020-11-14/el-gran-misterio-de-cuanta-gente-ha-usado-realmente-radar-covid.html)

En este [tuit](https://twitter.com/jordipc/status/1327911487244001280) ofrece un hilo con sus averiguaciones. 

| Estado | Actualización | Fuentes |
| --- | --- | --- |
| Aprobado | 30/01/2021 | --- |

#### <a name="FAQ-Z-2"></a>Z.2. Cómo comunican las Comunidades Autónomas (CCAA) el código de 12 digitos

No es posible indicar con exactitud el modo en que cada Comunidad Autónoma comunica el código para comunicar un positivo en Radar Covid ni cómo lo hacen para cada sistema sanitario. Indicamos a continuación la información que nos consta:

- **Aragón**: A través de saludinforma.es (para quien tiene acceso a ella) o por comunicación del sistema sanitario tras una consulta en la Historia Clínica Electrónica. Ver [saludinforma.es](https://www.saludinforma.es/portalsi/web/salud/radar-covid)
- **Cataluña**: Si tiene una prueba diagnóstica positiva de Covid-19, recibirá un SMS de la herramienta digital ContacteCovid.cat. Desde allí, puede solicitar el código para introducirlo en Radar COVID. [Canal Salut de la Generalitat](https://canalsalut.gencat.cat/ca/salut-a-z/c/coronavirus-2019-ncov/ciutadania/eines-aplicacions-covid-19/radar-covid/).
- **Comunidad Valenciana**: [Obtención del código para la notificación de positivo en la aplicación Radar COVID](https://coronavirusregistro.san.gva.es/sipcovid19/asignacodigo?language=es) 
- **Extremadura**: Cuando una persona con la app descargada y activa es diagnosticada de COVID19, el profesional que le está informando le proporciona un código alfanumérico que, voluntariamente, puede introducir en su aplicación [pregunta si tiene Radar COVID instalado y le dicta el número obtenido por el personal desde la aplicación JARA, que es la que contiene el código]. A partir del momento en que se introduce el código, la aplicación envía un mensaje a las app de todos los dispositivos móviles que estuvieron a menos de 2m durante 15 min o más en los 5 días anteriores. [Servicio Extremeño de Salud](https://saludextremadura.ses.es/web/1698846).
- **Galicia**: Desde la Central de Seguimiento de Contactos, te facilitan un código alfanumérico. [Servizo Galego de Saúde](https://coronavirus.sergas.gal/Contidos/Documents/485/RCOVID-DU-v.01.10-GR-RadarCovid_ES.pdf)
- **Pais Vasco**: En el SMS en el Osakidetza comunica el resultado positivo.

| Estado | Actualización | Fuentes |
| --- | --- | --- |
| Aprobado | 18/11/2020 | --- |

## Enlaces oficiales

- [Radar COVID (radarcovid.gob.es)](https://radarcovid.gob.es/)
   - [Preguntas frecuentes](https://radarcovid.gob.es/preguntas-frecuentes)
   - [Estadísticas](https://radarcovid.gob.es/estadisticas/descargas-radar)
   - [Recursos de comunicación y documentación técnica](https://radarcovid.gob.es/recursos-de-comunicacion)
- [Radar COVID - GitHub - Código abierto](https://github.com/radarcovid)
- [Preguntas y respuestas sobre Radar COVID (www.mscbs.gob.es)](https://www.mscbs.gob.es/en/profesionales/saludPublica/ccayes/alertasActual/nCov/documentos/Preguntas_y_respuestas_RADAR-COVID.pdf)
- [Soporte en Twitter @AppRadarCovid](https://twitter.com/AppRadarCovid/with_replies)

## Glosario

- **BLE** (Bluetooth Low Energy) BLE opera en la banda ISM (bandas de radio industriales, científicas y médicas ) de 2.4 GHz. Sin embargo, a diferencia del Bluetooth clásico, BLE permanece en modo de suspensión constantemente, excepto cuando se inicia una conexión. Proporciona un bajo consumo de energía a un costo considerablemente reducido.
- **CCAA**: Comunidades autónomas españolas
- **DP3T**: Es un protocolo de código abierto desarrollado en respuesta a la pandemia de coronavirus 2019-2020 para facilitar el [rastreo digital de contactos](https://es.wikipedia.org/wiki/Rastreo_de_proximidad_descentralizado_para_preservar_la_privacidad) de los participantes infectados.
- **EFGS** [EU Federation Gateway Service](https://github.com/eu-federation-gateway-service/efgs-federation-gateway). Tiene el objetivo de desarrollar la solución oficial europea para lograr la interoperabilidad de los servidores de diagnósticos, de las aplicaciones de rastreo de contactos, para combatir al COVID-19. 
- **Identificadores aleatorios.** Cadenas de caracteres que se intercambian dos móviles próximos a través de Bluetooth. Se les suele llamar también ID aleatorios, ID aleatorios Bluetooth, ID efímeros o Rolling Proximity Identifier (RPI, Identificador de proximidad móvil. Ver pregunta E.4
- **TAN (Transaction Authorization Number)**: códigos de 12 cifras que da el sistema sanitario de las CCAA y sirve para comunicar un diagnóstico positivo.
- **TEK (Temporary Exposure Key)**: Clave de exposición temporal. Un identificador aleatorio generado diariamente en el dispositivo que utilizan las aplicaciones de exposición como Radar COVID para detectar exposiciones y comunicar diagnósticos positivos.

## Reglas de estilo

- Está página no está sometida a intereses y conveniencias de partidos políticos ni de instituciones de gobierno u otras.
- Está página no cuenta con financiación ni otras limitaciones procedentes de empresas u otros intereses económicos.
- La página quiere estar redactada en un lenguaje claro y pedagógico, sin términos en inglés ni abreviaturas no explicadas.
- Las respuestas deben de tener una fuente de la que se han obtenido (salvo excepciones) y una fecha en la que se han redactado.

## <a name="contacto"></a> Contacto y colaboradores

- Email: <RadarCOVIDvoluntarios@gmail.com>
- [Contribuyen](https://github.com/utvoluntariado/radar-covid-docs/)

## Versión

- Versión: 1.5 
- Fecha actualización: 18/02/2020
- [Histórico de cambios](resources/historia.md)
