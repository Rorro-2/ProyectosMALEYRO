# Definir entregables asociados a cada tarea — Sprint 1 — Comisión 7

**Proyecto:** Sky Link — Sistema integral web + app móvil para pasajeros
**Sprint:** 1
**Objetivo:** definir el **entregable asociado a cada tarea realizada durante el Sprint 1**, estableciendo para cada una su criterio de verificación y su trazabilidad con las Historias de Usuario (US) del sprint.

---

## 1. Criterios de completitud de una tarea

Cada tarea se considera completa cuando cumple los 6 criterios:

1. **Estado medible:** en todo momento se puede determinar su avance.
2. **Acotada:** tiene fecha de comienzo y de fin.
3. **Produce un entregable:** genera un producto, documento o resultado visible.
4. **Tiempo y costo estimable.**
5. **Duración aceptable:** en lo posible ≤ 10 días.
6. **Independiente:** una vez comenzada, puede continuar sin interrupciones ni inputs externos.

---

## 2. Entregables por tarea (Sprint 1)

| ID tarea (WBS) | Tarea | Entregable | Criterio de verificación | US relacionada(s) | Sprint |
| :--: | :--- | :--- | :--- | :--- | :--: |
| **3.1** | Diseñar la arquitectura del sistema | Documento de arquitectura (web, app, API, BD, servicios externos) | El documento describe los componentes, sus responsabilidades y las integraciones externas; es aprobado por el equipo. | Transversal a US-01…US-13 | 1 |
| **3.2** | Diseñar el modelo de datos | Modelo de base de datos (vuelos, pasajes, usuarios, pagos, ocupación) | El modelo cubre las entidades necesarias y respeta las reglas de negocio (p. ej. máximo 9 pasajes por transacción). | Transversal a US-01…US-13 | 1 |
| **3.3** | Diseñar la UI/UX web (pasajero, mostrador, admin) | Prototipos / wireframes de la web | Los prototipos cubren las pantallas de creación/modificación de vuelos, búsqueda, registro/login y compra. | US-01, US-02, US-07, US-08, US-09, US-10, US-13 | 1 |
| **3.5** | Diseñar las integraciones externas | Especificación de API (pagos, email, WhatsApp, generación de PDF) | La especificación define endpoints, contratos y manejo de errores de cada servicio externo. | US-05, US-06 (email); base para US-11/US-12 (pagos) | 1 |
| **4.1** | Implementar el backend y la base de datos | Backend + BD funcionales | El backend expone los servicios base y la BD se crea según el modelo; migraciones aplicadas sin errores. | Transversal a US-01…US-13 | 1 |
| **4.2** | Implementar autenticación y perfiles | Módulo de usuarios (pasajero, mostrador, administrador) | Login por rol operativo (RBAC); solo el Pasajero se autorregistra; el Administrador crea Empleado y Administrador. | US-08, US-09 | 1 |
| **4.3** | Implementar la gestión de vuelos | Módulo de vuelos (CRUD: código, días, horarios, rutas, período, capacidad, precios) | Crear, modificar y cancelar vuelos con las validaciones de código (2–3 letras + hasta 5 números) y ruta (solo letras y guiones); error mostrado en la misma página. | US-01, US-02, US-03, US-04 | 1 |
| **4.4** | Implementar la búsqueda de vuelos | Módulo de búsqueda (origen/destino, fecha, ida / ida y vuelta) | La búsqueda devuelve solo vuelos directos que cumplen los filtros y responde en menos de 2 s (RNF01). | US-07 | 1 |
| **6.1** | Definir el plan y los casos de prueba | Plan y casos de prueba por módulo | El plan identifica los casos de prueba (exitosos y de excepción) por módulo del sprint. | Transversal a US-01…US-13 | 1 |
| **6.2** | Ejecutar pruebas unitarias | Reporte de pruebas unitarias | El reporte evidencia la ejecución de los casos unitarios y el resultado obtenido. | US-01…US-10, US-13 | 1 |
| **1.3** | Reportar el estado por sprint | Reportes de estado periódicos | El reporte documenta el avance, los bloqueos y las decisiones del sprint. | Gestión (todas las US) | 1 |

---

## 3. Matriz de trazabilidad US ↔ Tarea ↔ Entregable

| US | Tareas que la producen | Entregable principal |
| :--: | :--- | :--- |
| US-01 | 3.2, 3.3, 4.1, 4.3, 6.1, 6.2 | Módulo de vuelos (creación) |
| US-02 | 3.2, 3.3, 4.1, 4.3, 6.1, 6.2 | Módulo de vuelos (modificación) |
| US-03 | 3.2, 4.1, 4.3, 6.1, 6.2 | Módulo de vuelos (cancelación puntual) |
| US-04 | 3.2, 4.1, 4.3, 6.1, 6.2 | Módulo de vuelos (baja de frecuencia) |
| US-05 | 3.5, 4.1, 6.1, 6.2 | Módulo de notificaciones (email por cancelación) |
| US-06 | 3.5, 4.1, 6.1, 6.2 | Módulo de notificaciones (email por modificación) |
| US-07 | 3.2, 3.3, 4.1, 4.4, 6.1, 6.2 | Módulo de búsqueda de vuelos |
| US-08 | 3.3, 4.1, 4.2, 6.1, 6.2 | Módulo de autenticación y roles |
| US-09 | 3.3, 4.1, 4.2, 6.1, 6.2 | Módulo de registro de pasajeros |
| US-10 | 3.2, 3.3, 4.1, 6.1, 6.2 | Módulo de compra de pasajes |
| US-13 | 3.2, 3.3, 4.1, 6.1, 6.2 | Cancelación de reserva desde web |

---

## 4. Notas

- **Entregables de diseño (3.x):** son documentos/prototipos que habilitan la implementación; su entregable es verificable por revisión del equipo.
- **Entregables de implementación (4.x):** módulos funcionales verificables mediante pruebas.
- **Tareas de prueba (6.x):** producen reportes que evidencian la calidad del incremento.
- **Tarea de gestión (1.3):** transversal; produce los reportes de estado del sprint.
- La trazabilidad con las US permite verificar que cada historia del Sprint 1 tenga al menos una tarea que la materialice.
