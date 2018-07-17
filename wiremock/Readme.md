# Prueba Técnica: Wiremock
Para simular los servicios de SMS y Fax que actualmente están disponibles utilizaremos Wiremock (http://wiremock.org), en concreto hemos utilizado la versión 2.1.12
http://repo1.maven.org/maven2/com/github/tomakehurst/wiremock-standalone/2.1.12/wiremock-standalone-2.1.12.jar
## Levantar el servicio simulado
En una carpeta vacía:
1) Copiamos el jar de wiremock
2) En esta misma carpeta, creamos una carpeta mappings y añadimos los siguientes ficheros:
* tck.fax.fail.json
* tck.fax.success.json
* tck.sms.fail.json
* tck.sms.success.json
3) Desde la carpeta donde copiamos el jar del wiremock, ejecutamos el siguiente comando:
	java -jar wiremock-standalone-2.1.12.jar -v --port 9100
