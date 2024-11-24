
# Proyecto Urban Grocers 

SUSANA P�REZ APARICIO/ PROYECTO No.7

PASOS A SEGUIR:

1. Abre el proecto "qa-project-Urban-Grocers-app-es" en PyCharm.
2. Asegurate de que los paquetes "request" y "pytest" est�n descargados y actualizados. De no estar instalados o actualizados, descarga y actualiza los 2 paquetes. 
3. Selecciona el archivo configuration.py para coregir desde ah� la URL por la de un servidor nuevo. 
4. Selecciona el archivo "create_kit_name_kit_test.py" para correr desde ah� el programa
5. En la pesta�a superior en el boton "v" (Flecha). En la barra superior de PyCharm, asegurarse que la lista a la hora de desplegar los elemetos diga "Current File".
6. Has clic en el bot�n de "Play" que est� al lado de "Current File".  

LISTA DE COMPROBACI�N DETALLANDO LAS PRUEBAS AUTOMATIZADAS REALIZADAS AL CORRER EL ARCHIVO "create_name_kit_test".

Lista de comprobaci�n de pruebas ? Description: Prueba 1 El n�mero permitido de caracteres (1): kit_body = { "name": "a"} C�digo de respuesta: 201 El campo "name" del cuerpo de la respuesta coincide con el campo "name" del cuerpo de la solicitud Prueba 2 El n�mero permitido de caracteres (511): kit_body = { "name":"El valor de prueba para esta comprobaci�n ser� inferior a"} C�digo de respuesta: 201 El campo "name" en el cuerpo de la respuesta coincide con el campo "name" en el cuerpo de la solicitud Prueba 3 El n�mero de caracteres es menor que la cantidad permitida (0): kit_body = { "name": "" } C�digo de respuesta: 400 Prueba 4 El n�mero de caracteres es mayor que la cantidad permitida (512): kit_body = { "name":"El valor de prueba para esta comprobaci�n ser� inferior a� } C�digo de respuesta: 400 Prueba 5 Se permiten caracteres especiales: kit_body = { "name": ""?%@"," } C�digo de respuesta: 201 El campo "name" del cuerpo de la respuesta coincide con el campo "name" del cuerpo de la solicitud Prueba 6 Se permiten espacios: kit_body = { "name": " A Aaa " } C�digo de respuesta: 201 El campo "name" del cuerpo de la respuesta coincide con el campo "name" del cuerpo de la solicitud Prueba 7 Se permiten n�meros: kit_body = { "name": "123" } C�digo de respuesta: 201 El campo "name" del cuerpo de la respuesta coincide con el campo "name" del cuerpo de la solicitud Prueba 8 El par�metro no se pasa en la solicitud: kit_body = { } C�digo de respuesta: 400 Prueba 9 Se ha pasado un tipo de par�metro diferente (n�mero): kit_body = { "name": 123 } C�digo de respuesta: 400
