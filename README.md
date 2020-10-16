# Radar COVID – Documentación
 
_Proyecto de la [Unidad Tecnológica de Voluntariado](http://utv.com.es)._
 
## Objeto

Dar respuesta a las consultas que se formulan sobre la app Radar COVID tanto sobre su funcionamiento cómo su arquitectura más técnica. Va dirigida a las personas que no encuentan información oficial suficiente. Responde también a preguntas sobre el proyecto Radar STATS.

## Índice

- [Preguntas Frecuentes](#preguntas-frecuentes)
  * [A. Instalación de Radar COVID](#FAQ-A)
    * [A.1. ¿En qué móviles se puede instalar?](#FAQ-A-1)
    * [A.2. ¿Cónsume mucha batería Radar COVID?](#FAQ-A-2)
    * [A.3. ¿Tiene fallos de seguridad o privacidad Radar COVID?](#FAQ-A-3)
  * [B. Funcionamiento de Radar COVID](#FAQ-B)
    * [B.1. ¿Se puede instalar Radar COVID después de que me den el resultado positivo en un test?](#FAQ-B-1)
    * [B.2. ¿A qué horas calcula mi móvil las notificaciones si un usuario de un móvil próximo ha comunicado un test positivo?](#FAQ-B-2)
    * [B.3. ¿Si vivo en una Comunidad Autónoma (CCAA) que no proporciona código para comunicar un positivo ¿puedo recibir notificaciones de contacto alto?](#FAQ-B-3)
    * [B.4. Nuevas versiones de Radar COVID](#FAQ-B-4)
  * [C. Errores de Radar COVID](#FAQ-C)
    * [C.1. Radar COVID no funciona correctamente en Android: “Ahorro de energía activado. Debes desactivarlo para que Radar COVID funcione correctamente.”](#FAQ-C-1)
    * [C.2. Radar COVID no funciona correctamente en Android: “Error al cargar nuevos datos de infección”](#FAQ-C-2)
  * [D. Información sobre Radar STATS](#FAQ-D)
    * [D.1. ¿Qué hace Radar STATS?](#FAQ-D-1)
  * [E. Información técnica sobre Radar COVID](#FAQ-E)
     * [E.1. ¿Cómo puedo ver el listado de comprobaciones de exposición en Android?](#FAQ-E-1)
     * [E.2. ¿Cómo puedo ver el listado de comprobaciones de exposición en iOS?](#FAQ-E-2)
     * [E.3. ¿Qué es una comprobación de exposición?](#FAQ-E-2)
     * [E.4. Funcionamiento técnico de Radar COVID](#FAQ-E-2)
  * [F. Internacional](#FAQ-F)
    * [F.1. Aplicaciones similares a Radar COVID en otros países](#FAQ-F-1)
    * [F.2. Documentación sobre el acuerdo de Google-Apple para intercambio a través de Bluetooth](#FAQ-F-2)
    * [F.3. Las aplicaciones de diferentes países ¿son compatibles? ¿Un suizo de vacaciones por España, si da positivo y lo mete en SwissCovid, comunica su positivo a quienes tienen la aplicación española?](#FAQ-F-3)
  * [Z. Implantación en Comunidades Autónomas](#FAQ-Z)
- [Enlaces Oficiales](#enlaces-oficiales)
- [Glosario](#glosario)
- [Reglas de Estilo](#reglas-de-estilo)
- [Contacto y colaboradores](#contacto)
- [Versión](#versión)

## Preguntas Frecuentes

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

| Estado | Actualización | Fuentes |
| --- | --- | --- |
| Aprobado | 03/10/2020 | [Twitter (@YoryoBass)](https://twitter.com/YoryoBass/status/1312445670922489857) |

#### <a name="FAQ-A-3"></a>A.3. ¿Tiene fallos de seguridad o privacidad Radar COVID?

Parece que no tiene fallos de seguridad o privacidad. Diversos expertos han examinado el código y no consta que haya resquicios de seguridad. Como ejemplo incluimos un informe de la [Organización de Consumidores y Usuarios](https://www.ocu.org/tecnologia/telefono/noticias/radar-covid#) transmitido por la agencia [Europa Press](https://www.europapress.es/asturias/noticia-ocu-confirma-aplicacion-radar-covid-no-registra-datos-personales-segura-20201007124451.html).

Ha suscitado dudas que en Android obliga a tener activada la localización o ubicación. En este [enlace de Xataka](https://www.xataka.com/aplicaciones/que-radar-covid-no-funciona-gps-activo-android-hace-iphone) se indica que Android necesita tener los servicios de localización activos para que funcione la conexión de móviles por Bluetooth pero que Radar COVID no registra esta ubicación. En este [enlace del soporte de Google](https://support.google.com/googleplay/answer/9888358?hl=es) se indica que con Android 11 "no es necesario activar los ajustes de ubicación".

| Estado | Actualización | Fuentes |
| --- | --- | --- |
| Aprobado | 08/10/2020 | [OCU](https://www.ocu.org/tecnologia/telefono/noticias/radar-covid#), [Europa Press](https://www.europapress.es/asturias/noticia-ocu-confirma-aplicacion-radar-covid-no-registra-datos-personales-segura-20201007124451.html), [Xataka](https://www.xataka.com/aplicaciones/que-radar-covid-no-funciona-gps-activo-android-hace-iphone) |

### <a name="FAQ-B"></a>B. Funcionamiento de Radar COVID

#### <a name="FAQ-B-1"></a>B.1. ¿Se puede instalar Radar COVID después de que me den el resultado positivo en un test?

 Sí, pero los contactos estrechos anteriores a la instalación no recibirán ningún aviso.

[@pvieito](https://twitter.com/pvieito/status/1311026303643062272):

> Recordemos que Radar COVID tiene que estar instalada y activada días antes del diagnóstico para que al compartirlo en la app, haya TEKs (Clave de exposición temporal o identificador generado diariamente en el dispositivo) de días previos que subir al servidor. Si la instalación se hace a posteriori no sirve para avisar a los contactos de riesgo.

| Estado | Actualización | Fuentes |
| --- | --- | --- |
| Aprobado | 03/10/2020 | [Twitter (@pvieito)](https://twitter.com/pvieito/status/1311026303643062272) |

#### <a name="FAQ-B-2"></a>B.2. ¿A qué horas calcula mi móvil las notificaciones si un usuario de un móvil próximo ha comunicado un test positivo?

 La notificación a mi móvil no se produce en cuanto mi contacto ha comunicado su positivo, sino cuando el servidor envía las actualizaciones a los móviles, y eso sucede dos veces al día:

 - Entre las 6h y las 18h
 - Entre las 18h y las 6h

| Estado | Actualización | Fuentes |
| --- | --- | --- |
| Aprobado | 16/10/2020 | [Twitter (@AppRadarCovid)](https://twitter.com/AppRadarCovid/status/1310517441752182784) |

#### <a name="FAQ-B-3"></a>B.3. Si vivo en una Comunidad Autónoma (CCAA) que no proporciona código para comunicar un positivo ¿puedo recibir notificaciones de contacto alto?

Sí. Si usted ha estado en contacto con una persona que vive en otra CCAA que proporciona códigos a los positivos y esa persona lo ha comunicado recibirá notificaciones de contacto alto.

| Estado | Actualización | Fuentes |
| --- | --- | --- |
| Borrador | | |

#### <a name="FAQ-B-4"></a>B.4. Nuevas versiones de Radar COVID

 En las direcciones de descarga de Google y Apple, en la parte inferior, aparece el número de versión que estamos descargando.

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
| Aprobado | 09/10/2020 | [Twitter (@AppRadarCovid)](https://twitter.com/AppRadarCovid/status/1314476417946660864) |

### <a name="FAQ-C"></a>C. Errores de Radar COVID

#### <a name="FAQ-C-1"></a>C.1. Radar COVID no funciona correctamente en Android: “Ahorro de energía activado. Debes desactivarlo para que Radar COVID funcione correctamente.”

 Solución: Ir a Ajustes > Mantenimiento dispositivo > Batería

 - Modo de Ahorro de Energía. DESACTIVADO
 - Apps sin supervisión / Control de energía de aplicaciones: señalar Radar COVID (estas aplicaciones pueden usar tanta batería como requieran sin que el control de energía lo impida) ([ver captura](/resources/201.jpg)).

| Estado | Actualización | Fuentes |
| --- | --- | --- |
| Aprobado | 05/10/2020 | [Business Insider](https://www.businessinsider.es/configurar-radarcovid-app-rastreo-contactos-no-tan-facil-504213) |

#### <a name="FAQ-C-2"></a>C.2. Radar COVID no funciona correctamente en Android: “Error al cargar nuevos datos de infección”

 Una o varias de estas soluciones han funcionado:

 a) Desactivar y volver a activar las notificaciones de exposición
 b) Apagar y encender el teléfono.
 c) Actualizar Google Play 
 d) Limpiar la caché de las apps (en Android: Ajustes > Mantenimiento dispositivo > Almacenamiento > Aplicaciones > Radar COVID > Almacenamiento > Borrar Caché)

| Estado | Actualización | Fuentes |
| --- | --- | --- |
| Aprobado | 06/10/2020 | [Twitter (@AppRadarCovid)](https://twitter.com/AppRadarCovid/status/1311959104731189250) |

### <a name="FAQ-C"></a>D. Información sobre Radar STATS

#### <a name="FAQ-D-1"></a>D.1. ¿Qué hace Radar STATS?

Radar STATS es un proyecto desarrollada por @pvieito que publica sus resultados en Twitter en la cuenta [@RadarCOVIDSTATS](https://twitter.com/RadarCOVIDSTATS) cada hora.

Estima cuántos pacientes han comunicado su diagnóstico positivo ("Shared Diagnoses"), cuántos identificadores efímeros -simplificando- intercambiados por móviles se han subido por los que comunicaron positivo ("Uploaded TEKs") y cuál es el porcentaje de los infectados que han comunicado su positivo ("Usage Ratio"). Lo calcula para el último dia y los últimos 7 días.

Radar STATS es un proyecto de código abierto. Contiene un histórico de los datos y documentación sobre el significado de las estadísticas.

Existe una [aplicación para iOS](https://github.com/Radar-STATS/Radar-STATS-iOS) para visualizar las estadísticas de Radar STATS.

| Estado | Actualización | Fuentes |
| --- | --- | --- |
| Aprobado | 08/10/2020 | [Radar STATS](https://github.com/Radar-STATS/Radar-STATS#documentation), [Radar STATS – iOS](https://github.com/Radar-STATS/Radar-STATS-iOS) |

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

#### <a name="FAQ-E-1"></a>E.2. ¿Cómo puedo ver el listado de comprobaciones de exposición en iOS?

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

1. Cada móvil con Radar Covid instalado y Bluetooth activado genera, cada 10 minutos aproximadamente, identificadores aleatorios que se intercambian con otros móviles que están activados y a menos de 2 metros. Cada móvil almacena durante 14 días sus propios identificadores aleatorios y los de los móviles que han estado cerca.

    Hasta donde sabemos, no podemos ver si un móvil cercano nos ha enviado sus identificadores ni ver qué identificadores, propios o de terceros, tenemos almacenados. Por tanto, no podemos saber si nuestros móviles tienen bien instalada Radar Covid y tampoco podemos saber si nuestro vecino, desde una ventana cercana a la nuestra o desde el piso de arriba está intercambiando identificadores con nosotros.

 2. Dos veces al día mi móvil descarga, del servidor de diagnósticos positivos, los identificadores aleatorios que se han subido recientemente a ese servidor por quienes han comunicado su diagnóstico positivo. Mi móvil compara esos identificadores aleatorios con los que he almacenado en dias previos provenientes de otros móviles y si encuentra alguna coincidencia la marca como "matchCount" en las Notificaciones de Exposición (ver preguntas 401 y 402). En ese caso mi móvil habrá estado cerca de un positivo y me lo comunicará ("**Riesgo alto. Tu exposición es alta**"). Si no encuentra coincidencia, Radar Covid indicará "**Riesgo bajo. Sin contactos de riesgo identificados**". En el fichero adjunto ([hoja de cálculo](resources/comprobaciones_exposicion.xlsx), [pantallazo](resources/comprobaciones_exposicion.jpg)) se ilustran las **comprobaciones de exposición** que se han generado tras cada descarga.

    Por tanto, si me comunican "Riesgo alto" ninguna autoridad ni ningún servidor me está enviando un mensaje. Es mi propio móvil quien genera las notificaciones, con la información descargada del servidor y los identificadores aleatorios de terceros que mi móvil tenia almacenados.

    Por este motivo, las autoridades no pueden saber cuantas notificaciones de "Riesgo alto" han sido hechas.

 3. Cuando un usuario de la APP Radar Covid comunica su positivo, los identificadores aleatorios propios que tiene almacenados se cargan en el servidor de diagnósticos positivos que serán descargados por otros usuarios tal como se indica en el apartado 2.

    Cabe indicar que según se indica en la pregunta I.7 de este [documento](https://www.mscbs.gob.es/profesionales/saludPublica/ccayes/alertasActual/nCov/documentos/Preguntas_y_respuestas_RADAR-COVID.pdf) "los identificadores aleatorios generados por ese dispositivo durante los 5 días previos a ese momento se etiquetan como positivos y se lanzan a la nube con consentimiento del usuario". Es decir, no se lanzan a la nube mis identificadores de los 14 días sino algunos menos.

 **NOTA**

- A los identificadores aleatorios se les suele llamar ID aleatorios, ID efímeros o Rolling Proximity Identifier (RPI, Identificador de proximidad móvil).
- Al descargar (como se indica en el apartado 2) realmente no se descargan los identificadores aleatorios sino un identificador diario (TEK, Clave de exposición temporal o Temporary Exposure Key en inglés) a partir de los cuales se calculan los identificadores aleatorios.

| Estado | Actualización | Fuentes |
| --- | --- | --- |
| Borrador | 11/10/2020 | [Ministerio de Salud](https://www.mscbs.gob.es/en/profesionales/saludPublica/ccayes/alertasActual/nCov/documentos/Preguntas_y_respuestas_RADAR-COVID.pdf), [Google Support](https://support.google.com/googleplay/answer/9888358?hl=es), [Radar COVID](https://radarcovid.gob.es/politica-de-privacidad), [Apple](https://covid19-static.cdn-apple.com/applications/covid19/current/static/contact-tracing/pdf/ExposureNotification-CryptographySpecificationv1.2.pdf) |

### <a name="FAQ-F"></a>F. Internacional

#### <a name="FAQ-F-1"></a>F.1. Aplicaciones similares a Radar COVID en otros países

| País | Aplicación | Enlaces Relacionados |
| --- | --- | --- |
| Alemania | [Corona-Warn-App](https://www.coronawarn.app/en/) | [Documentación](https://github.com/corona-warn-app/cwa-documentation/blob/master/README.md), [Arquitectura](https://github.com/corona-warn-app/cwa-documentation/blob/master/solution_architecture.md) |
| Suiza | [SwissCovid](https://www.bag.admin.ch/bag/en/home/krankheiten/ausbrueche-epidemien-pandemien/aktuelle-ausbrueche-epidemien/novel-cov/swisscovid-app-und-contact-tracing.html) | [Estadísticas](https://www.experimental.bfs.admin.ch/expstat/en/home/innovative-methods/swisscovid-app-monitoring.html) |
| Irlanda | [CovidTracker](https://covidtracker.gov.ie/how-the-app-works/) | |
| Portugal | [StayawayCOVID](https://stayawaycovid.pt/funcionamento/) | |

| Estado | Actualización | Fuentes |
| --- | --- | --- |
| Aprobado | 09/10/2020 | |

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

| Estado | Actualización | Fuentes |
| --- | --- | --- |
| Aprobado | 09/10/2020 | |

#### <a name="FAQ-F-3"></a>F.3. Las aplicaciones de diferentes países ¿son compatibles? ¿Un suizo de vacaciones por España, si da positivo y lo mete en SwissCovid, comunica su positivo a quienes tienen la aplicación española?

[@YoryoBass](https://twitter.com/YoryoBass/status/1314242987367563264):

> La implementación europea ya está en curso y, hasta donde yo se, existe un “turno” para que cada país se integre. Se está trabajando en ello a nivel europeo. Mientras tanto la única solución es usar las apps de cada país.

| Estado | Actualización | Fuentes |
| --- | --- | --- |
| Borrador | 08/10/2020 | [Twitter (@YoryoBass)](https://twitter.com/YoryoBass/status/1314242987367563264) |

### <a name="FAQ-Z"></a>Z. Implantación en Comunidades Autónomas

#### <a name="FAQ-Z-1"></a>Z.1. Comunidades Autónomas (CCAA) cuyo sistema sanitario proporciona el código de 12 cifras para comunicar un diagnóstico positivo

La siguiente tabla contiene las comunidades que entregan el código necesario (al menos en el 50% de los casos) para comunicar que diagnósticos positivos en Radar COVID:

| Comunidad Autónoma | Activo | Fuente | Fecha de actualización |
| --- | --- | --- | --- |
| Andalucía | Sí | [Xataka Móvil](https://www.xatakamovil.com/aplicaciones/dia-d-para-radar-covid-espana-que-comunidades-autonomas-funciona-app-rastreo-contactos-covid-19) | 03/10/2020 |
| Aragón | Sí | [Heraldo](https://www.heraldo.es/noticias/aragon/2020/09/04/aragon-app-aplicacion-radar-covid-provincia-zaragoza-huesca-teruel-1393869.html) | 15/10/2020 |
| Asturias |    |   | 03/10/2020 |
| Baleares | Sí | [Xataka Móvil](https://www.xatakamovil.com/aplicaciones/dia-d-para-radar-covid-espana-que-comunidades-autonomas-funciona-app-rastreo-contactos-covid-19) | 03/10/2020 |
| Canarias | Sí | [Xataka Móvil](https://www.xatakamovil.com/aplicaciones/dia-d-para-radar-covid-espana-que-comunidades-autonomas-funciona-app-rastreo-contactos-covid-19) | 03/10/2020 |
| Cantabria | Sí | [Xataka Móvil](https://www.xatakamovil.com/aplicaciones/dia-d-para-radar-covid-espana-que-comunidades-autonomas-funciona-app-rastreo-contactos-covid-19) | 03/10/2020 |
| Castilla la Mancha |    |   | 03/10/2020 |
| Castilla y León |    |   | 03/10/2020 |
| Cataluña | No | [Hipertextual](https://hipertextual.com/2020/10/app-radar-covid-madrid-barcelona-no-operativa-pese-numero-contagios) | 05/10/2020 |
| Ceuta |    |   | 03/10/2020 |
| Comunidad Valenciana |    |   | 03/10/2020 |
| Extremadura |    |   | 03/10/2020 |
| Galicia | Sí | [La Voz de Galicia](https://www.lavozdegalicia.es/noticia/sociedad/2020/09/17/tienes-coronavirus-teclea-tu-movil-codigo-da-sergas-avise-tus-contactos-estrechos/00031600351167433512383.htm) | 18/09/2020 |
| Madrid | Sí | [El Confidencial](https://www.elconfidencial.com/tecnologia/2020-10-08/madrid-radar-covid-aplicacion-rastreo-contactos_2781579/), [El Diario](https://www.eldiario.es/tecnologia/madrid-activa-hoy-app-rastreo-contactos-radar-covid_1_6279298.html) | 09/10/2020 |
| Melilla |    |   | 03/10/2020 |
| Murcia | Sí | [Xataka Móvil](https://www.xatakamovil.com/aplicaciones/dia-d-para-radar-covid-espana-que-comunidades-autonomas-funciona-app-rastreo-contactos-covid-19) | 03/10/2020 |
| Navarra |    |   | 03/10/2020 |
| Pais Vasco | Sí | [El Correo](https://www.elcorreo.com/sociedad/salud/directo-rueda-prensa-20200928153045-nt.html) | 03/10/2020 |
| La Rioja |    |   | 03/10/2020 |

## Enlaces Oficiales

- [Radar COVID radarcovid.gob.es](https://radarcovid.gob.es/preguntas-frecuentes)
- [Radar COVID - GitHub - Código abierto](https://github.com/radarcovid)
- [Preguntas y respuestas sobre Radar COVID www.mscbs.gob.es](https://www.mscbs.gob.es/en/profesionales/saludPublica/ccayes/alertasActual/nCov/documentos/Preguntas_y_respuestas_RADAR-COVID.pdf)

## Glosario

- **CCAA**: Comunidades autónomas españolas
- **DP3T**: Es un protocolo de código abierto desarrollado en respuesta a la pandemia de coronavirus 2019-2020 para facilitar el [rastreo digital de contactos](https://es.wikipedia.org/wiki/Rastreo_de_proximidad_descentralizado_para_preservar_la_privacidad) de los participantes infectados.
- **TAN (Transaction Authorization Number)**: códigos de 12 cifras que da el sistema sanitario de las CCAA y sirve para comunicar un diagnóstico positivo.
- **TEK (Temporary Exposure Key)**: Clave de exposición temporal. Un identificador aleatorio generado diariamente en el dispositivo que utilizan las aplicaciones de exposición como Radar COVID para detectar exposiciones y comunicar diagnósticos positivos.

## Reglas de Estilo

- Está página no está sometida a intereses y conveniencias de partidos políticos ni de instituciones de gobierno u otras.
- Está página no cuenta con financiación ni otras limitaciones procedentes de empresas u otros intereses económicos.
- La página quiere estar redactada en un lenguaje claro y pedagógico, sin términos en inglés ni abreviaturas no explicadas.
- Las respuestas deben de tener una fuente de la que se han obtenido (salvo excepciones) y una fecha en la que se han redactado.

## <a name="contacto"></a> Contacto y colaboradores

- email: RadarCOVIDvoluntarios@gmail.com
- [Contribuyen](https://github.com/utvoluntariado/radar-covid-docs/)


## Versión

- Versión: 0.901 (version beta, de prueba; en 23/10/2020 será definitiva)
- Fecha actualización: 16/10/2020
