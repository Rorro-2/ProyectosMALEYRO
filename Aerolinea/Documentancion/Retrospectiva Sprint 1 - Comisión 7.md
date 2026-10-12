# Retrospectiva Sprint 1 - Comisión 7

> Documento de retrospectiva del Sprint 1 del sistema **Sky Link**. Registra las correcciones surgidas de la demo, las decisiones de repriorización del backlog y las notas para los sprints siguientes.

---

## 1. Correcciones y refinamientos surgidos de la demo

| # | Hallazgo | US afectada | Sprint | Tipo |
| :--: | :--- | :--: | :--: | :--- |
| 1 | Al crear un vuelo con datos inválidos se redirige a otra página. Debe mostrarse un cartel de error en la misma página, reutilizando el mismo componente que se muestra al modificar un vuelo con datos inválidos. | US-01 / US-02 | 1 | Bug |
| 2 | Origen/destino de la ruta: no se deben poder ingresar números. Solo letras; se permiten guiones. | US-01 / US-02 | 1 | Validación |
| 3 | Código de vuelo: definir formato de 2 o 3 letras seguidas de hasta 5 números (ej. `AB12345`). | US-01 / US-02 | 1 | Validación |
| 4 | Los tipos de avión que se muestran al crear un vuelo no coinciden con los de la modificación. Unificar el listado. | US-01 / US-02 | 1 | Bug / UI |
| 5 | Registro de cuenta: el desplegable de tipo de documento necesita más contraste con el fondo. Revisar el diseño general al crear una cuenta. | US-09 | 1 | UI |
| 6 | El rol Empleado debe mostrar sus operaciones y notificaciones. Falta implementar lo relacionado a empleado de mostrador. | US-08 | 2 | Pendiente |

---

## 2. Repriorizaciones

| US | Nombre | Sprint nuevo | Motivo |
| :--: | :--- | :--: | :--- |
| US-05 | Notificación por email por cancelación de vuelo | 1 | Ya en Sprint 1 (se ratifica) |
| US-06 | Notificación por email por modificación de vuelo | 1 | Ya en Sprint 1 (se ratifica) |
| US-10 | Compra de pasajes | **1** (desde 2) | Reserva de pasajes prioritario |
| US-13 | Cancelación de reserva desde plataforma web | **1** (desde 2) | Junto a la compra de pasajes |
| US-11 | Pago con único medio de pago | 2 | "Sprint 2 parte de pagos tiene que estar" |
| US-12 | Pago combinado con múltiples tarjetas | 2 | Idem pagos |
| US-15 | Consulta tabular de ocupación por vuelo | 2 | Sin cambios |
| US-16 | Filtros avanzados y comparativa por período y clase | 2 | Sin cambios |
| US-18 | Mostrador: búsqueda de reservas por pasajero | 2 | Todo lo relacionado a mostrador al Sprint 2 |
| US-19 | Mostrador: búsqueda de reservas por vuelo | 2 | Idem mostrador |
| US-20 | Validación de tickets electrónicos | 2 | Decisión final (no se posterga a Sprint 3) |
| US-14 | Cancelación de reserva desde App Móvil | 3 | Sin cambios |
| US-17 | Exportación de reportes de ocupación (PDF) | **3** (desde 2) | Postergada |
| US-21 | Reubicación manual de pasajeros | **3** (desde 2) | Postergada ("vemos después") |

---

## 3. Notas adicionales

- **Notificaciones y reserva/compra de pasajes** se priorizan en el Sprint 1.
- **SPRINT 2**: debe incluir la parte de pagos (único medio y combinado con múltiples tarjetas), la gestión de ocupación (consulta tabular y filtros) y todo lo relacionado al empleado de mostrador (búsquedas por DNI y por vuelo, validación de tickets).
- **SPRINT 3**: validación de tickets evaluada originalmente junto a exportación de reportes y reubicación manual; la decisión final deja US-20 en Sprint 2 y US-17/US-21 en Sprint 3.
- Las repriorizaciones impactan en `requerimientosMayorPrioridadSprint1.md` y `requerimientosMayorPrioridadSprint2.md`.
