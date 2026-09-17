# Planificación de Proyectos — Resumen

Fuente: *Administración de Proyectos de Software — Sesión de Planificación* (E. Estévez - P. Fillottrani, DCIC, UNS, segundo semestre 2026).

Contenido: 1) Sesión de Planificación, 2) WBS, 3) Estimación de Esfuerzos, 4) Cronograma, 5) Propuesta de Proyecto.

---

## 1. Sesión de Planificación

### Importancia de la Planificación
- Para el LP no es sólo una ruta para el trabajo a realizar, sino también una ayuda en la toma de decisiones.
- Es esperable el cambio: no hay que tomar la planificación como algo fijo; hay que estar preparado para el cambio.
- Beneficios:
  - Reducción de incertidumbre.
  - Incremento del conocimiento.
  - Mejora en la eficiencia.

### Uso de herramientas de Software
- El tamaño del proyecto influye en el tipo de herramientas a usar.
- Ventaja: permiten investigar distintas alternativas ajustando parámetros.
- Desventajas:
  - No han sido muy efectivas en el manejo de recursos y a veces producen resultados desconcertantes.
  - Costos: dinero, tiempo de aprendizaje y de mantenimiento.
- Es muy importante incorporarles estimaciones confiables.

### Tiempo para la Planificación
- Proyectos tipo D: menos de un día.
- Proyectos tipo C: hasta dos días.
- Proyectos tipo B: tres o cuatro días.
- Proyectos tipo A: cinco o más días.

### Herramientas y Procesos
- JPPS (Joint Project Planning Session).
- WBS (Work Breakdown Structure).
- Técnicas de estimación de duración, recursos y costos.
- Técnicas de construcción y compresión de cronogramas.
- Planificación del manejo de riesgos.
- Propuesta de Proyecto y obtención de la aprobación de la propuesta.

### Sesión Conjunta de Planificación de Proyecto (JPPS)
- Es una sesión grupal para generar el plan detallado.
- Objetivo: desarrollar un plan que satisfaga el COS y describa el POS.
- Obstáculo: poco tiempo de los miembros para planificar y reuniones virtuales.

#### Agenda de la JPPS
1. Revisión del POS.
2. Creación del WBS.
3. Estimación de duración y recursos para tareas.
4. Construcción del diagrama de red del proyecto.
5. Determinación del camino crítico.
6. Revisión y aprobación de la fecha de terminación.
7. Completar el cronograma.
8. Obtener consenso sobre el plan.

#### Roles
- **Facilitador**: conduce la sesión, de mente abierta (no es el LP) y con experiencia.
- **LP**: se concentra en el plan y no en la reunión; debe sentirse confiado en el plan resultante.
- **Consultor JPPS**: expertos externos para opinar sobre aspectos específicos, especialmente si no hay personal con experiencia.
- **Tecnógrafo**: ayuda al facilitador con las herramientas de software para documentar el proyecto.
- **Equipo central del proyecto**: participantes senior (ya involucrados), desde el primer día hasta el último.
- **Representante del cliente**: puede ser problemático.
- **Administradores de recursos**: expertos en estimación.
- **Campeón del proyecto**: encargado de "vender" el proyecto al/los gerentes. Puede ser el cliente.
- **Administradores funcionales**: proveen inputs o reciben outputs del proyecto; aseguran la integración de los entregables.

#### Entregables de la JPPS
- WBS (incluyendo estimación de duración y recursos).
- Diagrama de Red del proyecto.
- Cronograma de Tareas.
- Asignación de Recursos.
- Documento del Proyecto y Propuesta del Proyecto.

---

## 2. WBS (Work Breakdown Structure)

### Características generales
- El WBS es una **descripción jerárquica del trabajo** que se debe realizar para completar el proyecto.
- Es similar a una descomposición funcional.
- La jerarquía que se utiliza en la materia:
  - El trabajo se divide en **actividades**.
  - Las actividades se dividen en **tareas**.
  - (Es la convención de esta cátedra; otros autores la intercambian.)
- Se representa mediante un gráfico (diagrama de árbol) que parte del nivel 0 (la meta del proyecto) y se particiona hasta llegar a las tareas.

### Usos del WBS
1. **Diseñar y planificar el trabajo**: permite a los integrantes del equipo visualizar cómo puede definirse y administrarse el trabajo del proyecto.
2. **Diseñar la arquitectura**: es un gráfico del trabajo del proyecto; muestra cómo se relacionan los distintos ítems de trabajo a realizar.
3. **Planificar**: se debe estimar esfuerzo, tiempos y recursos para el **último nivel**.
4. **Informar el estado del proyecto**: se usa como estructura para mostrar el grado de avance.

### Construcción del WBS
- Su confección es **responsabilidad del LP**.
- Debe definirse de tal manera que el LP pueda administrar el proyecto.
- Para que funcione: se pueden usar stickers, resaltadores, pizarrón, paredes.
- Formas de construirlo:
  1. **Top-down**
     - Equipo completo.
     - Sub-equipos.
  2. **Bottom-up**.

#### Top-down — Equipo completo
- Todos los miembros del equipo participan de la descomposición.
- Se comienza con el **nivel 0** (el de la meta) y se particiona sucesivamente hasta que los participantes estén satisfechos de que el trabajo ha sido suficientemente definido.
- Debido a que las tareas se definen con suficiente nivel de detalle, las estimaciones de costo, tiempo y recursos son **más exactas**.
- Una vez definidas las tareas, se deben **secuenciar**: analizar qué tareas se pueden hacer concurrentemente.
- Ventaja: brinda la oportunidad de que todos presten atención al WBS y se discuta en el momento.

#### Top-down — Sub-equipos
- El equipo completo acuerda la partición del **primer nivel**.
- Se crean tantos sub-equipos como actividades haya en el nivel uno.
- Cada sub-equipo particiona una actividad (se le asigna la actividad de la que tenga más experiencia).
- Un sub-equipo puede solicitar ayuda externa.
- Demanda menos tiempo que el enfoque anterior.

#### Bottom-up
- Se asemeja a una lluvia de ideas (brainstorming).
- El grupo clasifica las tareas que parecieran relacionarse.
- Se reúnen todos los grupos y cada uno presenta sus resultados; se discute en conjunto.
- Desventaja: **no se definen las tareas con el suficiente grado de granularidad**.
- Existen metodologías que ayudan a la descomposición de actividades: proveen listados de tareas.

### Descripción completa de una tarea
Una tarea debe cumplir **6 criterios** para ser considerada completa:

1. **Estado medible**: en cualquier momento se debe poder determinar en qué estado se encuentra la tarea. (Ej.: "codificar 10 componentes" con tiempo asignado de 10 semanas: tras 4 semanas deben existir respuestas válidas de avance.)
2. **Acotada**: debe poseer evento/fecha de comienzo y evento/fecha de fin.
3. **Producir un entregable**: el entregable es un signo visible de que la tarea se completó. Puede ser un producto, un documento, una autorización para continuar con la próxima tarea, etc.
4. **Tiempo y costo estimable**: tiempo y costo deben ser fácilmente estimables. Estimar tiempo y costo para las tareas de menor nivel permite luego agregar y calcular el costo y tiempo total del proyecto.
5. **Duración aceptable**: en lo posible no trabajar con tareas de más de 10 días (2 semanas laborables). Cuidado: hay excepciones.
6. **Independiente**: una vez comenzada, se debe poder continuar razonablemente sin interrupciones ni necesidad de input adicional; el esfuerzo dedicado debe ser continuo.

### Enfoques para la construcción (criterios de nombrado)
- No hay reglas fijas; se pueden estipular criterios para nombrar las tareas:
  - **Enfoque por sustantivos**: en función de los entregables.
  - **Enfoque por verbos**: en función de las acciones requeridas para producir el entregable.
  - **Enfoque organizacional**: en función de las unidades organizativas que trabajarán en el proyecto.

---

## 3. Estimación de Esfuerzos

### Técnicas de estimación
- **Similitud con otras tareas**: estimar en base a las estimaciones de tareas similares de otros proyectos. Los datos están en la memoria de las personas.
- **Datos históricos**: igual que la similitud, pero los datos están en un registro o base de datos, no sólo en la memoria de las personas. La base histórica puede ser tan sofisticada como se desee.
- **Juicio experto**: las estimaciones las realizan consultores externos o vendedores con experiencia en la metodología o tecnología. Si se basa en vendedores, las estimaciones pueden no ser objetivas.
- **Técnica Delphi**: técnica de grupo que extrae y resume el conocimiento del grupo.
  - 1ᵉʳ pasada: cada miembro estima; resultados tabulados.
  - Los participantes cuyas estimaciones cayeron en los cuartiles exteriores deben justificar su estimación.
  - Tras escuchar argumentos, vuelven a estimar (2ᵃ pasada, histograma).
  - Se hace otra estimación (3ᵉʳ pasada), se permiten ajustes finales.
  - El **promedio de la 3ᵉʳ pasada** se usa como estimación del grupo.
- **Técnica de 3 puntos**: se necesitan 3 estimaciones de la duración de la tarea: optimista, pesimista y media.
  - Optimista: duración más corta suponiendo que todo suceda según lo planificado.
  - Pesimista: duración suponiendo que falle todo lo que se prevé que puede fallar.
  - Media: duración normal (usual) de la tarea.
  - Fórmula: `estimacion = (optimista + 4*media + pesimista) / 6`
- **Técnica Delphi de banda ancha**: combinación de Delphi y 3 puntos. Cada integrante da las 3 estimaciones; se eliminan los extremos, se calculan los promedios de optimistas, pesimistas y medias, y se aplica la fórmula de 3 puntos usando los promedios.

#### Otra clasificación de métodos de estimación
- Analogía con proyectos previos.
- Estimar tamaño:
  - Longitud (LOC).
  - Funcionalidad (Puntos de Función de Albrecht).
- Modelos algorítmicos: `a * (KLOC)^b * FactorAjuste` (COCOMO).
- Estimación top-down o bottom-up.

### Recursos
- **Clasificación**:
  - **Humanos**: los más difíciles de estimar en un proyecto de software.
  - **Facilidades**: lugares físicos (salas de reunión, salas de conferencias); se planifican fechas y tiempo de uso.
  - **Equipamiento**: tratado como otras facilidades (ej.: proyector, notebook).
  - **Viáticos**: gastos de representación, refrigerios.
  - **Materiales**: papel, tinta, CDs, DVDs, etc.
- **Personas como recursos**: se asignan por **perfil** y no con nombre y apellido; una vez definido el rol se personaliza y allí aparecen los problemas. Hay pocas herramientas para planificar personas; una es la **Matriz por Perfil** (matriz Actividad-Perfil + matriz Persona-Perfil que se componen).
- **Duración y disponibilidad**: tres variables que influyen en la duración de una tarea: la duración en sí, el esfuerzo de trabajo dedicado (ej.: horas/días de una persona) y el porcentaje de tiempo diario que la persona le dedica a la tarea.
  - Cálculo: `esfuerzo / porcentaje = duración`.
  - El software de administración de proyectos permite cargar 2 variables y calcula la tercera.

### Estimación de Costos
- Predicciones de cuánto tiempo, esfuerzo y perfiles de RRHH se requieren para construir software.
- Suele intercambiarse "estimación de esfuerzo" con "estimación de costos".
- Las estimaciones preliminares son las más difíciles y las menos exactas; en IS somos notoriamente inexactos para calcular tiempo y costo.
- No hay tareas repetitivas (a diferencia de otras profesiones); difieren el dominio de aplicación, hardware, herramientas, técnicas y personal. En IS somos más creadores que constructores.
- **Problemas**:
  - Políticos: cuando las estimaciones se convierten en objetivos; cuando se ajusta el precio por conveniencia.
  - Técnicos: no existen datos históricos para estimar.
- **Usos**:
  - En planificación: saber cuántos recursos va a insumir el proyecto.
  - En control: saber cuánto se hizo y cuánto falta.
- **Proceso**: la estimación de costos comienza a nivel de tarea (costo unitario × duración); una vez determinados los costos de todas las tareas, se agregan a nivel de proyecto. Se separan en **costos laborales** (se calculan por perfil, conociendo el valor horario de cada perfil) y **costos de materiales** (se estiman por precio o por uso).

### Modelo COCOMO
- **COCOMO** = *Constructive Cost Model*; desarrollado en la década del '70 por Boehm; revisado en 1995 y 2000.
- Colección de tres modelos:
  - **Básico**: aplicable cuando se conoce muy poco del proyecto.
  - **Intermedio**: aplicable luego de la especificación de requerimientos.
  - **Avanzado**: aplicable cuando se termina el diseño.
- **Cálculo del esfuerzo**: `PMinicial = c * KLOC^k` (PM en personas-mes; c y k constantes del modelo, k > 1); puede corregirse mediante conductores de costos.
- **Conductores de costos**: atributos del producto, computacionales/hardware, del personal y del proceso.

#### Conductores de costo del COCOMO original (15)
- **Atributos del producto**: RELY (confiabilidad requerida), DATA (tamaño de la base de datos), CPLX (complejidad del producto).
- **Atributos computacionales/hardware**: TIME (restricciones de tiempo de ejecución), STOR (restricciones de almacenamiento), VIRT (volatilidad de la máquina virtual), TURN (tiempo de optimización/respuesta, frecuencia de cambio en el modelo de explotación).
- **Atributos del personal**: ACAP (calificación de los analistas), AEXP (experiencia en la aplicación), PCAP (calificación de los programadores), VEXP (experiencia en la máquina virtual), LEXP (experiencia en el lenguaje).
- **Atributos del proceso/proyecto**: MODP (uso de prácticas modernas de programación), TOOL (uso de herramientas de software), SCED (planificación requerida / limitaciones en el cumplimiento de la planificación).

#### Escala de los conductores
- Escala ordinal de seis puntos: **Muy Baja, Baja, Nominal, Alta, Muy Alta, Extra Alta**.
- De más de 100 factores, Boehm retuvo 15 para COCOMO (agrupados en las 4 categorías anteriores).

#### Pasos básicos de COCOMO
1. Estimar el tamaño del software y usar la fórmula del modelo para estimar el esfuerzo inicial.
2. Revisar la estimación usando conductores de costos u otro factor dado por el modelo.
3. Aplicar las herramientas del modelo al resultado del paso 2 para determinar el esfuerzo total.
- No es sabio confiar ciegamente en los resultados del modelo, pero tampoco ignorar el valor de las herramientas que complementan el juicio experto y la intuición.

#### Fórmula general de esfuerzo
`E = a * S^b * F`
- E: esfuerzo en personas-mes.
- S: tamaño en KDSI (K-delivered source instructions).
- F: factor de ajuste (igual a 1 en el modelo básico).
- a, b: de tablas del modelo según el tipo de sistema.

#### Clasificación de sistemas
- **Orgánicos**: procesamiento de datos, uso de bases de datos, focalizado en transacciones y recuperación de datos (ej.: sistema de facturación).
- **Embebidos**: software de tiempo real, parte integral de un sistema mayor basado en hardware (ej.: control de ascensores).
- **Semi-embebidos**: entre orgánico y embebido, mayor procesamiento de transacciones (ej.: monitoreo de una red).

#### Modelo básico: fórmulas y valores
- `PM = a * (KDSI^b)`
- `TD = c * (PM^d)`

| Tipo | a | b | c | d |
|------|---|---|---|---|
| Orgánico | 2.40 | 1.05 | 2.50 | 0.38 |
| Embebido | 3.00 | 1.12 | 2.50 | 0.35 |
| Semi-embebido | 3.60 | 1.20 | 2.50 | 0.32 |

#### Notas por atributo
- **RELY**: consecuencias para el usuario si hay defectos. Muy baja (inconveniencia de corregir el fallo) → baja (pérdida recuperable) → nominal (pérdida moderada) → alta (gran pérdida financiera o inconveniencia masiva humana) → muy alta (pérdida de vidas humanas).
- **DATA**: tamaño de la base de datos en relación con el tamaño del programa; se define por el cociente D/P (D: tamaño BD en bytes; P: tamaño del programa en DSI). Cuatro segmentos con razón 10-100-1000 determinan puntuaciones de "bajo" a "muy alto".
- **CPLX**: complejidad de cada módulo; de muy baja (expresiones matemáticas simples) a extra alta (módulos con muchos recursos de planificación).
- **TIME**: porcentaje de tiempo de ejecución disponible; nominal al 50% y extra alto al 95%.
- **STOR**: esfuerzo para correr en menor volumen de almacenamiento principal; nominal con reducción del 50%, extra alta con 95%.
- **VIRT**: cambios que puede sufrir la máquina virtual (hardware + software) durante el desarrollo.
- **TURN**: tiempo de respuesta del ordenador desde el punto de vista del programador; mayor respuesta → más esfuerzo. De baja (sistema interactivo) a muy alta (>12 horas de respuesta media).
- **ACAP**: capacidad del grupo de analistas (habilidad de análisis, eficiencia, cooperación); a más capaz, menos esfuerzo.
- **AEXP**: experiencia del grupo en aplicación similar. Muy bajo ≤4 meses; bajo 1 año; nominal 3 años; alto 6 años; muy alto ≥12 años o reimplementación de un subsistema.
- **PCAP**: capacidad del grupo de programadores; similar a ACAP pero para programadores como grupo (no individuales).
- **VEXP**: experiencia en la máquina virtual. Muy bajo <1 mes; bajo 4 meses; nominal 1 año; alto >3 años.
- **LEXP**: experiencia en el lenguaje; más experiencia → menos defectos y requerimientos humanos. De muy bajo (<1 mes) a alto (>3 años).
- **MODP**: uso de prácticas modernas de programación, de "no se utilizan PMP" a "uso habitual de PMP".
- **TOOL**: uso de herramientas de software (multiplicador de productividad), de herramientas básicas (muy bajo) a herramientas específicas (muy alto).
- **SCED**: esfuerzo necesario para cumplir la planificación; el tiempo nominal requiere el menor esfuerzo; apresuramiento (muy bajo) o retraso (muy alto) demandan más esfuerzo.

#### Modelo avanzado y fases
- Para proyectos medios, COCOMO intermedio coincide con el básico.
- El modelo debe calibrarse al propio entorno de desarrollo.
- COCOMO avanzado/detallado: se aplica la versión intermedia a nivel de componentes y luego se construye la estimación para el proyecto completo.
- **Fases de desarrollo** (permite estimar tiempos por fase):
  1. **Requerimientos**: del 6% al 8% del esfuerzo nominal PM; del 10% al 40% del tiempo nominal TD.
  2. **Diseño del producto**: del 16% al 18% del PM; del 19% al 38% del TD.
  3. **Programación** (diseño detallado + prueba del código): del 48% al 68% del PM; del 24% al 64% del TD.
  4. **Prueba/Integración**: del 16% al 34% del PM; del 18% al 34% del TD.

### COCOMO 2.0
- Publicado en 2000 como actualización de COCOMO para adaptarse a nuevas tecnologías y enfoques OO.
- Objetivos: modelos de costos acordes a prácticas actuales; bases de datos y herramientas para mejora continua; un framework analítico cuantitativo y herramientas para evaluar mejoras en costos de ciclo de vida y planificaciones.
- **Tres modelos**:
  1. **Application Composition Model**: apoyo a la estimación en etapas tempranas (escasa información de requerimientos) y prototipos rápidos. Usa **puntos objeto**.
  2. **Early Design Model**: apoyo tras la definición de requerimientos (evaluación de arquitecturas y conceptos de operación alternativos). Usa **puntos función**.
  3. **Post-Architecture Model**: apoyo durante el desarrollo del sistema; más detallado, con nuevos conductores de costo y ecuaciones. Usa **KDSI**.
- **Cálculo de puntos objeto**:
  1. Estimar número de pantallas, reportes y componentes 3GL.
  2. Clasificar cada objeto en complejidad simple, media o alta.
  3. Ponderar según la complejidad (tabla de pesos).
  4. Sumar los pesos → **Puntos Objeto (PO)**.
  5. Estimar porcentaje de reuso y calcular **Nuevos Puntos Objeto (NPO)**: `NPO = PO * (100 - %reuso) / 100`.
  6. Determinar el ratio de productividad: `PROD = NPO / personasMes`.
- **Cálculo de puntos función**:
  1. Contar: inputs externos (IE), outputs externos (OE), consultas externas (CE), archivos internos (AI), archivos de interfaz externos (AE).
  2. Clasificar cada punto función por complejidad (tablas).
  3. Aplicar pesos de complejidad.
  4. Sumar → **puntos función no ajustados (PFNA)**.
  5. Convertir puntos de función a líneas de código según proporciones del lenguaje.
- **Cálculo de esfuerzo en COCOMO II**: `PMnominal = a * (Tamaño)^b` (tamaño en KSLOC).
  - `a`: cuantifica efectos multiplicativos del esfuerzo en proyectos de tamaño creciente.
  - `b`: mide la economía (o no economía) de escala.
    - `b < 1.0`: el proyecto exhibe economía de escala (aumenta la productividad con el tamaño).
    - `b = 1.0`: economía balanceada.
    - `b > 1.0`: no hay economía de escala (aumento de comunicación, problemas de integración).

### Otros modelos
- SLIM (Putnam), DBA COCOMO 2004, COINCOMO 2004, COCOTS 2000, COSYSMO 2002, COSOSIMO 2004, Costing Secure System 2004.

### Problemas con los modelos existentes
- El tamaño del producto es un factor determinante del esfuerzo; la mayoría sugiere que el esfuerzo es aproximadamente proporcional al tamaño.
- Incluyen un ajuste inverso a la economía de escala (proyectos más grandes son menos productivos).
- Modelo de Putnam: disminuir la duración aumenta el esfuerzo; aumentarla lo disminuye.
- Los modelos funcionan bien en el entorno del que fueron derivados; es poco razonable que un modelo simple valga universalmente.
- Son muy sensibles al factor tecnológico (difícil de obtener).
- La mayoría trabaja sobre datos de análisis post hoc.
- Los parámetros de entrada son difíciles de obtener en las primeras etapas.

### Mejoras de las predicciones
- **Datos locales**: medidas de tamaño y esfuerzo definidas consistentemente en todo el entorno.
- **Calibración**: valores consistentes con el modelo; reajustar coeficientes con datos de proyectos pasados; eliminar/agregar/modificar conductores de costos; personalizar el modelo.
- **Grupo de estimación independiente** (propuesta de De Marco): consistencia entre proyectos, mayor experiencia, monitoreo de la base de datos.
- **Reducir subjetividad al input**: los modelos locales basados en datos homogéneos son más exactos que los generales y complejos.
- **Estimación preliminar y re-estimación**: la estimación temprana usa información incompleta; mejorar relacionando ambos pasos.
- **Proceso del grupo de estimación**: el coordinador entrega la información; reunión para preguntas y discusión; cada experto da una estimación inicial anónima; el coordinador circulariza resumen y promedio; nueva reunión; nuevas estimaciones anónimas; se repite hasta que el grupo decide que el promedio es representativo. Putnam propone: `estimacion = (cotaInferior + 4*valoresSimilares + cotaSuperior) / 6`.

---

## 4. Cronograma (Diagramas de Tareas del Proyecto)

- Una vez definidas las tareas (construido el WBS), se decide en qué orden se realizarán.
- Con las tareas y la duración se construye un gráfico que representa el modelo del proyecto, del que se desprenden datos importantes: el tiempo más temprano de comienzo de una tarea y el tiempo más temprano en que puede finalizar el proyecto.
- **Diagrama de red del proyecto**: representación de la secuencia en la que se realizarán las tareas.
- Dos formas de representación:
  1. **Diagrama de Gantt**.
  2. **Diagrama de Red**:
     - **AON** (activity on the node) / PDM (precedence diagramming method).
     - **AOA** (activity on the arrow) / PERT (program evaluation and review technique).

### Diagrama de Gantt
- Desarrollado por Henry L. Gantt como técnica de control de proyectos; sirve para: planificación temporal, presupuestos y planificación de recursos.
- Cuadro de doble entrada; diagrama de barras sobre un eje de tiempo. Cada barra representa una tarea, medio de producción o recurso; su longitud indica el tiempo requerido.
- **Ventajas**: muy sencillo de construir; no requiere herramientas automatizadas específicas.
- **Desventajas**: no contiene información detallada (sólo tareas y fechas de comienzo/fin); no indica cómo terminar anticipadamente el proyecto ni si la asignación de recursos es la más efectiva.
- **Construcción**:
  1. Dibujar ejes: tareas en el vertical, tiempo en el horizontal.
  2. Dibujar los bloques de tareas sin predecesoras (lado izquierdo en el instante 0).
  3. Dibujar los bloques de tareas que sólo dependen de las ya introducidas.
  4. Repetir hasta dibujar todas las tareas.

### AON (Activity on the node)
- La unidad de análisis básica es la tarea: cada tarea es un **rectángulo (nodo)**; las **flechas** representan relaciones predecesoras/sucesoras.
- Para crear el PDM hay que determinar predecesoras y sucesoras de cada tarea ("¿qué tareas deben estar terminadas antes de que pueda comenzar esta?").
- **Construcción del PDM**: se hace siguiendo un orden de secuencia lógico (se lee de izquierda a derecha). Cada tarea (excepto las de comienzo y fin) debe tener al menos una tarea anterior (inmediata predecesora) y una posterior (inmediata sucesora). Una tarea comienza cuando todas sus predecesoras se completan. Son redes conectadas.

#### Dependencias (4 tipos)
- **Fin a Inicio (FI)**: A debe completarse antes que B comience (ej.: codificación del módulo A y testing del módulo A).
- **Inicio a Inicio (II)**: B comienza después de que A comenzó; pueden comenzar juntas o con una diferencia (ej.: codificación del módulo A y generación de datos de prueba del módulo A).
- **Inicio a Fin (IF)**: B no puede terminar antes de que A haya comenzado (ej.: no se puede discontinuar el sistema viejo si el nuevo no comenzó a funcionar).
- **Fin a Fin (FF)**: B no puede terminar antes de que termine A (ej.: el diseño de los módulos no puede terminar hasta que termine el diseño de las interfaces).

#### Restricciones (determinan el tipo de dependencias)
1. **Técnicas**: la tarea sucesora requiere un output de la predecesora. En el caso más simple la predecesora debe completarse antes que comience la sucesora (conviene usar dependencias fin a comienzo). Dentro de esta categoría:
   - **Discrecionales**: juicios del LP que agregan dependencias (p. ej., estrategia de prevención de riesgos).
   - **Por mejores prácticas**: experiencias pasadas documentadas (p. ej., convertir una dependencia fin-comienzo en comienzo-comienzo para acortar tiempos).
   - **Lógicas**: como las discrecionales pero con una justificación razonable sobre cómo organizar actividades.
   - **Requerimiento único**: un recurso crítico necesario para varias actividades; el LP crea dependencias fin-comienzo para evitar conflictos.
2. **Gerenciales**: decisiones políticas de la empresa; a diferencia de las técnicas, pueden ser **revertidas**.
3. **Inter-proyectos**: los entregables de un proyecto son necesarios para otro; surgen en grandes proyectos descompuestos en sub-proyectos.
4. **De fechas**: imponen fechas de comienzo o fin según una planificación. **Deben evitarse** (crean complicaciones innecesarias). Tipos:
   - **No antes que**: fecha más temprana de completamiento (la más leve).
   - **No después de**: fecha límite de completamiento (intermedia).
   - **En esta fecha**: fecha exacta (la más grave).

#### Variable lag
- Pausas o demoras entre tareas. Ej.: "registrar datos de la encuesta comienza 5 días después de enviar las encuestas" → dependencia comienzo-comienzo con lag de 5 días.

#### Planificaciones
- Para establecer la planificación se calculan dos:
  - **Planificación temprana** (estrategia forward): tiempo más temprano en que una actividad puede comenzar y terminar.
  - **Planificación tardía** (estrategia backward): último tiempo en que una actividad puede comenzar y terminar.
- La combinación provee: la **ventana de tiempo** de cada tarea y la **fecha de terminación del proyecto**.
- **Camino crítico**: la secuencia de tareas que determina la fecha de terminación del proyecto.

#### Cálculos de tiempos
- **CMTe (Comienzo Más Temprano)**: tiempo más temprano en que todas las predecesoras están terminadas. Sin predecesoras: se fija en 1 (primer día de trabajo). Con varias predecesoras: `CMTe(p) = max_{predecesor q} {FMTe(q)} + 1`.
- **FMTe (Finalización Más Temprana)**: `FMTe(p) = CMTe(p) + duración(p) - 1`. Ej.: duración 20 días, comienzo día 45 → finaliza el día 64.
- **FMTa (Finalización Más Tardía)**: último tiempo sin causar demoras en el proyecto. `FMTa(p) = min_{sucesor q} {CMTa(q)} - 1`; si no tiene sucesoras coincide con el FMTe.
- **CMTa (Comienzo Más Tardío)**: `CMTa(p) = FMTa(p) - duración(p) + 1`. Ej.: duración 20 días, finalización más tardía día 90 → comienzo más tardío día 71.
- **Ventana de tiempo**: período entre el comienzo más temprano y la finalización más tardía, donde se pueden planificar recursos sin demorar el proyecto. Los tiempos más tardíos se calculan de atrás hacia delante.

#### Camino crítico y margen
- El camino crítico puede definirse como: el camino de duración más larga del diagrama; la secuencia de tareas cuya planificación temprana y tardía es la misma; o la secuencia de tareas con margen cero.
- **Margen (slack)**: demora (en unidades de tiempo) en el comienzo o fin de una tarea que puede tolerarse sin demorar la finalización del proyecto. `margen(p) = FMTa(p) - FMTe(p)`.
  - **Margen total**: rango de fechas en que una tarea puede terminar sin demorar la fecha de terminación del proyecto.
  - **Margen libre**: rango de fechas en que una tarea puede terminar sin causar demoras en la planificación más temprana de sus inmediatas sucesoras.
- **Cálculo del camino crítico**: sumar duraciones por todos los caminos posibles (útil en proyectos pequeños); en proyectos grandes se trabaja con márgenes: las tareas con **margen cero** determinan el camino crítico.
- Toda demora en una tarea del camino crítico demora la terminación del proyecto en esa misma cantidad. Las tareas del camino crítico deben realizarse en su planificación más temprana o el proyecto se atrasará.

#### Análisis del modelo inicial (compresión)
- Generalmente los cálculos iniciales dan una fecha de finalización fuera de las fechas requeridas → se debe reducir la duración total del proyecto.
- Se estudia el modelo para identificar áreas de compresión: buscar pares de tareas secuenciales que puedan ejecutarse en paralelo; la sucesora puede comenzar con cierto grado de avance de la predecesora.
- Hacer disponibles los entregables de la predecesora puede **aumentar los riesgos** (posible trabajo a rehacer).
- La compresión afecta el marco de tiempo, no la cantidad de trabajo; exige mayor coordinación y comunicación en las tareas afectadas.
- Se focaliza en el camino crítico (generalmente se busca en las primeras tareas, aunque no es aconsejable porque el grupo recién comienza a funcionar); otra alternativa es buscar tareas **particionables**.
- Si se cambia la secuencia, el camino crítico puede modificarse (si se reduce su duración).

#### Reserva gerencial
- Se agrega una tarea final llamada **reserva gerencial**: entre un **5% y 10%** de la duración total del proyecto según sus características.
- Se debe administrar el proyecto para no necesitarla; sirve de motivación al equipo (puede acortarse según haga falta) y es útil con contratos rígidos de cumplimiento de fechas.

### AOA (Activity on the arrow) y PERT
- **Características AOA**: cada **flecha** representa una tarea; el nodo izquierdo es el evento/hito de comienzo y el derecho el de fin. Inicialmente los nodos se numeraban secuencialmente (se debía preservar el orden). Se pueden agregar **tareas fantasmas** para preservar la integridad de la red. No es muy usado actualmente.
- **PERT**: *Program Evaluation and Review Technique*.
  - Hipótesis: el proyecto se divide en tareas; una tarea tiene nombre, duración y tareas previas.
  - Grafo orientado: los **vectores (flechas)** representan las tareas (AOA) y los **vértices** representan los sucesos que marcan el inicio/fin de las tareas.
  - **Condiciones de representación**: si es necesario se introduce una actividad final (sucesora de todas las que no tienen sucesores) y una actividad inicial (predecesora de todas las que no tienen predecesores). **Entre dos vértices no puede haber más de un vector**; si dos tareas comparten inicio y fin, se introduce una **tarea ficticia de duración nula**.
  - **Valoración de nodos**: las tareas no condicionadas reciben valor 0 en el vértice inicial; los demás vértices se valoran examinando todos los valores que llegan: `valorVertice = valorVerticePrecedente + duracionTarea`, tomando el **mayor valor**.
  - **Camino crítico en PERT**: el camino que permite alcanzar el valor del último vértice (ej.: tareas A, F y E).

---

## 5. Propuesta de Proyecto

- Entregable de la JPPS; se envía a los **gerentes senior** para su aprobación.
- Establece la descripción completa de la **oportunidad de negocio** del proyecto.
- Incluye: valor de negocio esperado, costos, cronogramas, planes de riesgos y otros apéndices.
- Se esperan varias revisiones antes de la aprobación.

### Posible estructura
- **Resumen ejecutivo**: muy corto; situación del negocio, objetivo del proyecto y su valor de negocio (contenido expandido del POS).
- **Antecedentes**: breve descripción de la situación que motivó el proyecto (condiciones, problemas, oportunidades).
- **Objetivos**: qué se espera obtener del proyecto.
- **Estrategia**: descripción breve de las tareas (modelo de PMLC) a usar, para quienes no están interesados en los detalles.
- **Descripción Detallada del Trabajo**: resumen de alto nivel de qué se hará, cuándo y quién, cuánto tiempo demandará y criterios de completitud; los diagramas de Gantt son útiles aquí.
- **Resumen de Tiempos y Costos**: tabla resumen con tiempos y costos de las actividades.
- **Apéndices**: todos los datos de soporte, anticipando preguntas de los revisores y sus respuestas.

### Obteniendo la aprobación
- La propuesta debe convencer de que el proyecto es una buena oportunidad de negocio y que los recursos están en línea con esa oportunidad.
- Motivos de revisión y respuestas:
  - **El costo/beneficio no está a favor**: descomponer la solución y estimar los beneficios por funciones; posiblemente eliminar funciones con poco beneficio o mucho costo.
  - **Riesgos de fracaso altos**: tratar de eliminar los riesgos buscando otras soluciones.
  - **El costo excede la posibilidad de financiamiento**: analizar el triángulo de alcance o descomponer el proyecto en fases.
  - **Otros proyectos compiten por los mismos recursos**: quizás sea tiempo de presionar a los "sponsors" en la política de la organización.