# FAQ a revisar antes de ser publicadas
#### <a name="FAQ-D-2"></a>D.2. La interoperabilidad de las aplicaciones europeas y la pérdida de detalle estadístico.


El 30/10/2020 Radar COVID ya está conectada al nodo de interoperabilidad de la Comisión Europea según [informa @AppRadarCovid](https://twitter.com/AppRadarCovid/status/1322142080483864577) 

Radar COVID ha integrado sus servidores de positivos (TEK) con algunos paises europeos: Alemania, Italia, Letonia o Irlanda. Si hemos estado cerca de un italiano y este comunica un diagnóstico positivo, nosotros, en España, recibiremos la notificación de Exposición alta"

En las próximas semanas se irán uniendo apps de más países adheridos al nodo de interoperabilidad.

La relación completa de los paises integrados es la [web de la Comisión Europea](https://ec.europa.eu/info/live-work-travel-eu/health/coronavirus-response/travel-during-coronavirus-pandemic/mobile-contact-tracing-apps-eu-member-states_en). 

En esta tabla generada por [@pvieito](https://twitter.com/pvieito) en [@RadarStatsCovid](https://github.com/pvieito/Radar-STATS#documentation) **Multi-Backend Summary Table** calcula el porcentaje de TEK (ver (Glosario)[https://utvoluntariado.github.io/radar-covid-docs/#glosario]) del servidor A de un pais (backend A) que están presentes en el servidor B de otro pais (backend B).

> En cuanto activen la integración con la EFGS (eu-federation-gateway-service) el ratio de uso se calculará respecto a la suma de los casos de los países integrados (source countries) pero claro, ya será un ratio de uso agregado para las aplicaciones de la UE, y no concreto o específico de Radar COVID.

Lamentablemente, perdemos las estadísticas de uso a nivel de España que venían siendo publicadas en [@RadarCOVIDSTATS](https://twitter.com/RadarCOVIDSTATS). Ahora esos recuentos se hacen para los paises que se han integrado. El porcentaje de casos que comunicaron su positivo ("Usage ratio") ha subido del 1% de los últimos dias de octubre a más del 4%. [@UTVoluntariado](http://utv.com.es) ha pedido al equipo de desarrollo de Radar COVID que [añada estadísticas](https://github.com/RadarCOVID/radar-covid-backend-dp3t-server/issues/8#issue-734461489), a semejanza de otras aplicaciones europeas, para estimular su uso.

Al comunicar un nuevo positivo en Radar COVID, nos pregunta, tras indicar la fecha de diagnóstico, si queremos "Compartir con personas usuarias de Radar COVID" o "Compartir con personas usuarias de Radar COVID y aplicaciones europeas" [@UTVoluntariado ha pedido que se cambie la respuesta por defecto](https://github.com/RadarCOVID/radar-covid-ios/issues/39#issue-733986441).

Actualizado: 07/11/2020 version 17
Actualizado: 05/11/2020 version 16


