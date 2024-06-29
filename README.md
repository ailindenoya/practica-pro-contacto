# practica-pro-contacto


Ejercicio 2. 
1. ¿Qué es un servidor HTTP?
Un servidor HTTP se utiliza para procesar una aplicación del lado del servidor. Se realizan conexiones con el cliente otorgando o pidiendo una respuesta (response/request).
2. ¿Qué son los verbos HTTP? Mencionar los más conocidos
Los verbos HTTP son un conjunto de caracteres que se utilizan en el protocolo para indicar acciones. Los más conocidos son
GET: para consultas
POST: para crear información nueva en el servidor y para cualquier operación con efecto que no esté cubierta por PUT, PATCH o DELETE
PUT: para actualizar por completo
PATCH: para actualizar parcialmente
DELETE: para eliminar información del servidor
3. ¿Qué es un request y un response en una comunicación HTTP? ¿Qué son los headers?
Un request o pedido es un mensaje que envia el cliente al servidor con el fin de realizar un acción. Un response o respuesta es, en contraparte, un mensaje que envia el servidor al cliente como respuesta a un pedido. Por otro lado, un header o encabezado HTTP es información que se intercambia entre un navegador y un sitio web al ingresar en él. 
4. ¿Qué es un queryString? (En el contexto de una url)
Un queryString es un término que se utiliza para referenciar una interacción con una base de datos. El queryString forma parte de la URL y contiene los datos que se enviarán a las aplicaciones web.
5. ¿Qué es el responseCode? ¿Qué significado tiene los posibles valores devueltos?
Los responseCode o codigos de estado de respuesta nos permiten saber si un request o pedido se completó o no de manera satisfactoria.
Hay estados informativos (100–199), estados de éxito (200–299), estados de redirección (300–399), estados de error del cliente (400–499) y estados de error del servidor (500–599).
6. ¿Cómo se envía la data en un Get y cómo en un POST?
En un pedido GET, los datos se envían como parámetros que se agregan a la URL luego del símbolo "?". Cada parámetro se especifica de la forma "clave=valor". Si queremos enviar más de uno, los diferenciamos con un "&".
En un POST, los datos se envían en el cuerpo de la solicitud HTTP y su estructura dependerá del lenguaje de programación que se utilice. Por otro lado, existen herramientas como Postman, que nos simplifican esta codificación.
7. ¿Qué verbo http utiliza el navegador cuando accedemos a una página?
El verbo GET se utiliza para obtener la página y sus recursos asociados.
8. Explicar brevemente qué son las estructuras de datos JSON y XML dando ejemplo de estructuras posibles.
JSON o JavaScript Object Notation es un formato de texto que se utiliza para intercambiar datos. Es independiente a cualquier lenguaje de programación.
Un ejemplo puede ser:
{
  "animal": "Gato",
  "nombre": "Luli",
  "sexo": "Hembra"
  "comidasFavoritas":  [
    {
      "id": 1,
      "comida": "Carne",
    },
    {
      "id": 2,
      "comida": "Atún",
    },
    {
      "id": 3,
      "comida": "Sobrecito",
    }
  ]
}
XML o Extensible Markup Language es un metalenguaje que permite definir datos mediante el uso de reglas. No puede realizar operaciones de cómputo por si mismo.
Un ejemplo puede ser:
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






