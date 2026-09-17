# Resumen de Estudio — Proyectos de Sistemas de Software (PSS)

> Resumen de la teoría de los PDFs de cátedra: **01 - Introducción a Proyectos** y **02 - Concepción.**

---

## 1. INTRODUCCIÓN A PROYECTOS (PDF 1)

Autores: E. Estévez – P. Fillottrani. Cinco bloques: **Definición, Clasificación, Administración, Etapas/Ciclos de Vida, Atributos Críticos.**

### 1.1 Definición
- Un **proyecto** = **secuencia de actividades** con un propósito que debe completarse:
  - en un **tiempo determinado**, dentro de un **presupuesto**, de acuerdo a una **especificación**.
- Cualquier actividad que dé como resultado un **producto o "entregable"**.
- Comienza con el **enunciado de un problema**.
- **Evaluación de un proyecto:** ¿soluciona el producto el problema del usuario? ¿está satisfecho el usuario con el proceso? ¿la gerencia con el producto/proceso? ¿el equipo de desarrollo satisfecho?

#### Características de un proyecto
- **Secuencia de actividades**, **únicas** (nunca repetidas), **complejas** (no repetitivas), **conectadas** (dependencia lógica/técnica).
- **Propósito simple** (los grandes pueden dividirse en subproyectos).
- **En tiempo y presupuesto** (restringido), y de acuerdo a una **especificación**.

#### Ambiente actual de desarrollo
- **Alta velocidad**, **alto cambio**, **bajos costos**, **altos niveles de complejidad**, **alta incertidumbre**.

#### Desafíos para la administración
- **Flexibilidad y adaptabilidad**, **comprensión del negocio y sus sistemas**, **hacerse cargo del proyecto**.

### 1.2 Parámetros de ejecución (Triángulo de Alcance)
- **Ámbito** (qué se hace y qué no), **Calidad** (producto y proceso), **Costo** (presupuesto), **Tiempo** (ventana de finalización), **Recursos** (consumibles; pueden ser fijos y limitados).
- Triángulo clásico: **calidad, costo, tiempo** — se mantiene el **equilibrio** entre ellos.
- El balance permite al administrador **escalar problemas** y es la base para **definir el impacto de los cambios**.
- Los proyectos son **sistemas dinámicos**; **cualquier imprevisto desbalancea el proyecto**.
- **Quién controla cada parámetro:**
  - **LP (Líder de Proyecto):** utilización de recursos, cronograma de trabajo.
  - **Gerente:** niveles de recursos, costos.
  - **Cliente:** alcance, niveles de calidad, fechas de entrega.

### 1.3 Corrimientos (desviaciones típicas)
- **De alcance:** cualquier cambio que no estaba en el plan original. El LP debe acomodar el proyecto.
- **De esperanza:** informar que no hay demoras para no dar una mala noticia, pensando recuperarse después. El LP debe controlar si los informes son veraces (controles aleatorios).
- **De esfuerzo:** el trabajo del equipo no representa progresos proporcionales (siempre se avanza pero nunca se termina).
- **De rasgos:** miembros agregan arbitrariamente rasgos que el usuario **no especificó** (costos adicionales: pruebas, datos, documentación, entrenamiento).

### 1.4 Evaluación de proyectos
- Un proyecto puede ser **exitoso** o **fracasar** en tres momentos: **al comienzo**, **durante el desarrollo** o **al final**.
- **Éxito:** claro comienzo/plan detallado; criterios de medición aceptables; monitoreo cercano; documentación clara con revisiones frecuentes; procedimientos de detección de problemas; costo cercano al estimado.
- **Fracaso al comienzo:** sin planificación ("no despegan", avanzan al 90% y se quedan ahí). *Planificar* = saber a dónde se va, cómo llegar y cómo probar que se está ahí.
- **Fracasos durante:** análisis/diseño mal documentados, responsabilidades confusas, falta de planificación, codificación prematura, falta de revisiones y walk-through, falta de estándares, deserciones, "fuerza bruta".
- **Fracasos al final:** entregas sin suficientes pruebas, sin performance, altos costos de mantenimiento, **cancelación** (falta de fondos, cambios de contexto, deserción de elementos clave, desastre técnico).

### 1.5 Clasificación de proyectos
- **Cada proyecto es único** → no existe un esquema único de administración. Se definen políticas por **grupos con características comunes**.
- **Criterios de clasificación:** riesgo, valor para el negocio, duración, complejidad, tecnologías usadas, departamentos afectados, costo.

#### Tabla de categorías
| Tipo | Duración | Riesgos | Complejidad | Tecnologías | Complicaciones |
|------|----------|---------|-------------|-------------|----------------|
| **A** | > 18 meses | alto | alto | de avanzada | seguro |
| **B** | 9–18 meses | medio | medio | actual | alta probabilidad |
| **C** | 3–9 meses | bajo | bajo | buena | alguna probabilidad |
| **D** | < 3 meses | muy bajo | muy bajo | práctica | ninguna |

- **Tipo A:** alto valor de negocio y complejidad; la organización debe asignar **todos los recursos** (ej: nueva tecnología en un producto muy beneficioso).
- **Tipo B:** significativos pero más cortos; tecnológicamente desafiantes; muchos recursos (ej: muchos desarrollos de productos).
- **Tipo C:** muy frecuentes, cortos, tecnologías establecidas (ej: equipo de 5, hasta 6 meses).
- **Tipo D:** apenas "proyectos"; poca documentación y cronograma básico (cambios menores).

#### Uso de procesos según tipo (**R** = requerido, **O** = opcional)
| Etapa / Proceso | A | B | C | D |
|-----------------|---|---|---|---|
| **Concepción** — Condiciones de satisfacción | R | R | O | O |
| **Concepción** — POS | R | R | R | R |
| **Concepción** — Aprobación del pedido | R | R | R | R |
| **Planificación** — Sesión de planificación | R | R | O | O |
| **Planificación** — Propuesta de proyecto | R | R | R | R |
| **Planificación** — Aprobación de propuesta | R | R | R | R |
| **Lanzamiento** — Reunión kick-off | R | R | O | O |
| **Lanzamiento** — Cronograma de actividades | R | R | R | R |
| **Lanzamiento** — Asignación de recursos | R | R | R | O |
| **Lanzamiento** — Definición de trabajo | R | O | O | O |
| **Monitoreo** — Reporte de estado | R | R | R | R |
| **Monitoreo** — Reuniones de equipo | R | R | O | O |
| **Monitoreo** — Aprobación de entregables | R | R | R | R |
| **Cierre** — Auditoría post-implementación | R | R | R | R |
| **Cierre** — Notas del proyecto | R | R | O | O |

### 1.6 Administración de Proyectos
- **PMI:** aplicación de conocimientos, habilidades, herramientas y técnicas a las actividades para satisfacer los requerimientos del proyecto.
- **Objetivo de la Administración de Proyectos de Software:** aplicar buenos principios de administración e ingeniería de software para entregar el producto a **mínimo costo, mínimo tiempo y con buena calidad**.
- **Datos de relevancia (2016):**
  - Menos de **1/3** de los proyectos se terminan a tiempo y dentro del presupuesto.
  - Por cada **U$S 1000 millones** invertidos en EEUU, **U$S 122 millones (12,2%)** se pierden por falta de rendimiento.
  - **71%** alcanza los objetivos cuando la cultura de administración de proyectos es de **alta prioridad**.
- **Desafíos:** innovación, complejidad, requerimientos ambiguos, falta de competencias, herramientas inmaduras, regulaciones, plazos, proveedores, retención de personal, equipos multiculturales/multilingües y distribuidos.
- **Principios:**
  - Todos los **atributos críticos** se deben especificar claramente.
  - El diseño debe satisfacer **todos** los atributos críticos **simultáneamente**.
  - Especificar en términos **testeables y medibles**, identificando el **peor caso**.
  - **Nunca** entregar grandes sistemas complejos en **"big-bang"**.
  - No creer ciegamente en métodos; usar el propio y el **sentido común**.
  - *"Si no se sabe lo que se está haciendo, no hacerlo en gran escala."*

### 1.7 Etapas y ciclos de vida
- Para planificar/controlar hay que **descomponer** en partes pequeñas y manejables → en **partes componentes** y **trabajo a realizar**.
- Se descomponen en **fases de tiempo** (primero esto, luego lo otro) que producen **uno o más hitos**.

#### Hitos (milestones)
- Un **hito** = evento que **prueba claramente que una etapa se concluyó satisfactoriamente**.
- Ejemplos: entrega del documento de requerimientos, de la especificación del sistema, del diseño de la interfaz, del documento de diseño de tests, del código fuente, y el **deploy** del sistema.

#### Procesos típicos (5 etapas)
1. **Concepción** (scoping): definir **qué se hará** (no incluye realización). Incluye establecer los **criterios de éxito**. Tareas: reclutar el LP; obtener las reales necesidades del cliente; documentarlas; negociar cómo se cubrirán; escribir el **POS**; ganar la aprobación para planificar.
2. **Planificación:** definir **cómo se hará**. Tareas: definir el trabajo; estimar tiempo, recursos y costo; secuenciar el trabajo; desarrollar el cronograma inicial; escribir un **plan de contención de riesgos**; documentar el plan; ganar la aprobación para **lanzar**.
3. **Lanzamiento:** acciones **preparatorias para la ejecución**. Tareas: reclutar el equipo; emitir la descripción del proyecto; establecer reglas del equipo; establecer el **proceso de cambio de alcance**; administrar comunicaciones; terminar el cronograma; describir **paquetes de trabajo**.
4. **Monitoreo y Control:** acciones de **ejecución**. Establecer performance y reportes; monitorear riesgos; reportar el estado; procesar requerimientos de cambio de alcance; descubrir y resolver problemas.
5. **Finalización / Cierre:** acciones de **evaluación**. Aprobación del cliente del cumplimiento de metas; instalar entregables; reporte final; **auditoría post-implementación**.

#### Ciclos de vida (variaciones)
- Solo concepción/planificación/lanzamiento → para 1-2 personas, como lista de tareas.
- + control → el lanzamiento es solo el 50%; el control **anticipa problemas**.
- + cierre → el LP **aprende de la experiencia**.

### 1.8 Atributos Críticos
- **Atributo crítico** = una **calidad o recurso** que puede causar que el sistema **colapse si supera determinados límites** (el **peor caso aceptable**).
- Ejemplos: **performance de la operativa diaria**; **habilidad para incorporar nuevas unidades de negocio**.
- **Ejemplo 1 — Capacidad de trabajo:** requisito: suficiente para la operación diaria normal.
  - **Peor caso:** 4 segundos promedio por transacción.
  - **Nivel planificado (inicial):** menos de 1 segundo por transacción.
  - **Nivel planificado (si >100.000 transacciones diarias):** 0,2 segundos por transacción.
  - **Mejor caso:** 0,1 segundo por transacción.
  - **Lección:** como no se especificó como requerimiento formal, nadie se preocupó → el sistema colapsó.
- **Ejemplo 2 — Adaptabilidad:** integrar nuevas unidades de negocio sin retraso.
  - **Peor caso:** integrar una nueva unidad en **6 meses** y con esfuerzo máximo de **10 programadores/analistas o 5 años-hombre**.
  - **Nivel planificado:** agregar/eliminar unidades en **menos de 6 meses** de esfuerzo calificado.

---

## 2. CONCEPCIÓN DE PROYECTOS (PDF 2)

Herramientas de la fase de concepción: **COS**, **POS**, reuniones de definición, especificación de requerimientos, diagramación de procesos, prototipos, validación de casos de uso, administración de la provisión/outsourcing, y **aprobación para la planificación**.

### 2.1 Condiciones de Satisfacción (COS)
- Los clientes suelen esperar más de lo que el LP está preparado para entregar → **falla de comunicación** (el LP asume que entiende lo que el cliente pide; el cliente asume que eso es lo que necesita). **Estas suposiciones no se chequean.**
- El **LP es responsable de clarificar** las diferencias lo antes posible, preguntando al cliente *por qué* quiere lo que quiere.
- **Nunca empezar un proyecto sin estar seguro de que la solución satisface realmente al cliente.**
- **COS** (*Conditions of Satisfaction*) = **conversación estructurada** entre el cliente (requiriente) y el probable LP (proveedor). Su **entregable** es el **POS** (una página, quizá con adjuntos). **Ambos firman el POS.**
- La concepción se considera **concluida cuando el POS es aprobado por un gerente senior**.
- **COS** se adapta mejor a proyectos **pequeños y medianos**; en grandes, usar métodos más formales.

#### Proceso del COS (4 etapas)
1. **Requerimiento:** el requiriente hace un requerimiento.
2. **Clarificación:** el proveedor explica qué entendió; se establece el entendimiento **en el lenguaje del requiriente**.
3. **Respuesta:** el proveedor establece qué es capaz de proveer.
4. **Acuerdo:** el requiriente describe qué entendió sobre lo que el proveedor ofrecerá.
> La conversación continúa hasta que el proveedor comprende que el requiriente entendió lo que será provisto. Probablemente **no se llegue a un acuerdo en la primera fase**.

- **Criterios de éxito:** métricas **cuantitativas** que demuestran que el COS fue satisfecho. El COS es **dinámico** y puede revisarse.

### 2.2 Project Overview Statement (POS)
- Documento **corto** que especifica de forma concisa: **qué** se va a hacer, **por qué**, y **qué valor comercial** tendrá.
- Sirve para que la **gerencia apruebe el proyecto** y **autorice recursos**. También como base/referencia para la planificación y para solicitud de iniciativas.

#### Plantilla del POS
1. Nombre del Proyecto
2. Nombre del Equipo / Líderes del Proyecto
3. **Problema/Oportunidad**
4. **Metas**
5. **Objetivos**
6. **Criterios de Éxito**
7. **Suposiciones, Riesgos, Obstáculos**
8. Preparado por / Fecha — Aprobado por / Fecha

#### Metas
- Dan idea del **valor** del proyecto (para que la alta gerencia decida seguir leyendo). Dan **propósito y dirección**; definen el resultado final. Descripción **corta y concisa**; no necesariamente con fechas.

#### Objetivos — criterios **SMART**
- **Específicos** (concretos), **Medibles** (indicador de progreso), **Asignables** (a una persona), **Realistas** (con los recursos disponibles), **Limitados en el tiempo** (duración).
- Son una **descomposición detallada de la meta**; conjunto de objetivos **necesarios y suficientes** (ninguno superfluo).
- **Enunciado de un objetivo (4 elementos):** 1) **Salida** (qué se va a realizar), 2) **Marco de tiempo** (fecha esperada), 3) **Medida** (métricas de éxito), 4) **Acción** (cómo se logrará).

#### Factores Críticos de Éxito (FCE)
- Guía: *"¿qué debiera sucedernos a nosotros y al cliente para decir que el proyecto fue un éxito?"*
- Base para que la **alta gerencia autorice los recursos** para la planificación detallada.
- Deben ser **medibles y cuantificables**, preferentemente **en términos del negocio**. Se busca **vender la idea** a los *decision-makers*.

### 2.3 Requerimientos y Soluciones
- **Requerimiento** = una **función** que el sistema debe realizar, una **característica deseada**, o un **enunciado sobre el sistema propuesto** que los stakeholders acuerdan que debe satisfacerse para solucionar el problema del cliente.
- **Proceso de requerimientos (5 actividades, NO lineal):** elicitación, especificación, modelamiento/análisis, validación y administración.
- **Requerimiento funcional:** describe interacción sistema-entorno; *está presente o ausente* (binario, sin grado).
- **Requerimiento no funcional:** describe **restricciones** del sistema; tiene **escala de demanda** y posibles negociaciones (performance, etc.).
- **Estándares:** IEEE Guide P1233/D3, IEEE Std. 1233, IEEE Std. 830-1998, ISO/IEC 12119-1994, IEEE std 1362-1998 (ConOps).

#### Soluciones
- Una **solución** = conjunto de ideas cuya implementación **impacta positivamente** en al menos una parte del problema. *Una idea sin efectos positivos en los requerimientos no es una solución.*
- **Una solución es válida en la medida que mejor sirva a los requerimientos actuales.**
- **Búsqueda:** las **funciones determinan los requerimientos de interés** (empezar por los funcionales), y los **atributos determinan las soluciones técnicas**.

#### Cómo evaluar una solución (requisitos)
1. Especificar los requerimientos conocidos de forma **clara y precisa**.
2. Conocer **todas las contribuciones positivas** de la solución a los requerimientos de calidad.
3. Conocer cómo impactan **todos los efectos colaterales negativos**.
4. Conocer **todo el consumo de recursos** en relación al presupuesto.

#### Requerimientos vs. Soluciones
- Requerimiento **funcional** = absoluto (verdadero/falso). No funcional = escala de medición. **Solución** = idea que impacta en los requerimientos.
- ⚠️ **Cuidado:** que una solución **no se transforme en un requerimiento**.
- **Flexibilidad:** una solución puede especificarse como requerimiento funcional solo si tiene prioridad mayor a un no funcional que afecta negativamente; puede haber soluciones *non-sancta* (sujetas a cambios).

#### Quiénes proponen las soluciones (**roles**, no puestos formales)
- **Gerentes:** enuncian sus problemas en términos de objetivos.
- **Problem solvers:** encuentran las soluciones adecuadas. Son procesos separados.

#### Estimación y comparación de soluciones
- Más de una solución puede impactar en un atributo y viceversa; algún atributo puede no tener solución → revisar objetivos.
- **Estimación de impacto:** cuánto contribuye una solución a los atributos requeridos; se expresa como **estimación o rango de valores** y se arma una **tabla de estimación de impacto**.
- **Beneficios de cuantificar:** discutir con el responsable, base para aprender a estimar, motivación, discusión profesional, clarificar objetivos.
- **Comparación de soluciones:** técnica escrita, numérica y tabular. La mejor solución = mayor **impacto positivo** en los atributos. Se puede **sumar algebraicamente los efectos** (mayor suma en **calidad** = mejor; menor suma en **recursos** = mejor). **Razón de impactos = Σ impactos de calidad / Σ impactos de recursos**.

#### Proceso para encontrar soluciones (7 pasos)
1. Concentrarse en **un atributo por vez** y hacer **lluvia de ideas** para plantear soluciones.
2. **Estimar efectos colaterales** (tabla de estimación de impacto) en los otros atributos.
3. **Eliminar soluciones** que produzcan el peor caso en algún atributo.
4. Repetir hasta encontrar todos los niveles planificados o no encontrar más.
5. Si se encontraron los niveles planificados → paso 7.
6. Si no hay más soluciones: buscar más experiencia de diseño (volver al paso 1) **o** modificar/negociar los niveles planificados.
7. **Testear las hipótesis de diseño** (inspección de Fagan, entregas parciales, medición).

#### Especificación e identificación de soluciones
- Mantenerlas **resumidas**, lo más **precisas (no ambiguas)** posibles; poner ideas nuevas en enunciados nuevos.
- Toda idea de solución debería tener una **etiqueta de identificación única** (numérica o mnemotécnica, jerárquica, temporal) para tablas de evaluación y gestión de configuración/versiones.

#### Método de Inspección de Fagan
- Inspecciones en puntos prefijados del proceso; se inspeccionan **todas las clases de defectos** de la documentación.
- Las realizan **colegas de todos los niveles excepto el gerente**, con **roles específicos**, guiados por un **moderador entrenado** y **checklists de preguntas**.
- **Reuniones de revisión limitadas a 2 horas.**

### 2.4 Riesgos
> *"Si no atacamos activamente a los riesgos, ellos nos atacarán a nosotros."*

- **Principio de compartir el riesgo:** el verdadero profesional conoce los riesgos, sus niveles, causas y acciones de control, y los comparte con colegas y clientes.
- **La prevención del riesgo es más efectiva en costo que la detección.**
- Al indicar desviaciones, indicar **causas** y **acciones de control**. El grado de riesgo y sus causas **nunca deben ocultarse** de los *decision-makers*.

#### Estrategias
- **Reactiva** ("escuela Indiana Jones"): *"no te preocupes, pensaré en algo"*; a lo sumo supervisa.
- **Proactiva:** comienza **antes** del trabajo técnico; se **identifican** riesgos, se **valoran** probabilidad e impacto, se **priorizan** y se establece un **plan de control**.

#### Riesgos del software
- Medir: **incertidumbre** (probabilidad de que ocurra) y **pérdida** (consecuencias no deseadas).

#### Clasificación
- **Del proyecto:** amenazan el plan del proyecto.
- **Técnicos:** amenazan la **calidad y la planificación temporal**.
- **Del negocio:** amenazan la **viabilidad**:
  - **Mercado:** el producto es bueno pero nadie lo quiere.
  - **Estratégico:** no encaja en la estrategia comercial.
  - **Ventas:** el depto. de ventas no sabe cómo venderlo.
  - **Dirección:** pérdida de apoyo de gestión (cambios de enfoque/personal).
  - **Presupuesto:** pérdida de presupuesto o personal.
- **Charette:** **conocidos** (evaluando el plan/entorno), **predecibles** (por experiencia de proyectos previos), **impredecibles** (difíciles de prever).

#### Identificación
- Intento **sistemático** de especificar las amenazas al plan. **Genéricos** (a todos los proyectos) vs. **específicos** (del producto). Se crea una **lista de comprobación de elementos de riesgo**.

#### Lista de comprobación (7 categorías)
1. **Tamaño del producto** (LDC/PF, seguridad de la estimación, bases de datos, transacciones, usuarios, cambios previstos, software reutilizado).
2. **Impacto en el negocio** (ingresos, viabilidad, fecha límite, clientes, interoperatividad, sofisticación del usuario, documentación, regulaciones, costos de retraso).
3. **Características del cliente** (¿trabajó antes?, ¿tiene idea escrita?, ¿gastará tiempo en reuniones?, ¿buena comunicación?, ¿participa en revisiones?, ¿entiende el proceso?).
4. **Definición del proceso** (¿proceso estándar?, ¿documentación?, ¿personal de acuerdo?, ¿revisiones formales?, ¿control de cambios?, ¿estándares? + aspectos técnicos: métodos de diseño, casos de prueba, herramientas, métricas de calidad/productividad).
5. **Entorno de desarrollo** (herramientas de análisis/diseño/gestión, BD, expertos, ayuda en línea, integración de herramientas).
6. **Tecnología a construir** (¿nueva?, ¿algoritmos/interfaces especiales?, ¿hardware/software no probado?, ¿métodos no convencionales?).
7. **Tamaño y experiencia del grupo** (¿la mejor gente?, ¿suficiente y con conocimientos?, ¿rotación?, ¿expectativas correctas?, ¿formación?).

#### Componentes del riesgo
- **Rendimiento** (¿resuelve los requerimientos?), **Costo** (¿presupuesto?), **Soporte** (¿se puede corregir/adaptar/mejorar?), **Planificación temporal** (¿a tiempo?).

#### Proyección del riesgo (4 actividades del equipo)
1. Establecer una **escala** de probabilidad.
2. Definir las **consecuencias**.
3. **Estimar el impacto** en proceso y producto.
4. **Anotar la exactitud** de la proyección.
- El impacto se divide en **4 categorías:** despreciable, marginal, crítico, catastrófico.

#### Tabla de Riesgos
- Columnas: **riesgos, categoría, probabilidad (media), impacto**.
- Se **ordena por probabilidad e impacto** y se determina un **nivel de corte**.
- Riesgos **por encima del corte** reciben un **PRSGR**.
- **Consideración:** gran impacto + poca probabilidad → poca gestión; gran impacto + probabilidad moderada, o impacto medio + probabilidad alta → requieren gestión.

#### Evaluación del impacto (si ocurre)
- Tres factores: **naturaleza** (problemas que aparecerán), **alcance** (severidad × distribución), **cuándo ocurre** (cuándo y por cuánto tiempo). La tabla debe **evaluarse periódicamente**.

#### Análisis del riesgo (matriz de colores)
- Probabilidad y magnitud del daño: 1) insignificante/nula, 2) baja, 3) media, 4) alta.
- Rangos: **Bajo riesgo = 1–6 (verde)**, **Medio = 8–9 (amarillo)**, **Alto = 12–16 (rojo)**.

#### Estrategias y gestión del riesgo
- Estrategia eficaz: **evitar**, **supervisar**, y **gestión del riesgo/planes de contingencia**.
- **PRSGR** (Plan de Reducción, Supervisión y Gestión del Riesgo): tareas proactivas para reducir la probabilidad. Si la reducción fracasa, la **gestión y contingencia** asumen que el riesgo se hizo realidad.
- Cada paso del PRSGR **aumenta costos**; evaluar cuándo los costos superan los beneficios.
- En grandes proyectos se identifican **30–40 riesgos** → aplicar **regla de Pareto 80-20**.

#### Regla de Pareto (80-20)
- 80% del tiempo se consume en el 20% de las tareas; 80% del trabajo lo hace el 20% de las personas; 80% de la frustración se debe al 20% de los problemas; 80% de los problemas se soluciona con el 20% del código.

#### Estimación de riesgos
- Importa la **confianza**, no los números. Formas: expresar una **desviación**, varios **niveles del atributo** (peor caso, planificado, actual), una **probabilidad**, o **listar los factores** de variación.
- **Exposición al riesgo (ER) = probabilidad × costo.** Puede usarse para ajustar costos y asegurar riesgos.

#### PRSGR
- Documenta el análisis de riesgos y acompaña el plan global del proyecto. Consiste en: **evitar** el problema (mitigando causas), **valorar** si los riesgos ocurren (monitorear probabilidad), asegurar el **cumplimiento de los pasos de reducción**, y **recopilar información** para futuros proyectos.

### 2.5 Aprobación para la planificación
- Tras completar el POS, se envía **con sus adjuntos a los gerentes senior** para aprobación.
- La aprobación **no es un proceso formal**; implica que el proyecto **tiene valor** y que su definición es precisa, y determina **asignar recursos para planificar en detalle**.
- Puede haber **varias iteraciones** (los gerentes piden aclaraciones).
- El POS debe intentar ser **auto-explicativo**.
- La aprobación sirve a **3 audiencias:** **alta gerencia** (dedicar recursos), **cliente** (proyecto claramente definido), **equipo** (el proyecto es claro para ambos).
- Es una **aprobación para confeccionar el plan detallado**. La **aprobación definitiva del proyecto** ocurre tras analizar el plan detallado.

#### Participantes (equipo principal)
- **LP**, **gerentes de usuarios** (recursos), **gerentes de procesos/funciones** (contexto), **cliente** (puede ser hasta LP), **alta gerencia** (soporte crítico). Algunos son potenciales integrantes del equipo de desarrollo.

#### Aclaraciones esperadas del POS (preguntas típicas)
- ¿Importancia del problema/oportunidad? ¿Relación con los **FCE**? ¿La meta se relaciona con el problema? ¿Los objetivos representan la meta? ¿El valor justifica gastos? ¿Relación objetivos–FCE? ¿Pueden los gerentes mitigar la exposición a los riesgos?

#### Posibles resultados del POS
- **Aprobado** o **desaprobado** (con variantes):
  - **Rechazado:** sin oportunidad de realizarse.
  - **Reformulación:** redefinir meta/objetivos según nuevas expectativas; puede re-enviarse.
  - **Postergado:** la decisión no puede tomarse ahora.
  - **Derivado a un portafolio** de proyectos.

---

## 3. CHEAT-SHEET / REPASO RÁPIDO

- **COS** = conversación estructurada (requerimiento → clarificación → respuesta → acuerdo), entregable = **POS**.
- **POS** = documento de una página (qué, por qué, valor comercial) con plantilla: Problema/Oportunidad, Metas, Objetivos (SMART), Criterios de Éxito, Suposiciones/Riesgos/Obstáculos.
- **Metas** = finalidad. **Objetivos** = hitos medibles con tiempo. **Criterios de éxito** = hitos del éxito (no siempre ligados a la meta).
- **Requerimientos funcionales** (binarios) vs **no funcionales** (en escala). ⚠️ Que una **solución** no se vuelva un requerimiento.
- **Triángulo/Parámetros:** ámbito, calidad, costo, tiempo, recursos. Balance para escalar problemas.
- **Corrimientos:** alcance, esperanza, esfuerzo, rasgos.
- **Hitos** = evento que prueba la conclusión de una etapa.
- **Ciclo de vida:** Concepción → Planificación → Lanzamiento → Monitoreo y Control → Cierre.
- **Categorías de proyectos A/B/C/D** según duración/riesgo/complejidad/tecnología.
- **Atributo crítico:** calidad/recurso cuyo peor caso (si se supera) colapsa el sistema; debe ser testeable, medible y con peor caso definido.
- **Clasificación de riesgos:** proyecto / técnico / negocio (mercado, estratégico, ventas, dirección, presupuesto).
- **Proyección:** escala → consecuencias → impacto → exactitud. **Tabla de riesgo** ordenada con nivel de corte.
- **Matriz de riesgo:** bajo = 1–6 (verde), medio = 8–9 (amarillo), alto = 12–16 (rojo).
- **ER = probabilidad × costo.** **PRSGR** para riesgos por encima del corte. **Pareto 80-20.**
- **Aprobación del POS** → habilita la planificación detallada (3 audiencias: alta gerencia, cliente, equipo).
