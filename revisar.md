# FAQ a revisar antes de ser publicadas (15/02/2021)

Añadir B.6

#### <a name="FAQ-B-6"></a>B.6. Radar COVID ha considerado una exposición pero no la ha catalogado como significativa 

[Pantalla de Radar COVID exposición sin contacto de riesgo](resources/b6_registros_exposicion.jpg)

Lo que indica esa alerta es que esa semana se han encontrado dos claves de infectados coincidentes con las que tienes almacenadas el teléfono y se han notificado a Radar COVID. Si no le ha saltado la alerta de contagio es porque Radar COVID no ha catalogado la exposición como significativa (es decir, no cumple una exposición acumulada >= 15 minutos a menos de dos metros de distancia en el mismo día).

| Estado | Actualización | Fuentes |
| --- | --- | --- |
| Aprobado | 15/01/2021 | [Twitter 1 de @AppRadarCovid](https://twitter.com/AppRadarCovid/status/1356875757738487809)|
| Aprobado | 15/01/2021 | [Twitter 2 de @AppRadarCovid](https://twitter.com/AppRadarCovid/status/1356875993101852672)|

Añadir E.5

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










