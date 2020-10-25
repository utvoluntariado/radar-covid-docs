# FAQ a revisar antes de ser publicadas

#### <a name="FAQ-A-5"></a>A.5 Rebaja por consumo de datos en RadarCovid en algunas operadoras.

NUEVO

Las principales operadoras de telefonía,  @movistar_es @vodafone_es @orange_es @o2es @tuenties @Amena se comprometen a no repercutir el consumo de datos de #RadarCOVID a sus usuarios

[Nota de prensa de La Moncloa](https://www.lamoncloa.gob.es/serviciosdeprensa/notasprensa/asuntos-economicos/Paginas/2020/221020-radarcovid.aspx)

La noticia no indica nada de Pepephone, MasMóvil, Yoigo, Simyo, Lowi y algunas otras

La comunicación, que diariamente se hace dos veces entre el servidor y nuestro móvil, supone al día menos de 100 Kb. de datos (1000 Kb = 1 Mb)


| Estado | Actualización | Fuentes |
| --- | --- | --- |
| Aprobado | 25/10/2020 | [Tuit oficial](https://twitter.com/desdelamoncloa/status/1319716470150946817)|

#### <a name="FAQ-F-2"></a>F.2. Documentación sobre el acuerdo de Google-Apple para intercambio a través de Bluetooth.

MODIFICAR. Añadir a Protocolo DP-3T

[Buenas prácticas para la seguridad operacional en el rastreo de proximidad. Equipo DP-3T, Carmela Troncoso](https://github.com/DP-3T/documents/blob/master/DP3T%20-%20Best%20Practices%20for%20Operation%20Security%20in%20Proximity%20Tracing.pdf) 

[Visión general de protección de datos y seguridad, Carmela Troncoso y otros](https://github.com/DP-3T/documents/blob/master/DP3T%20-%20Data%20Protection%20and%20Security.pdf)


#### <a name="FAQ-A-2"></a>A.2. ¿Cónsume mucha batería Radar COVID?.

MODIFICAR. Añadir 

Hemos hecho el siguiente experimento. De su naturaleza no pueden obtenerse conclusiones pero puede dar indicios.

Hemos tomado una Galaxy S7 Edge con Android 8.0 Durante 24 horas no ha hecho ni recibido llamadas. Ha tenido conexión Internet (whatsapp, twitter y mail) Ha estado en la calle 90 minutos. Tiene Radar Covid instalada. Y hemos hecho dos pruebas durante 24 horas cada una: a) con Bluetooth y Ubicación activadas y b) con Bluetooth y Ubicación desactivadas.

a) La batería ha pasado de una carga del 100% a una carga del 80%
b) La batería ha pasado de una carga del 100% a una carga del 80% (coincide con a)


#### <a name="FAQ-D-2"></a>D.2. La interoperabilidad de las APP europeas y la pérdida de detalle estadístico.

NUEV0

La interoperabilidad de las aplicaciones de rastreo europeas que se anuncia que estará disponible en la semana del 26/10/2020 [tuit de la EU](https://twitter.com/EU_Commission/status/1318152800887558144) inicialmente perderá el dato del uso de Radar COVID en España ("Usage Ratio" y otros indicadores que calcula @pvieito para dar cada hora la estadística en [RadarCovidStats](https://twitter.com/radarcovidstats).

En cuanto activen la integración con la EFGS (eu-federation-gateway-service) el ratio de uso se calculará respecto a la suma de los casos de los países integrados (source countries) pero claro, ya será un ratio de uso agregado para las aplicaciones de la UE, y no concreto o específico de Radar COVID.

@pvieito ha pedido al equipo de desarrollo de la integración europea que EFGS proporcione algún modo de obtener los [TEK de cada pais](https://github.com/eu-federation-gateway-service/efgs-federation-gateway/issues/209) para poder monitorizar el rendimiento de cada uno.

| Estado | Actualización | Fuentes |
| --- | --- | --- |
| Aprobado | 25/10/2020 | [Desarrollo de EFGS](https://github.com/eu-federation-gateway-service/efgs-federation-gateway/issues/209)|



Actualizado: 25/10/2020 version 14


