##TCK: Prueba Técnica
En la empresa X, dedicada a la realización de chapuzas, se necesita avisar al cliente de la fecha y la hora de comienzo de la obra. Actualmente el aviso lo realiza una operadora, pero esto crea muchos problemas de comunicación, ya que en ocasiones se puede llamar al cliente en un momento en el que se le moleste o que no sea posible contactar antes de la fecha de inicio de la obra.
El departamento comercial, después de estudiar posibles mejoras al sistema actual se ha decidido a modernizar este sistema y utilizar un sistema de comunicación que envíe las notificaciones automáticamente. Con el nuevo sistema se da la posibilidad al cliente de elegir la forma en la que desea recibir la comunicación. En una primera fase sólo se van a enviar comunicaciones a través de Fax y SMS. 
Para realizar el envío de los SMSs y de los faxes se ha contratado una empresa que provee un servicio para el envío de faxes y otro servicio para el envío de SMS. Estos servicios sólo necesitan conocer el destinatario (ej: número de teléfono) y el mensaje que se desea enviar.
Después de analizar varias soluciones, se ha decidido contratar a la empresa Y, que era la que ofrecía la solución más barata posible. La documentación aportada de estos servicios es bastante deficiente.
Después de realizar algunas pruebas sobre los servicios se ha detectado que son un poco “inestables” y fallan en bastantes ocasiones. Por lo que la solución debe tener en cuenta esta inestabilidad, ofrecer una buena operativa y gestión de los errores producidos en los servicios.
Al conocer la propuesta, el departamento de facturación, ha visto con buenos ojos la solución y desea aplicar este sistema de comunicaciones dentro de su proceso de facturación. Por lo tanto, la solución a implementar debe poder utilizarse por cualquiera de las aplicaciones de la empresa.

Dado el volumen actual de incidencias respecto a las comunicaciones, el departamento de soporte ha expuesto la necesidad de almacenar en base de datos las comunicaciones solicitadas y el estado de estas.
Después de analizar el ecosistema de la empresa y sus necesidades, se ha llegado a la conclusión de que es necesario que el módulo de comunicaciones se encuentre separado del resto de aplicaciones de la empresa.
Independientemente de la arquitectura (SOA, Microservicios ...) se ha optado por un un enfoque Restful de los web services.

#Diagrama Arquitectura
Realizar un breve diagrama donde se diseñe una solución. Para este diseño se puede hacer uso de cualquier tipo de tecnología (o combinación de estas) para dar una solución al problema.
Para esta prueba no es relevante conocimientos de powerpoint, photoshop o similares. Realizar el diagrama con la herramienta que seas más ágil, y/o te sientas más cómodo. Un diagrama en un cuaderno o pizarra es suficiente (siempre que se entienda la solución propuesta).
Definición contrato servicios
Definir los endpoints principales del módulo de comunicaciones e indicar qué decisiones se han tomado para conseguir una definición lo más cercana a Restful. Incluir en la documentación cómo quedarían la petición y las posibles respuestas para cada uno de los endpoints definidos.
Implementación Solución
Implementar una parte de la solución propuesta en los puntos anteriores, por ejemplo, uno de los endpoints definidos en el punto anteriores (hay que tener en cuenta que elegir el endpoint más sencillo no va a aportar mucho valor). El propósito de este punto no es terminar con un proyecto completo listo para producción, sino ver el proceso de trabajo y la solución propuesta.
No se debería dedicar más de 2-3h a este apartado. Lo importante es poder analizar la forma de trabajar, de diseñar las clases y de testear. No se tendrá en cuenta que la solución final no funcione o esté incompleta.
Para la integración con los servicios existentes (Fax, SMS) dispones de un dummy para la invocación de los servicios (documento adjunto de Wiremock).
Como el propósito de esta prueba no es la creación del entorno de trabajo, dispones de un documento adjunto describiendo una forma de generar un proyecto base.
Propuesta de Mejoras
Enumera y describe brevemente posibles modificaciones (carencias, mejoras, ampliación de funcionalidad ...) que hayas encontrado durante la realización del ejercicio.
