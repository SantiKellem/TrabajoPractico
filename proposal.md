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
Sistema de gestión para restaurantes que optimiza la experiencia del comensal y el trabajo del personal. A través de un QR único por mesa, el comensal puede visualizar el menú, realizar su pedido y efectuar el pago desde su dispositivo móvil. El sistema permite además la reserva, la recomendación de platos por parte de la cocina y una gestión integral por parte de mozos y administradores.

### Modelo
[Ver diagrama](https://drive.google.com/file/d/1pa-LWP9kE9zRg4e_uUt9t6BNZLI03Qqm/view?usp=drive_link)


## Alcance Funcional 

### Alcance Mínimo

Regularidad:
| Req         | Detalle |
|:------------|:--------|
|CRUD simple|1. CRUD Producto<br>2. CRUD Mesa<br>3. CRUD Usuario (Cliente, Admin, Mozo, Cocina)<br> 4. CRUD Novedades<br>5. CRUD Horarios|
|CRUD dependiente|1. CRUD Reserva {depende de} CRUD Mesa y CRUD Usuario<br>2. CRUD Sugerencias {depende de} CRUD Productos|
|Listado<br>+<br>detalle| 1. Listado de productos => Listado de las opciones del menu filtrado por comida o bebida. Muestra nombre, descripción, precio, tipo de plato y especificaciones<br> 2. Listado de mozos => Listado de todos los mozos que trabajan en el restaurante, pudiendo buscar por nombre. Muestra nombre de usuario, nombre,	apellido y telefono|
|CUU/Epic|1. CUU01 Registrar Asistencia<br>2. CUU02 Realizar Pedido|


### Adicionales para Aprobación

| Req | Detalle |
|:----|:---------|
| CRUD | 1. CRUD Producto<br>2. CRUD Mesa<br>3. CRUD Usuario (Cliente, Mozo, Administrador, Cocina)<br>4. CRUD Línea de Pedido<br>5. CRUD Precio (Histórico de precios)<br>6. CRUD Reserva<br>7. CRUD Pedido<br>8. CRUD Pago<br>9. CRUD Horario<br>10. CRUD Sugerencia<br>11. CRUD Políticas del Restaurante<br>12. CRUD Novedad<br>13. CRUD Estado Cliente<br>14. CRUD Información del Restaurante|
| CUU/Epic | 1. CUU03 Preparar Comidas<br>2. CUU04 Cobrar Pedido<br>3. CUU05 Cargar Pedido<br>4. CUU08 Realizar Reserva<br>5. CUU09 Cancelar Reserva<br>6. CUU10 Registrar Mozo<br>7. CUU11 Registrar Cliente<br>8. CUU12 Iniciar Sesión<br>9. CUU13 Registrar Horario<br>10. CUU14 Modificar Horario<br>11. CUU15 Registrar Novedad<br>12. CUU16 Modificar Novedad<br>13. CUU17 Registrar Mesa<br>14. CUU18 Registrar Producto<br>15. CUU19 Modificar Producto<br>16. CUU20 Registrar Sugerencia<br>17. CUU21 Modificar Sugerencia<br>18. CUU22 Eliminar Mozo<br>19. CUU23 Modificar Información<br>20. CUU24 Modificar Datos de Usuario<br>21. CUU25 Modificar Políticas<br>22. CUU26 Registrar Precio<br>23. CUU27 Eliminar Precio<br>24. CUU28 Eliminar Mesa<br>25. CUU29 Modificar Mesa |


### Alcance Adicional Voluntario

| Req       | Detalle |
|:----------|:--------|
| Listados  | 1. Historial de reservas => Listado de reservas realizadas por un cliente. Muestra fecha reserva, fecha cancelación, horario, cantidad comensales, estado.<br>2. Listado de novedades activas => Listado de todas las novedades activas en un rango de fechas. Muestra titulo, descripcion, fecha desde, fecha hasta.<br>3. Listado con pedido activo => listado con las mesas que tienen un pedido a cargo de un mozo. Muestra numero de mesa, estado del pedido. |
| CUU/Epic  | 1. CUU06 Modificar Pedido<br>2. CUU07 Registrar Modificación |
| Otros     | 1. Implementación de gestión propia mediante código QR.<br>2. Realización, modificación y seguimiento de un pedido activo en tiempo real mediante WebSockets |

