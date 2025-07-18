# Propuesta TP DSW

## Grupo
### Integrantes
* 53190 - José Sebastián Alberto Barragán Landriel
* 53210 - Shakir Chaya
* 53187 - Santiago Kellemberger
* 52984 - Nicolás Mazzaglia
* 53116 - Franco Nicolás Sussi

### Repositorios
* [fullstack app](https://github.com/ShakirChaya0/Fullstack-app)

## Tema
### Descripción
Sistema de gestión para restaurantes que optimiza la experiencia del cliente y el trabajo del personal. A través de un QR único por mesa, el cliente puede visualizar el menú, realizar su pedido y efectuar el pago desde su dispositivo móvil. El sistema permite además la reserva anticipada de mesas, la recomendación de platos por parte de la cocina y una gestión integral por parte de mozos y administradores.

### Modelo
[Ver diagrama en Draw.io](https://drive.google.com/file/d/13MFX2FGwSIfcKgfaU-S0YrmG_0Gn1tV4/view?usp=sharing)


## Alcance Funcional 

### Alcance Mínimo

Regularidad:
| Req         | Detalle |
|:------------|:--------|
|CRUD simple|1. CRUD Comida<br>2. CRUD Mesa<br>3. CRUD - Usuario (Admin, Mozo, Cocina)<br> 4. CRUD - Novedades<br>5. CRUD - Horarios|
|CRUD dependiente|1. CRUD Reserva {depende de} CRUD Mesa y CRUD Usuario<br>2. CRUD Pedido {depende de} CRUD Mesa y CRUD Comida|
|Listado<br>+<br>detalle| 1. Listado de comida => Listado de las opciones del menu filtrado por tipo de plato o opción bebidas. Muestra IdComida, nombre, descripción (ingredientes), precio, tipo de plato<br> 2. Listado de mesa => Listado de todas las mesas del restaurante filtrado por mesa seleccionada. Muestra idMesa, estado, capacidad|
|CUU/Epic|1. CUU - Preparar Comida<br>2. CUU - Pagar Pedido|


Adicionales para Aprobación
| Req         | Detalle |
|:------------|:--------|
| CRUD        | 1. CRUD Producto<br>2. CRUD Mesa<br>3. CRUD - Usuario<br>4. CRUD - Línea de Pedido<br>5. CRUD - Histórico de Precios<br>6. CRUD - Reserva<br>7. CRUD - Pedido<br>8. CRUD - Horarios<br>9. CRUD - Sugerencias<br>10. CRUD - Políticas del Restaurante<br>11. CRUD - Pagos<br>12. CRUD - Novedades |
| CUU/Epic    | 1. CUU01 - Atender_Reservas<br>2. CUU02 - Realizar_Pedido<br>3. CUU03 - Preparar_Comida<br>4. CUU04 - Pagar_Pedido<br>5. CUU05 - Cargar_Pedido |


### Alcance Adicional Voluntario

| Req       | Detalle |
|:----------|:--------|
| Listados  | 1. Listado de reservas => Listado de reservas filtrado por día. Muestra idReserva, horario, cantidad comensales, idMesa, nombreCliente, estado.<br>2. Listado de pedidos => Listado de todos los pedidos del día. Muestra idPedido, idMesa, horaInicio.<br>3. Listado de usuarios => Listado de todos los usuarios del sistema filtrado por nombre y tipoUsuario. Muestra idUsuario, nombre, apellido, DNI, teléfono, mail. |
| CUU/Epic  | 1. CUU06 - Modificar_Pedido<br>2. CUU07 - Agregar_Comida |
| Otros     | 1. Recomendaciones por día de la cocina.<br>2. Implementación de gestión propia mediante QR code |

