
# Practica para ProContacto

## Ejercicio 2. 

**🖥️ 1. ¿Qué es un servidor HTTP?**

Un servidor HTTP se utiliza para procesar una aplicación del lado del servidor. Se realizan conexiones con el cliente otorgando o pidiendo una respuesta (response/request).

**📜 2. ¿Qué son los verbos HTTP? Mencionar los más conocidos**

Los verbos HTTP son un conjunto de caracteres que se utilizan en el protocolo para indicar acciones. Los más conocidos son:
- GET: para consultas
- POST: para crear información nueva en el servidor y para cualquier operación con efecto que no esté cubierta por PUT, PATCH o DELETE
- PUT: para actualizar por completo
- PATCH: para actualizar parcialmente
- DELETE: para eliminar información del servidor

**📩 3. ¿Qué es un request y un response en una comunicación HTTP? ¿Qué son los headers?** 

Un request o pedido es un mensaje que envía el cliente al servidor con el fin de realizar una acción. Un response o respuesta es, en contraparte, un mensaje que envía el servidor al cliente como respuesta a un pedido. Por otro lado, un header o encabezado HTTP es información que se intercambia entre un navegador y un sitio web al ingresar en él. 

**🔍 4. ¿Qué es un queryString? (En el contexto de una URL)**

Un queryString es un término que se utiliza para referenciar una interacción con una base de datos. El queryString forma parte de la URL y contiene los datos que se enviarán a las aplicaciones web.

**🔢 5. ¿Qué es el responseCode? ¿Qué significado tienen los posibles valores devueltos?**

Los responseCode o códigos de estado de respuesta nos permiten saber si un request o pedido se completó o no de manera satisfactoria.
Hay estados informativos (100–199), estados de éxito (200–299), estados de redirección (300–399), estados de error del cliente (400–499) y estados de error del servidor (500–599).

**📨 6. ¿Cómo se envía la data en un GET y cómo en un POST?**

En un pedido GET, los datos se envían como parámetros que se agregan a la URL luego del símbolo "?". Cada parámetro se especifica de la forma "clave=valor". Si queremos enviar más de uno, los diferenciamos con un "&".
En un POST, los datos se envían en el cuerpo de la solicitud HTTP y su estructura dependerá del lenguaje de programación que se utilice. Por otro lado, existen herramientas como Postman, que nos simplifican esta codificación.

**🌐 7. ¿Qué verbo HTTP utiliza el navegador cuando accedemos a una página?**

El verbo GET se utiliza para obtener la página y sus recursos asociados.

**📊 8. Explicar brevemente qué son las estructuras de datos JSON y XML dando ejemplo de estructuras posibles.**

JSON o JavaScript Object Notation es un formato de texto que se utiliza para intercambiar datos. Es independiente a cualquier lenguaje de programación.

Un ejemplo puede ser:
```json
{
  "animal": "Gato",
  "nombre": "Luli",
  "sexo": "Hembra",
  "comidasFavoritas": [
    {
      "id": 1,
      "comida": "Carne"
    },
    {
      "id": 2,
      "comida": "Atún"
    },
    {
      "id": 3,
      "comida": "Sobrecito"
    }
  ]
}

```

XML o Extensible Markup Language es un metalenguaje que permite definir datos mediante el uso de reglas. No puede realizar operaciones de cómputo por si mismo.

Un ejemplo puede ser:

```<XML>
<michis>
  <michi>
    <id>1</id>
    <nombre>Luli</nombre>
  </michi>
  <michi>
    <id>2</id>
    <nombre>Chuchi</nombre>
  </michi>
  <michi>
    <id>3</id>
    <nombre>Chulin</nombre>
  </michi>
</michis>

```
**🔗 9. Explicar brevemente el estándar SOAP**

Simple Object Access Protocol es un protocolo de comunicación basado en XML que permite interoperar de manera fluida entre sistemas heterogéneos. Tiene una definición clara y estandar para el formato de mensajes, además de poder incluir metadatos en los mismos. También puede ser transportado a través de varios protocolos subyacentes. SOAP permite invocar de forma remota funciones en sistemas distribuidos y esta conformado por mecanismos de seguridad que asegura integridad y confidencialidad de los datos.

**🔆 10. Explicar brevemente el estándar REST Full**

Una API es un conjunto de funciones y procedimientos que pueden ser usadas por un software. Una API web es una especie de puerta de enlace entre los clientes y los recursos de la web. REST (Representational State Transfer) es una arquitectura de software que impone condiciones sobre cómo debe funcionar una API. Se puede utilizar este tipo de arquitecturas para comunicaciones confiables y de alto rendimiento. Las API que siguen el estilo arquitectónico de REST se llaman API REST y, API RESTful alude a las API web RESTful.

**💭 11. ¿Qué son los headers en un request? ¿Para qué se utiliza el key Content-type en un header?**

Los headers o encabezados HTTP contienen metadata en pares clave-valor. Se pueden utilizar para definir comportamiento manejo de caché, estado de sesiones y facilitar la autenticación. Estos permiten una comunicación mas efectiva entre cliente y servidor. El header Content-Type identifica el tipo de medio de cualquier recurso en el cuerpo del request. Dicha información permite que el servidor lo interprete y procese de manera correcta.

## Ejercicio 3.

Hago GET: 
![alt text](https://i.postimg.cc/bvMYSpQn/pro-con.png)

Hago POST: 
![alt text](https://i.postimg.cc/Gh9MqRYt/pro-con2.png)

Hago GET nuevamente para ver que se haya hecho el POST de manera correcta: 

![alt text](https://i.postimg.cc/dtX5ffmB/pro-con3.png)

¿Qué diferencias se observan entre las llamadas el punto 1 y 3?
Mi POST (mi email y mi nombre) fueron agregados al listado de emails y nombres que obtuve en el primer GET.


## Ejercicio 4.

[Hacer click aquí para ver mi perfil](https://www.salesforce.com/trailblazer/ailindenoya)


## Ejercicio 5.

**📈 1. Lead**

Los Leads representan nuevos clientes u oportunidades de venta. Su fuente puede ser la web, una lista, entre otros. Contienen la información básica que necesita el equipo para hacer seguimiento al negocio. 

**🏢 3. Account**

Los Accounts son las compañías con las que se negocia. Por lo general se encuentran en el centro de las relaciones entre objetos.

**👤 5. Contact**

Los Contacts son las personas con las que se contacta el equipo. Pueden provenir de Leads o de otras fuentes y son una buena forma de rastrear información individual para hacer crecer estas relaciones. 

**💼 7. Opportunity**

Las Opportunities son los tratos en los que se encuentra trabajando el equipo y éste mismo validó como útiles para la organización. Permiten hacer seguimiento a tiempo real de información importante.

**📦 9. Product**

Los Products son ítems o servicios que una compañía vende a sus clientes. Pueden ser utilizados en Objects, Opportunities, Quotes, Orders y Contracts. Pueden tener distintas jerarquías, condiciones y atributos.

**💰 11. PriceBook**

Los Products se listan en los PriceBooks con sus respectivos precios.

**📝 13. Quote**

Los Quotes son documentos formales que permiten al cliente conocer información sobre el producto o servicio en el que esté interesado.

**🔧 15. Asset**

Los Assets son registros que representan productos o servicios comprados por un cliente. Sirven para hacer un rastreo postventa, tal como garantías, mantenimiento y soporte.  

**🆘 17. Case**

Los Cases son registros útiles para la gestión de consultas de clientes, issues, o solicitudes de soporte. Son muy importantes para resolver cualquier problema que pueda ocurrir con algún cliente.

**📚 19. Article**

Los Articles son parte de la base de conocimiento de Salesforce (Salesforce Knowledge base), y proveen información, soluciones, y buenas prácticas tanto para usuarios como para clientes.


![alt text](https://i.postimg.cc/cLdwtsd6/pro-con4.png) 

*Nota*: Para las relaciones representé las que existen por default según el Schema Builder. Lead no parecía tener relación con alguno de los ítems relacionados. Por otro lado, investigué sobre Articles, y al ser un elemento que es gestionado por una base de datos interna de Salesforce, ésta no aparece en el Schema Builder. Sin embargo, podemos decir que este elemento puede tener una relación de muchos a muchos con cada uno de los demás elementos, ya que un artículo puede tratar sobre muchos elementos, y viceversa.

## Ejercicio 6.

### Soluciones de Salesforce

**❓ A. ¿Qué es Salesforce?**

Es una empresa que ofrece software basado en la nube con el objetivo de que las organizaciones puedan tener una gestión rápida, fácil y segura. Cuenta flexibilidad, escalabilidad y un extenso ecosistema de aplicaciones que amplían sus funcionalidades principales a través de AppExchange.

**☁️ B. ¿Qué es Sales Cloud?**

Sales Cloud es un producto que ofrece Salesforce diseñado para la gestión y optimización de los procesos de venta de las organizaciones. Ayuda a las empresas a aumentar la productividad de sus equipos comerciales, mejorar la eficiencia operativa y optimizar el ciclo de ventas desde la captación de leads hasta el cierre de negocios. 

**❄️ C. ¿Qué es Service Cloud?**

Service Cloud es un servicio de atención al cliente basado en la nube ofrecido por Salesforce. Aprovecha el potencial de CRM (Customer Relationship Management) para brindar diferentes servicios de asistencia multicanal.

**💊 D. ¿Qué es Health Cloud?**

Health Cloud es una solución CRM ofrecida por Salesforce para el sector de la salud que permite una interacción mejor con los pacientes desde cualquier dispositivo. Permite una colaboración más efectiva entre proveedores de salud, pacientes y equipos médicos.

**💫 E. ¿Qué es Marketing Cloud?**

Salesforce Marketing Cloud provee software y servicios de análisis y automatización de marketing digital. Está diseñada para facilitar la creación, ejecución y análisis de campañas de marketing multicanal.


### Funcionalidades de Salesforce

**📋 A. ¿Qué es un RecordType?**

Un RecordType es un tipo de registro que permite personalizar la presentación y el comportamiento de los registros según las necesidades específicas de la organización. Es una manera de definir conjuntos distintos de campos, page layouts (diseños de página) y picklist values (valores de listas desplegables) que se aplican a un objeto estándar o personalizado.

**📚 B. ¿Qué es un ReportType?**

Un ReportType es un tipo de reporte es un conjunto predefinido de objetos y relaciones que determina qué datos se pueden incluir en un informe y cómo se organizan y muestran esos datos. Es un esquema que define la estructura y las relaciones entre los datos que se pueden seleccionar y mostrar en un informe.

**📖 C. ¿Qué es un Page Layout?**

Un Page Layout define la organización y visibilidad de los campos, secciones, y otros elementos en la interfaz de usuario para un objeto específico. Determina cómo se presentan y se ordenan los datos cuando los usuarios ven o editan registros de ese objeto.

**📃 D. ¿Qué es un Compact Layout?**

Un Compact Layout es una configuración de diseño que proporciona una vista rápida y accesible de información importante sin necesidad de abrir el registro completo. 

**👑 E. ¿Qué es un Perfil?**

Un Perfil es un conjunto de permisos y diferentes configuraciones que sirven para determinar qué acciones y funciones puede realizar un usuario en la plataforma. Son fundamentales para gestionar y controlar el acceso y las capacidades de los usuarios en la plataforma.

**💬 F. ¿Qué es un Rol?**

Un Rol define la jerarquía de acceso y visibilidad. Se utilizan en conjunto con los perfiles para determinar quién puede ver y editar registros. También sirven para establecer la seguridad y el acceso en diferentes niveles dentro de la estructura organizativa. 

**✔️ G. ¿Qué es un Validation Rule?**

Un Validation Rule es una regla lógica que se utiliza para asegurar que los datos ingresados por usuarios cumplan con diversos criterios antes de almacenarlos en la base de datos. Sirven para mantener la integridad y consistencia de los datos en Salesforce, asegurando que los registros cumplan con los estándares propios de cada organización.
**H. ¿Qué diferencia hay entre una relación Master Detail y Lookup?**
La relación Lookup vincula dos objetos para poder "buscar" un objeto en los elementos relacionados del otro objeto. Por otro lado, en las relaciones Master Detail, un objeto es el principal y otro es el detalle: en este tipo de relaciones, el objeto principal controla determinados comportamientos del objeto de detalle.

**⛳ I. ¿Qué es un Sandbox?**

Un Sandbox es una copia del sistema u organización que se desarrolló en Salesforce que se utiliza para el desarrollo y pruebas. Este no afecta la instancia de producción principal.

**👥 J. ¿Qué es un ChangeSet?**

Un ChangeSet es una herramienta que se utiliza para agrupar y migrar configuraciones personalizadas entre un Sandbox y el entorno de producción. 

**🧙🏻‍♂️ K. ¿Para qué sirve el import Wizard de Salesforce?**

El import Wizard de Salesforce sirve para la importación masiva de datos desde fuentes externas a la organización. Es útil para grandes cantidades de registros como cuentas, contactos, oportunidades u otros objetos estándar y personalizados.

**📱 L. ¿Para qué sirve la funcionalidad Web to Lead?**

La funcionalidad Web to Lead permite capturar de manera automática información de Leads desde el propio sitio web de la organización y convertirla en registros de Salesforce.

**🎫 M. ¿Para qué sirve la funcionalidad Web to Case?**

La funcionalidad Web to Case permite recolectar solicitudes de soporte de los clientes desde el propio sitio web de la organización y generar cases de Salesforce.

**📺 N. ¿Para qué sirve la funcionalidad Omnichannel?**

La funcionalidad Omnichannel utiliza reglas de enrutamiento y priorización configurables para dirigir automáticamente interacciones entrantes al agente más adecuado según la disponibilidad, habilidades y cargas de trabajo actuales.

**📢 O. ¿Para qué sirve la funcionalidad Chatter?**

La funcionalidad Chatter habilita a que los usuarios colaboren en Opportunities, Cases, campañas y proyectos con aplicaciones incrustadas y acciones personalizadas. Proporciona un flujo de noticias personalizado donde los usuarios pueden publicar actualizaciones, compartir archivos, mencionar a otros usuarios y comentar en publicaciones, tal como si se tratase de una red social. 


### Conceptos generales

**⛈ A. ¿Qué significa SaaS?**

Software As A Service es un modelo para distribuir software. El soporte y los datos son gestionados en servidores de un proveedor al que se accede a través de internet. El proveedor proporciona tanto el hardware como el software. 

**❔ B. ¿Salesforce es Saas?**

Salesforce es un SaaS ya que se distribuye a través de internet y está disponible para los usuarios a través de un navegador web sin necesidad de contar con más que acceso a internet.

**💭 C. ¿Qué significa que una solución sea Cloud?**

Una solución Cloud es aquella que tiene por objetivo almacenar los datos de una organización a través de un proveedor. Este tipo de soluciones permite acceso remoto a softwares, almacenamiento de archivos y procesamiento de datos por medio de Internet.

**🏙️ D. ¿Qué significa que una solución sea On-Premise?**

Una solución On-Premise refiere a cualquier solución que instale y opere software en los servidores y equipos de una organización. 

**🌫️ E. ¿Qué es un pipeline de ventas?**

Un pipeline de ventas es un flujo de trabajo secuencial que sigue una organización para convertir prospectos en clientes mediante ventas. Representa visual y conceptualmente todas las etapas que atraviesa un prospecto desde que muestra interés inicial hasta que realiza una compra.

**🔽 F. ¿Qué es un funnel de ventas?**

Un funnel de ventas, también conocido como "embudo de ventas" está centrado en el filtrado y clasificación de prospectos a medida que avanzan a través de las diferentes etapas del proceso de ventas.

**👨‍💼 G. ¿Qué significa Customer Experience?**

Customer Experience es la impresión que se llevan los clientes de la imágen de una organización a lo largo de todos los puntos del ciclo del comprador. 

**🗺️ H. ¿Qué significa omnicanalidad?**

Igual a la pregunta H. La omnicanalidad implica que los clientes puedan interactuar con una organización a través de diversos canales de manera fluida y consistente, sin importar por dónde elijan hacerlo.

**💼 I. ¿Qué significa que un negocio sea B2B? ¿Qué significa que un negocio sea B2C? ¿Qué es un KPI?**

Un modelo de negocio B2B (Business-To-Business) refiere a transacciones comerciales donde una empresa vende productos, servicios o soluciones a otra empresa. Por otro lado, un model B2C (Business-To-Consumer) implica la venta directa a consumidores individuales.
Un KPI es una métrica métrica utilizada para ayudar a gestionar un servicio de IT, proceso, plan de proyecto o actividad. Pueden utilizarse muchas métricas, pero solo las más importantes se definen como KPIs y se utilizan para gestionar e informar sobre un
proceso, servicio de IT o actividad.

**🛠️ J. ¿Qué es una API y en qué se diferencia de una Rest API?**

Una API (Application Programming Interface) es un conjunto de reglas y definiciones que permite que diferentes aplicaciones se comuniquen entre sí. Una REST API (Representational State Transfer API) es un tipo específico de API que sigue los principios del estilo arquitectónico REST. Este está basado en HTTP, los recursos se representan a través de URLs y es stateless (cada request HTTP contiene toda la información necesaria para ser procesada y no se mantiene estado de sesión).

**🗂️ K. ¿Qué es un Proceso Batch?**

Un proceso batch es la ejecución automatizada y programada de tareas que se realizan en lotes o conjuntos. Es muy útil para manejar grandes volúmenes de datos o realizar operaciones que requieren tiempo y recursos significativos.

**🌱 L. ¿Qué es Kanban?**

Kanban permite gestionar el trabajo y optimizar los procesos de manera eficiente y visual. Cuenta con tableros y tarjetas para planificar con claridad. Además cuenta con un enfoque "pull" que consiste en que las tarjetas se muevan de una columna a la siguiente a medida que se avanza en el trabajo

**🤝 M. ¿Qué es un ERP?**

Un ERP (Enterprise Resource Planning) es un sistema integrado de gestión empresarial diseñado para ayudar a las organizaciones a manejar y automatizar sus procesos centrales. Permite la integración de varias funciones comerciales, como la planificación de recursos humanos, contabilidad, inventario, gestión de pedidos, compras y más, en un sistema unificado.

**❗ N. ¿Salesforce es un ERP?**

Salesforce no es un ERP. Sin embargo, ofrece varias soluciones comerciales que se pueden integrar para mejorar y respaldar un ERP. Tiene capacidades extendidas a través de su ecosistema de aplicaciones y servicios, y su enfoque principal está en la gestión de ventas, marketing y servicio al cliente.

## Ejercicio 7.

Instalamos e iniciamos Data Loader.
![alt text](https://i.postimg.cc/2SPwnh6T/Capture1.png) 

Una vez logueados, hacemos click en insert.

![alt text](https://i.postimg.cc/SKCGdRY4/Capture4.png) 

Importamos el archivo del módulo 4, y siguiendo las mismas instrucciones que en ese ejercicio, selecciono contacto.

![alt text](https://i.postimg.cc/L56BmVC4/Capture5.png) 

Dejo estos campos de la manera en que estaban.

![alt text](https://i.postimg.cc/QC4gCWwQ/Capture6.png) 

Hago el mapeo de cada uno de los campos, tal como se especificaba en dicho módulo.

![alt text](https://i.postimg.cc/fLvf4Pvg/Capture7.png) 

Elegimos la carpeta de destino. 

![alt text](https://i.postimg.cc/ydKybK0Z/Capture8.png)

La operación se concretó correctamente.

![alt text](https://i.postimg.cc/44BQBryY/Capture9.png)

Observamos los resultados de lo que se insertó.



