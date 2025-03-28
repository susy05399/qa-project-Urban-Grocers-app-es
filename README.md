
# Proyecto Urban Grocers 

*Datos del creador:*

- Nombre: Susana Pérez Aparicio
- perezapariciosusana@gmail.com
- Mexico city

PASOS A SEGUIR:

1. Abre el proecto "qa-project-Urban-Grocers-app-es" en PyCharm.
2. Asegurate de que los paquetes "request" y "pytest" estén descargados y actualizados. De no estar instalados o actualizados, descarga y actualiza los 2 paquetes. 
3. Selecciona el archivo configuration.py para coregir desde ahí la URL por la de un servidor nuevo. 
4. Selecciona el archivo "create_kit_name_kit_test.py" para correr desde ahí el programa
5. En la pestaña superior en el boton "v" (Flecha). En la barra superior de PyCharm, asegurarse que la lista a la hora de desplegar los elemetos diga "Current File".
6. Has clic en el botón de "Play" que está al lado de "Current File".  

LISTA DE COMPROBACIÓN DETALLANDO LAS PRUEBAS AUTOMATIZADAS REALIZADAS AL CORRER EL ARCHIVO "create_name_kit_test".

Lista de comprobación de pruebas ? Description: Prueba 1 El número permitido de caracteres (1): kit_body = { "name": "a"} Código de respuesta: 201 El campo "name" del cuerpo de la respuesta coincide con el campo "name" del cuerpo de la solicitud Prueba 2 El número permitido de caracteres (511): kit_body = { "name":"El valor de prueba para esta comprobación será inferior a"} Código de respuesta: 201 El campo "name" en el cuerpo de la respuesta coincide con el campo "name" en el cuerpo de la solicitud Prueba 3 El número de caracteres es menor que la cantidad permitida (0): kit_body = { "name": "" } Código de respuesta: 400 Prueba 4 El número de caracteres es mayor que la cantidad permitida (512): kit_body = { "name":"El valor de prueba para esta comprobación será inferior a” } Código de respuesta: 400 Prueba 5 Se permiten caracteres especiales: kit_body = { "name": ""?%@"," } Código de respuesta: 201 El campo "name" del cuerpo de la respuesta coincide con el campo "name" del cuerpo de la solicitud Prueba 6 Se permiten espacios: kit_body = { "name": " A Aaa " } Código de respuesta: 201 El campo "name" del cuerpo de la respuesta coincide con el campo "name" del cuerpo de la solicitud Prueba 7 Se permiten números: kit_body = { "name": "123" } Código de respuesta: 201 El campo "name" del cuerpo de la respuesta coincide con el campo "name" del cuerpo de la solicitud Prueba 8 El parámetro no se pasa en la solicitud: kit_body = { } Código de respuesta: 400 Prueba 9 Se ha pasado un tipo de parámetro diferente (número): kit_body = { "name": 123 } Código de respuesta: 400
