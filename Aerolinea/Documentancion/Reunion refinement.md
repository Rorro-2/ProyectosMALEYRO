# Reunión de Refinement — Sprint 1 — Comisión 7

**Proyecto:** Sky Link — Sistema integral web + app móvil para pasajeros
**Sprint:** 1
**Fecha:** 09/10/2026
**Objetivo:** revisar y consolidar la **versión final de la descripción de las Historias de Usuario (US)** del Sprint 1, partiendo de las descripciones entregadas en el Sprint 0 y aplicando los cambios surgidos durante el Sprint 1 (decisiones del cliente, criterios técnicos y hallazgos de la demo).

**Participantes:**
- Mier Mazini, Emanuel Sebastian
- Lauret, Matias Javier
- Giordano, Nicolás
- Koch, Valentina
- Martin, Álvaro Nicolás
- Simos, Candela
- Orellano, Rocío
- Robaina, Malena Rubí
- Galan Marcelli, Diego Ezequiel
- Junca, Matías Javier

---

## 1. Motivo del refinement

En el Sprint 0 se entregó una primera descripción de las US según el entendimiento inicial del equipo. Durante el Sprint 1 ese entendimiento cambió por:

- **Decisiones del cliente** (relevadas en las dailies y en el POS).
- **Criterios técnicos** adoptados por el equipo (modelo de datos, arquitectura, validaciones).
- **Hallazgos de la demo** del 08/10/2026 (validaciones faltantes, inconsistencias de UI).

Este documento entrega la **versión final** de cada US del alcance del Sprint 1.

---

## 2. Consultas y resoluciones del refinement

Resumen de los temas tratados en las dailies del Sprint 1 (05/10 y 09/10):

| Tema | Resolución |
| :--- | :--- |
| **Registro de actores** | El sistema solo permite el autorregistro de usuarios con rol **Pasajero**. Los roles **Empleado de Mostrador** y **Administrador** son creados por un Administrador. |
| **Modelo de avión al crear vuelo** | El modelo de avión está **predefinido por el sistema**. Se contemplan tres tipos: **regional**, **fuselaje ancho** y **fuselaje estrecho**. |
| **Origen / destino** | Se optó inicialmente por **texto libre** (queda pendiente la validación de formato). |
| **Categorías (clases) de vuelo** | Existen dos categorías: **Economy** y **Primera**. |
| **Funcionalidades del Empleado de Mostrador** | Quedan **pendientes para el siguiente sprint**. En el Sprint 1 únicamente se debe implementar el **acceso a la página del rol**. |
| **Validación de código de vuelo** | Formato **2 o 3 letras seguidas de hasta 5 números** (ej. `AB12345`). |
| **Validación de ruta (origen/destino)** | Solo **letras**; se permiten **guiones**, no números. |
| **Manejo de error al crear vuelo** | Ante un dato inválido debe mostrarse un **cartel de error en la misma página** (mismo componente que en la modificación), **sin redirigir** a otra página. |
| **Tipos de avión consistentes** | Unificar el listado de tipos de avión entre **crear** y **modificar** vuelo. |
| **Diseño del registro de cuenta** | Mayor **contraste** en el desplegable de tipo de documento y revisión general del diseño. |

---

## 3. Historias de Usuario — versión final (Sprint 1)

| Id | Nombre | Descripción final | Prioridad | Estimación (hs) | Sprint | Cambios vs. Sprint 0 |
| :--: | :--- | :--- | :--: | :--: | :--: | :--- |
| **US-01** | Creación de Vuelos Programados | Como Administrador del sistema, quiero crear nuevos vuelos definiendo **código de vuelo** (2–3 letras + hasta 5 números), ruta (origen/destino, solo letras y guiones), días de operación, horarios de salida y llegada, disponibilidad anual (periodo del año), **modelo de avión predefinido** (regional, fuselaje ancho o fuselaje estrecho), capacidades y precios por clase (**Economy / Primera**), para ponerlos a la venta en el catálogo oficial de la aerolínea. | Alta | 6 hs | 1 | Se agrega formato de código de vuelo y validación de ruta; el modelo de avión pasa a ser predefinido (3 tipos); se explicitan las clases Economy/Primera; el error de validación se muestra en la misma página. |
| **US-02** | Modificación de Vuelos Programados | Como Administrador del sistema, quiero modificar los datos de un vuelo existente (código, ruta, horarios, días de operación, periodo anual, capacidades o precios por clase), para gestionar los cambios en un determinado vuelo. | Media | 4 hs | 1 | Se aplican las mismas validaciones que en la creación (código de vuelo y ruta); se unifica el listado de tipos de avión con el de creación. |
| **US-03** | Cancelación de un Vuelo en Fecha Específica | Como Administrador del sistema, quiero cancelar la salida de un vuelo para una fecha puntual en específico, para responder a situaciones inesperadas (clima, mantenimiento, etc.) sin afectar la programación anual de las demás salidas programadas. | Media | 4 hs | 1 | Sin cambios de alcance; se integra con las notificaciones (US-05). |
| **US-04** | Cancelación de la Operación Completa de un Vuelo | Como Administrador del sistema, quiero dar de baja la operación completa de un vuelo (todas sus fechas asociadas), para retirar del catálogo una ruta o itinerario. | Baja | 3 hs | 1 | Sin cambios de alcance; se integra con las notificaciones (US-05). |
| **US-05** | Notificación por Email por Cancelación de vuelo | Como Pasajero con reserva en un vuelo, quiero recibir una alerta por correo electrónico automáticamente cuando un vuelo sea cancelado, para estar informado a tiempo y poder reprogramar o gestionar mi viaje. | Alta | 4 hs | 1 | Se aclara que **no se envía correo si no hay pasajeros** afectados. |
| **US-06** | Notificación por Email por Modificación de Vuelo | Como Pasajero con reserva en un vuelo, quiero recibir una alerta por correo electrónico automáticamente cuando un vuelo sufra un cambio, para estar informado a tiempo y poder reprogramar o gestionar mi viaje. | Alta | 4 hs | 1 | Se aclara que **no se envía correo si no hay pasajeros** afectados; el correo identifica datos originales y modificados. |
| **US-07** | Búsqueda de Vuelos Directos | Como Pasajero, quiero buscar vuelos de tramos directos indicando origen, destino, tipo de tramo (solo ida o ida y vuelta) y fechas, para consultar las opciones disponibles. | Alta | 5 hs | 1 | Se confirma que solo se consideran tramos directos (sin escalas). |
| **US-08** | Inicio de Sesión y Control de Acceso por Roles | Como Usuario registrado (Pasajero, Empleado de mostrador o Administrador), quiero iniciar sesión con mi email y contraseña, para acceder a las funcionalidades y permisos correspondientes a mi perfil. | Alta | 3 hs | 1 | Se aclara que solo el Pasajero se autorregistra; el Administrador crea los roles Empleado de Mostrador y Administrador. En Sprint 1, el rol Empleado solo accede a su página (funcionalidades pendientes). |
| **US-09** | Registro de Cuenta de Pasajeros | Como Pasajero nuevo, quiero crear una cuenta en la plataforma ingresando mis datos personales (DNI, Nombre, Apellido, Email, Teléfono, Contraseña y Fecha de nacimiento), para agilizar futuras compras de pasajes y consultar mi historial de reservas. | Alta | 4 hs | 1 | Se restringe el autorregistro al rol **Pasajero**; se mejora el contraste del desplegable de tipo de documento y el diseño general. |
| **US-10** | Compra de Pasajes | Como Comprador, quiero seleccionar hasta 9 pasajes en una misma transacción e ingresar los datos personales (DNI, Nombre, Edad y Teléfono) de cada integrante, para registrar formalmente a todos los pasajeros que viajan conmigo. | Media | 3 hs | 1 | **Repriorizada** desde Sprint 2 (ver Retrospectiva Sprint 1). |
| **US-13** | Cancelación de Reserva desde Plataforma Web | Como Pasajero, quiero solicitar la cancelación de mi reserva desde el portal web hasta 48 horas antes del despegue, para autogestionar la anulación de mi pasaje. | Alta | 2 hs | 1 | **Repriorizada** desde Sprint 2 (ver Retrospectiva Sprint 1). |

---

## 4. Escenarios y criterios de aceptación por US

### US-01 — Creación de Vuelos Programados

**Escenario 1 — Camino exitoso**
1. Loguearse con un usuario Administrador.
2. Seleccionar "Crear Nuevo Vuelo" en el panel de administrador.
3. Completar los campos obligatorios (código `AB12345`, ruta, días, horarios, periodo, avión, capacidades y precios).
4. Presionar "Publicar".

**Resultado esperado:** el vuelo se da de alta en el catálogo y todos los campos se guardan correctamente. Se muestra el cartel "Vuelo creado con éxito" y el vuelo aparece en "Todos los vuelos".

**Escenario 2 — Camino de excepciones (dato inválido)**
1. Loguearse con un usuario Administrador.
2. Seleccionar "Crear Nuevo Vuelo".
3. Ingresar un dato incoherente (p. ej. horario de llegada anterior al de salida, código con formato inválido o ruta con números).
4. Presionar "Publicar".

**Resultado esperado:** el sistema **no redirige** a otra página; muestra un **cartel de error de validación** (mismo componente que en la modificación), indicando los campos erróneos/pendientes, y mantiene los datos cargados en la misma página.

**Criterios de aceptación**
- El **código de vuelo** acepta 2 o 3 letras seguidas de hasta 5 números; rechaza otro formato.
- La **ruta (origen/destino)** acepta solo letras y guiones; rechaza números.
- El **modelo de avión** se elige de una lista predefinida (regional, fuselaje ancho, fuselaje estrecho).
- Se definen capacidades y precios para **Economy** y **Primera**.
- Si un campo obligatorio está incompleto, el botón "Publicar" permanece deshabilitado.

---

### US-02 — Modificación de Vuelos Programados

**Escenario 1 — Camino exitoso**
1. Loguearse con un usuario Administrador.
2. Seleccionar "Todos los vuelos" y presionar "Modificar".
3. Modificar los campos deseados correctamente.
4. Presionar "Publicar cambios".

**Resultado esperado:** la acción se procesa sin errores y se muestra el cartel "Vuelo modificado correctamente".

**Escenario 2 — Camino de excepciones**
1. Loguearse con un usuario Administrador.
2. Seleccionar "Todos los vuelos" y presionar "Modificar".
3. Modificar un campo ingresando un valor incorrecto.
4. Presionar "Publicar cambios".

**Resultado esperado:** el sistema no procesa la actualización, muestra una alerta de error de validación y conserva los datos originales del vuelo intactos.

**Criterios de aceptación**
- Se aplican las mismas validaciones de código de vuelo y ruta que en US-01.
- El listado de tipos de avión es **idéntico** al de la creación.

---

### US-03 — Cancelación de un Vuelo en Fecha Específica

**Escenario 1 — Camino exitoso**
1. Loguearse con un usuario Administrador.
2. Seleccionar "Todos los vuelos" y presionar "Cancelar".
3. Elegir la modalidad "Cancelar en fecha puntual".
4. Seleccionar la fecha e ingresar el motivo.
5. Presionar "Confirmar cancelación".

**Resultado esperado:** se cancela únicamente la salida del vuelo para la fecha seleccionada, manteniendo el resto de las salidas del año sin alteraciones. Se muestra el cartel "Vuelo cancelado correctamente".

**Criterios de aceptación**
- Solo se ve afectada la fecha elegida.
- Se dispara la notificación por email a los pasajeros con reserva (US-05).

---

### US-04 — Cancelación de la Operación Completa de un Vuelo

**Escenario 1 — Camino exitoso**
1. Loguearse con un usuario Administrador.
2. Seleccionar "Todos los vuelos" y presionar "Cancelar".
3. Elegir la modalidad "Eliminar vuelo".
4. Presionar "Confirmar cancelación".

**Resultado esperado:** la frecuencia de vuelo queda eliminada de forma definitiva y se muestra el cartel "Frecuencia cancelada correctamente".

**Criterios de aceptación**
- Se eliminan todas las fechas asociadas a la frecuencia.
- Se dispara la notificación por email a los pasajeros con reserva (US-05).

---

### US-05 — Notificación por Email por Cancelación de vuelo

**Escenario 1 — Camino exitoso**
1. Loguearse con un usuario Administrador.
2. Cancelar un vuelo (puntual o frecuencia completa).
3. Confirmar la cancelación.
4. Abrir la casilla de prueba de un pasajero afectado.
5. Verificar el email recibido.

**Resultado esperado:** llega el email a la casilla del pasajero afectado, identificando correctamente el vuelo cancelado con su fecha y horario.

**Escenario 2 — Sin pasajeros afectados**
1. Cancelar un vuelo sin pasajeros.
2. Confirmar la cancelación.

**Resultado esperado:** el sistema detecta que no hay pasajeros y **no envía** ningún correo.

---

### US-06 — Notificación por Email por Modificación de Vuelo

**Escenario 1 — Camino exitoso**
1. Loguearse con un usuario Administrador.
2. Modificar un vuelo.
3. Confirmar la modificación.
4. Abrir la casilla de prueba de un pasajero afectado.
5. Verificar el email recibido.

**Resultado esperado:** llega el email a la casilla del pasajero afectado, identificando el vuelo modificado con sus datos originales y los modificados.

**Escenario 2 — Sin pasajeros afectados**
1. Modificar un vuelo sin pasajeros.
2. Confirmar la modificación.

**Resultado esperado:** el sistema **no envía** ningún correo.

---

### US-07 — Búsqueda de Vuelos Directos

**Escenario 1 — Camino exitoso**
1. Loguearse con un usuario Pasajero.
2. Seleccionar "Buscar vuelos".
3. Completar origen, destino, fecha/s, tipo de tramo y cantidad de asientos.
4. Presionar el botón de búsqueda.

**Resultado esperado:** el sistema lista todos los vuelos directos que cumplen con los datos ingresados.

**Escenario 2 — Campos obligatorios incompletos**
1. Dejar incompleto algún campo obligatorio.
2. Presionar el botón de búsqueda.

**Resultado esperado:** el sistema muestra un cartel solicitando el ingreso de los campos obligatorios.

**Escenario 3 — Sin resultados**
1. Completar los campos con datos sin coincidencias.
2. Presionar el botón de búsqueda.

**Resultado esperado:** el sistema informa que no existen vuelos que satisfagan la búsqueda y solicita un nuevo conjunto de datos.

**Criterios de aceptación**
- Solo se consideran tramos directos (sin escalas).
- El resultado se carga en pantalla en menos de 2 segundos (RNF01).

---

### US-08 — Inicio de Sesión y Control de Acceso por Roles

**Escenario 1 — Inicio de sesión exitoso (Pasajero)**
1. Ingresar a la página principal.
2. Completar correo electrónico y contraseña.
3. Presionar "Iniciar sesión".

**Resultado esperado:** el sistema valida las credenciales y redirige al usuario a la vista de su rol (Pasajero).

**Escenario 2 — Rol Administrador**
1. Iniciar sesión con credenciales de Administrador.

**Resultado esperado:** redirige a la vista de Administrador, con las opciones correspondientes (Todos los vuelos, Crear nuevo vuelo, etc.).

**Escenario 3 — Rol Empleado de mostrador**
1. Iniciar sesión con credenciales de Empleado de mostrador.

**Resultado esperado:** redirige a la página del rol Empleado de mostrador. En Sprint 1 la página solo da acceso; sus funcionalidades están pendientes para el sprint siguiente.

**Escenario 4 — Credenciales inválidas**
1. Ingresar credenciales no registradas o contraseña incorrecta.
2. Presionar "Iniciar sesión".

**Resultado esperado:** el sistema rechaza el intento, muestra un mensaje de alerta y no inicia sesión.

**Criterios de aceptación**
- Solo el rol **Pasajero** puede autorregistrarse.
- Los roles **Empleado de Mostrador** y **Administrador** son creados por un Administrador.

---

### US-09 — Registro de Cuenta de Pasajeros

**Escenario 1 — Registro exitoso**
1. Ingresar a la página de inicio de sesión.
2. Seleccionar "Registrarme".
3. Completar los campos obligatorios (DNI, Nombre, Apellido, Email, Teléfono, Contraseña y Fecha de nacimiento; tipo de documento).
4. Presionar "Registrarme".

**Resultado esperado:** el sistema valida los datos y crea un nuevo usuario **Pasajero** con los valores ingresados.

**Escenario 2 — Datos ya registrados**
1. Completar los campos con datos de un usuario existente.
2. Presionar "Registrarme".

**Resultado esperado:** el sistema detecta el duplicado y muestra un cartel de error informando que ya existe un usuario registrado con esos datos.

**Criterios de aceptación**
- El desplegable de **tipo de documento** presenta contraste suficiente con el fondo.
- El diseño general del formulario de registro se revisa según el hallazgo de la demo.

---

### US-10 — Compra de Pasajes

**Escenario 1 — Camino exitoso**
1. Loguearse con un usuario Pasajero.
2. Haber realizado una búsqueda y seleccionado un vuelo.
3. Seleccionar la cantidad de pasajes deseada (hasta 9).
4. Completar los datos personales (DNI, Nombre, Edad y Teléfono) de cada integrante.
5. Presionar el botón para confirmar/continuar.

**Resultado esperado:** el sistema registra a todos los pasajeros, asocia sus datos a la transacción y permite avanzar al siguiente paso de la compra, mostrando una indicación visual de guardado correcto.

**Escenario 2 — Límite de pasajes excedido**
1. Intentar seleccionar más de 9 pasajes para la misma transacción.

**Resultado esperado:** el sistema no permite superar los 9 pasajes, mostrando un error o deshabilitando la opción de agregar más pasajeros.

**Escenario 3 — Campos obligatorios incompletos**
1. Seleccionar una cantidad válida de pasajes.
2. Omitir un dato obligatorio de al menos un pasajero.
3. Intentar continuar.

**Resultado esperado:** el sistema bloquea la acción, mantiene el botón deshabilitado o muestra los campos requeridos faltantes.

**Criterios de aceptación**
- No se puede comprar dos pasajes a nombre de la misma persona.
- Máximo 9 pasajes por transacción.

---

### US-13 — Cancelación de Reserva desde Plataforma Web

**Escenario 1 — Camino exitoso (cancelación a tiempo)**
1. Loguearse con un usuario Pasajero.
2. Navegar a "Mis Reservas".
3. Seleccionar una reserva cuyo despegue sea dentro de **más de 48 horas**.
4. Presionar la opción de cancelación.
5. Confirmar la cancelación.

**Resultado esperado:** el sistema anula el pasaje y actualiza el estado de la reserva, mostrando un mensaje de confirmación.

**Escenario 2 — Cancelación fuera de término (menos de 48 hs)**
1. Seleccionar una reserva cuyo despegue sea dentro de **menos de 48 horas**.
2. Intentar cancelar.

**Resultado esperado:** el sistema no permite la anulación; el botón se deshabilita/oculta o muestra un mensaje informando que expiró el plazo permitido (hasta 48 horas antes del despegue).

**Criterios de aceptación**
- Solo se puede cancelar hasta **48 horas antes** del despegue.
- La acción se realiza desde el perfil del pasajero autenticado.

---

## 5. Repriorizaciones

Las siguientes US fueron repriorizadas respecto de las tablas de Sprint 0 y quedan documentadas en `Retrospectiva Sprint 1 - Comisión 7.md`:

- **US-10 (Compra de Pasajes)** y **US-13 (Cancelación desde plataforma web)**: adelantadas del Sprint 2 al **Sprint 1**.
- **US-05 y US-06 (Notificaciones por email)**: se ratifican en el **Sprint 1**.

---

## 6. Próximos pasos

- Incorporar las resoluciones del refinement a la implementación del Sprint 1.
- Mantener el formato final de las US como referencia para los sprints 2 y 3.
- Dejar pendientes para el sprint siguiente: funcionalidades del Empleado de Mostrador; validación de formato de origen/destino.
