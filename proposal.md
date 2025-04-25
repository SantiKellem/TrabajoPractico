# Propuesta TP DSW

## Grupo
### Integrantes
* 53190 - José Sebastián Alberto Barragán Landriel
* 53210 - Shakir Chaya
* 53187 - Santiago Kellemberger
* 52984 - Nicolás Mazzaglia
* 53116 - Franco Nicolás Sussi

### Repositorios
* [fullstack app](http://hyperlinkToGihubOrGitlab)

## Tema
### Descripción
Sistema de gestión para restaurantes que optimiza la experiencia del cliente y el trabajo del personal. A través de un QR único por mesa, el cliente puede visualizar el menú, realizar su pedido y efectuar el pago desde su dispositivo móvil. El sistema permite además la reserva anticipada de mesas, la recomendación de platos por parte de la cocina y una gestión integral por parte de mozos y administradores.

### Modelo
![imagen del modelo]()

*Nota*: incluir un link con la imagen de un modelo, puede ser modelo de dominio, diagrama de clases, DER. Si lo prefieren pueden utilizar diagramas con [Mermaid](https://mermaid.js.org) en lugar de imágenes.

## Alcance Funcional 

### Alcance Mínimo

Regularidad:
|Req|Detalle|
|:-|:-|
|CRUD simple|1. CRUD Comida<br>2. CRUD Mesa<br>3. CRUD - Usuario (Admin, Mozo, Cocina)<br> 4. CRUD - Novedades<br>5. CRUD - Horarios|
|CRUD dependiente|1. CRUD Reserva {depende de} CRUD Mesa y CRUD Usuario<br>2. CRUD Pedido {depende de} CRUD Mesa y CRUD Comida|
|Listado<br>+<br>detalle| 1. Listado de comida => Listado de las opciones del menu filtrado por tipo de plato o opción bebidas. Muestra IdComida, nombre, descripción (ingredientes), precio, tipo de plato<br> 2. Listado de mesa => Listado de todas las mesas del restaurante filtrado por mesa seleccionada. Muestra idMesa, estado, capacidad|
|CUU/Epic|1. CUU - Preparar Comida<br>2. CUU - Pagar Pedido|


Adicionales para Aprobación
|Req|Detalle|
|:-|:-|
|CRUD |1. CRUD Comida
<br>2. CRUD Mesa
<br>3. CRUD - Usuario 
<br> 4. CRUD - Novedades
<br>5. CRUD - Linea de Pedido
<br>6. CRUD - Histórico de Precios
<br>7. CRUD - Reserva
<br>8. CRUD - Pedido
<br>9. CRUD - Novedades
<br>10. CRUD - Horarios
|
|CUU/Epic| CUU01 - Atender_Reservas
<br> CUU02 - Realizar_Pedido
<br> CUU03 - Preparar_Comida
<br> CUU04 - Pagar_Pedido
<br> CUU05 - Cargar_Pedido |


### Alcance Adicional Voluntario

*Nota*: El Alcance Adicional Voluntario es opcional, pero ayuda a que la funcionalidad del sistema esté completa y será considerado en la nota en función de su complejidad y esfuerzo.

|Req|Detalle|
|:-|:-|
|Listados |1. Listado de reservas => Listado de reservas filtrado por día. Muestra idReserva, horario, cantidad comensales, idMesa, nombreCliente, estado. <br>2. Listado Pedido => Listado de todos los pedidos del día. Muestra idPedido, idMesa, horaInicio. <br>3. Listado Usuario => Listado de todos los usuarios del sistema filtrado por nombre, tipoUsuario. Muestra idUsuario, nombre, apellido, DNI, teléfono, mail.
| 
|CUU/Epic|CUU06 - Modificar_Pedido<br>CUU07 - Agregar_Comida|
|Otros|1. Recomendaciones por día de la cocina. <br>2. Implementación de gestión propia mediante QR code|

