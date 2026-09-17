# WBS — Sistema Integral "Sky Link" (Aerolínea Nacional)

Basado en la teoría de *Planificación de Proyectos* (03-PSS-APS-Planificacion.pdf, sección WBS) y en la documentación de la Comisión 7 (Enunciado, POS, clarificaciones, riesgos y métricas).

**Convención de cátedra aplicada:**
- El trabajo se divide en **actividades**, y las actividades se dividen en **tareas**.
- **Nivel 0** = la meta del proyecto.
- **Nivel 1** = actividades (enfoque **por sustantivos**: entregables del producto).
- **Nivel 2** = tareas (enfoque **por verbos**: acciones que producen el entregable).
- Cada tarea cumple los **6 criterios de completitud**: estado medible, acotada, produce un entregable, tiempo y costo estimable, duración aceptable (≤ 10 días) e independiente.
- Sobre el último nivel (las tareas) se estimarán luego esfuerzo, tiempos y recursos.

---

## Árbol del WBS

```
0. "SKY LINK" — Sistema integral web + app móvil para pasajeros        ◄── NIVEL 0 (Meta: digitalizar y
│                                                                         centralizar la gestión operativa,
│                                                                         optimizar la venta y mejorar la
│                                                                         experiencia del pasajero)
│
├─ 1. Gestión del Proyecto                                              ◄── NIVEL 1 (Actividad)
│   ├─ 1.1 Confeccionar el plan del proyecto        → Entregable: Plan del proyecto aprobado (cronograma, recursos, propuesta)
│   ├─ 1.2 Gestionar riesgos                        → Entregable: Tabla de riesgos + PRSGR
│   ├─ 1.3 Reportar el estado por sprint            → Entregable: Reportes de estado periódicos
│   └─ 1.4 Gestionar cambios de alcance             → Entregable: Registro de cambios y comunicaciones con el cliente
│
├─ 2. Análisis de Requerimientos
│   ├─ 2.1 Relevar requerimientos con el cliente                → Entregable: Actas de relevamiento (COS y sesiones de clarificación)
│   ├─ 2.2 Especificar requerimientos funcionales               → Entregable: Historias de usuario y especificación funcional
│   ├─ 2.3 Especificar requerimientos no funcionales            → Entregable: Especificación no funcional (búsqueda < 2 s, seguridad, disponibilidad)
│   └─ 2.4 Validar los requerimientos con stakeholders          → Entregable: Acta de aprobación de requerimientos
│
├─ 3. Diseño de la Solución
│   ├─ 3.1 Diseñar la arquitectura del sistema        → Entregable: Documento de arquitectura (web, app, API, BD, servicios externos)
│   ├─ 3.2 Diseñar el modelo de datos                 → Entregable: Modelo de base de datos (vuelos, pasajes, usuarios, pagos, ocupación)
│   ├─ 3.3 Diseñar la UI/UX web (pasajero, mostrador, admin) → Entregable: Prototipos / wireframes de la web
│   ├─ 3.4 Diseñar los prototipos de la app móvil     → Entregable: Prototipos de la app móvil
│   └─ 3.5 Diseñar las integraciones externas         → Entregable: Especificación de API (pagos, email, WhatsApp, generación de PDF)
│
├─ 4. Construcción del Sistema Web
│   ├─ 4.1  Implementar el backend y la base de datos → Entregable: Backend + BD funcionales
│   ├─ 4.2  Implementar autenticación y perfiles      → Entregable: Módulo de usuarios (pasajero, mostrador, administrador)
│   ├─ 4.3  Implementar la gestión de vuelos          → Entregable: Módulo de vuelos (CRUD: días, horarios, rutas, período, capacidad, precios)
│   ├─ 4.4  Implementar la búsqueda de vuelos         → Entregable: Módulo de búsqueda (origen/destino, fecha, ida / ida y vuelta)
│   ├─ 4.5  Implementar la compra de pasajes          → Entregable: Módulo de compra (máx. 9 pasajes, clase Economy/Primera, invitado o registrado)
│   ├─ 4.6  Implementar la gestión de pagos y facturación → Entregable: Módulo de pagos (validación tarjeta, transacción, factura)
│   ├─ 4.7  Implementar el check-in y selección de asientos → Entregable: Módulo de check-in (desde 2 semanas antes, hasta 48 h)
│   ├─ 4.8  Implementar el control de ocupación       → Entregable: Módulo de reportes (ocupación por vuelo, clase y fecha)
│   ├─ 4.9  Implementar las notificaciones            → Entregable: Módulo de notificaciones (email y WhatsApp ante cambios/cancelaciones)
│   ├─ 4.10 Implementar cancelaciones y reubicación   → Entregable: Módulo de cancelación / reprogramación y reubicación en mostrador
│   └─ 4.11 Implementar pasajes electrónicos (PDF)    → Entregable: Generador de pasajes y facturas en PDF
│
├─ 5. Desarrollo de la App Móvil (iOS + Android)
│   ├─ 5.1 Configurar la base multiplataforma y navegación → Entregable: App móvil base compilable
│   ├─ 5.2 Implementar búsqueda y compra en la app    → Entregable: Búsqueda y compra de pasajes móviles
│   ├─ 5.3 Implementar check-in y tickets en la app   → Entregable: Check-in y descarga de tickets electrónicos móviles
│   └─ 5.4 Implementar notificaciones e historial     → Entregable: Alertas móviles y gestión de reservas (historial de 2 años)
│
├─ 6. Pruebas y Calidad
│   ├─ 6.1 Definir el plan y los casos de prueba      → Entregable: Plan y casos de prueba por módulo
│   ├─ 6.2 Ejecutar pruebas unitarias                 → Entregable: Reporte de pruebas unitarias
│   ├─ 6.3 Ejecutar pruebas de integración            → Entregable: Reporte de integración (pagos, email, WhatsApp, PDF)
│   ├─ 6.4 Ejecutar pruebas de sistema y UAT          → Entregable: Pruebas de aceptación con el usuario aprobadas
│   ├─ 6.5 Ejecutar pruebas de rendimiento/concurrencia → Entregable: Reporte de rendimiento (búsqueda < 2 s, check-in simultáneo)
│   └─ 6.6 Ejecutar pruebas de seguridad              → Entregable: Reporte de seguridad (sanitización de inputs, accesos)
│
└─ 7. Despliegue, Migración y Cierre
    ├─ 7.1 Preparar el entorno de producción          → Entregable: Entorno e infraestructura disponibles
    ├─ 7.2 Migrar los datos existentes                → Entregable: Datos migrados y verificados
    ├─ 7.3 Capacitar al personal                      → Entregable: Capacitación de mostrador y administradores realizada
    ├─ 7.4 Desplegar web y publicar la app            → Entregable: Sistema en producción / app publicada
    └─ 7.5 Realizar la auditoría post-implementación  → Entregable: Informe de cierre del proyecto
```

**Resumen de niveles:** Nivel 0 = 1 nodo (meta) · Nivel 1 = 7 actividades · Nivel 2 = 34 tareas.

---

## Verificación de los 6 criterios de completitud por tarea

Criterios: (1) **Estado medible**, (2) **Acotada** (fecha de comienzo y fin), (3) **Producir un entregable** (columna "Entregable"), (4) **Tiempo y costo estimable**, (5) **Duración aceptable** ≤ 10 días (2 semanas laborables; duración inicial sugerida, a refinar con las técnicas de estimación), (6) **Independiente**.

| ID | Tarea | Entregable | Medible | Acotada | Estimable | Duración | Independiente |
|----|-------|-----------|:------:|:------:|:--------:|:--------:|:------------:|
| 1.1 | Confeccionar el plan del proyecto | Plan del proyecto aprobado | ✓ | ✓ | ✓ | 3–5 dd | ✓ |
| 1.2 | Gestionar riesgos | Tabla de riesgos + PRSGR | ✓ | ✓ | ✓ | 2–4 dd | ✓ |
| 1.3 | Reportar el estado por sprint | Reportes de estado | ✓ | ✓ | ✓ | 1–2 dd | ✓ |
| 1.4 | Gestionar cambios de alcance | Registro de cambios y comunicaciones | ✓ | ✓ | ✓ | 1–2 dd | ✓ |
| 2.1 | Relevar requerimientos con el cliente | Actas de relevamiento | ✓ | ✓ | ✓ | 3–5 dd | ✓ |
| 2.2 | Especificar requerimientos funcionales | Especificación funcional / historias de usuario | ✓ | ✓ | ✓ | 4–6 dd | ✓ |
| 2.3 | Especificar requerimientos no funcionales | Especificación no funcional | ✓ | ✓ | ✓ | 2–3 dd | ✓ |
| 2.4 | Validar los requerimientos con stakeholders | Acta de aprobación | ✓ | ✓ | ✓ | 1–2 dd | ✓ |
| 3.1 | Diseñar la arquitectura del sistema | Documento de arquitectura | ✓ | ✓ | ✓ | 3–5 dd | ✓ |
| 3.2 | Diseñar el modelo de datos | Modelo de base de datos | ✓ | ✓ | ✓ | 3–5 dd | ✓ |
| 3.3 | Diseñar la UI/UX web (3 roles) | Prototipos / wireframes web | ✓ | ✓ | ✓ | 4–6 dd | ✓ |
| 3.4 | Diseñar los prototipos de la app móvil | Prototipos de la app | ✓ | ✓ | ✓ | 3–5 dd | ✓ |
| 3.5 | Diseñar las integraciones externas | Especificación de API | ✓ | ✓ | ✓ | 2–4 dd | ✓ |
| 4.1 | Implementar el backend y la base de datos | Backend + BD funcionales | ✓ | ✓ | ✓ | 5–8 dd | ✓ |
| 4.2 | Implementar autenticación y perfiles | Módulo de usuarios | ✓ | ✓ | ✓ | 3–5 dd | ✓ |
| 4.3 | Implementar la gestión de vuelos | Módulo de vuelos | ✓ | ✓ | ✓ | 5–7 dd | ✓ |
| 4.4 | Implementar la búsqueda de vuelos | Módulo de búsqueda | ✓ | ✓ | ✓ | 5–7 dd | ✓ |
| 4.5 | Implementar la compra de pasajes | Módulo de compra | ✓ | ✓ | ✓ | 5–7 dd | ✓ |
| 4.6 | Implementar la gestión de pagos y facturación | Módulo de pagos | ✓ | ✓ | ✓ | 4–6 dd | ✓ |
| 4.7 | Implementar el check-in y selección de asientos | Módulo de check-in | ✓ | ✓ | ✓ | 4–6 dd | ✓ |
| 4.8 | Implementar el control de ocupación | Módulo de reportes | ✓ | ✓ | ✓ | 3–5 dd | ✓ |
| 4.9 | Implementar las notificaciones | Módulo de notificaciones | ✓ | ✓ | ✓ | 3–5 dd | ✓ |
| 4.10 | Implementar cancelaciones y reubicación | Módulo de cancelación/reprogramación | ✓ | ✓ | ✓ | 3–5 dd | ✓ |
| 4.11 | Implementar pasajes electrónicos (PDF) | Generador de pasajes y facturas PDF | ✓ | ✓ | ✓ | 3–5 dd | ✓ |
| 5.1 | Configurar la base multiplataforma y navegación | App móvil base compilable | ✓ | ✓ | ✓ | 3–5 dd | ✓ |
| 5.2 | Implementar búsqueda y compra en la app | Búsqueda y compra móviles | ✓ | ✓ | ✓ | 5–7 dd | ✓ |
| 5.3 | Implementar check-in y tickets en la app | Check-in y tickets móviles | ✓ | ✓ | ✓ | 4–6 dd | ✓ |
| 5.4 | Implementar notificaciones e historial | Alertas móviles y historial de reservas | ✓ | ✓ | ✓ | 3–5 dd | ✓ |
| 6.1 | Definir el plan y los casos de prueba | Plan de pruebas | ✓ | ✓ | ✓ | 2–4 dd | ✓ |
| 6.2 | Ejecutar pruebas unitarias | Reporte de pruebas unitarias | ✓ | ✓ | ✓ | 4–6 dd | ✓ |
| 6.3 | Ejecutar pruebas de integración | Reporte de integración | ✓ | ✓ | ✓ | 3–5 dd | ✓ |
| 6.4 | Ejecutar pruebas de sistema y UAT | UAT aprobada | ✓ | ✓ | ✓ | 4–6 dd | ✓ |
| 6.5 | Ejecutar pruebas de rendimiento/concurrencia | Reporte de rendimiento | ✓ | ✓ | ✓ | 3–5 dd | ✓ |
| 6.6 | Ejecutar pruebas de seguridad | Reporte de seguridad | ✓ | ✓ | ✓ | 2–4 dd | ✓ |
| 7.1 | Preparar el entorno de producción | Entorno e infraestructura disponibles | ✓ | ✓ | ✓ | 2–4 dd | ✓ |
| 7.2 | Migrar los datos existentes | Datos migrados y verificados | ✓ | ✓ | ✓ | 3–5 dd | ✓ |
| 7.3 | Capacitar al personal | Capacitación realizada | ✓ | ✓ | ✓ | 2–4 dd | ✓ |
| 7.4 | Desplegar web y publicar la app | Sistema en producción / app publicada | ✓ | ✓ | ✓ | 2–4 dd | ✓ |
| 7.5 | Realizar la auditoría post-implementación | Informe de cierre | ✓ | ✓ | ✓ | 2–3 dd | ✓ |