Ejercicio 0
Para cada acción, decidan por dónde viaja y por qué: pedir entrar, aceptar a alguien, mandar un mensaje, preguntar la dirección del túnel.

- Pedir entrar va por HTTP: quien pide todavía no tiene token, así que no puede abrir el WebSocket.
Aceptar va por el WebSocket del anfitrión, que ya está abierto y autenticado.
Los mensajes, por WebSocket: es lo que tiene que llegarle a todos al instante.
La dirección del túnel, por HTTP: es una pregunta con una respuesta, y se hace una vez.