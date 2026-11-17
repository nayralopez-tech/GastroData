# GastroData
### Digitalización, gestión y análisis de negocio para hostelería

GastroData es un proyecto de portfolio que explora la aplicación de herramientas digitales y análisis de datos a situaciones habituales del sector de la restauración. Nace de mi experiencia en hostelería y busca conectar la gestión operativa de un establecimiento con el control de costes, el análisis de información y la experiencia del cliente.

> **Proyecto demostrativo con datos ficticios y simulados.** Los ingredientes, precios y resultados económicos se utilizan para mostrar la lógica del proyecto; no representan tarifas actuales ni datos de un establecimiento real.

## Estructura del proyecto

GastroData se organiza en tres módulos complementarios:

### 01. Gestión de costes y escandallos
Desarrollo de fichas de recetas y subrecetas en Excel para calcular costes, estudiar márgenes y simular precios de venta.

- Fichas de recetas y subrecetas.
- Selección de ingredientes mediante listas vinculadas a la hoja Inventario.
- Cálculo de costes por elaboración y por ración.
- Márgenes predeterminados por categoría y margen objetivo configurable.
- Identificación automatizada de alérgenos.

**Tecnologías:** Excel y VBA.

### 02. Análisis de datos y Business Intelligence
Preparación y análisis de información del negocio hostelero para convertir los datos operativos en indicadores útiles para la toma de decisiones.

- Preparación y transformación de datos.
- Diseño de modelos de datos.
- Construcción de indicadores (KPIs).
- Dashboards interactivos y análisis del rendimiento.

**Tecnologías:** Power Query y Power BI.

### 03. Carta digital y gestión de alérgenos
Carta digital accesible mediante código QR, orientada a facilitar la consulta de platos y la identificación de alérgenos.

- Consulta digital de la oferta gastronómica.
- Información de alérgenos por plato.
- Acceso mediante código QR.
- Presentación de información orientada al cliente.

**Tecnologías:** HTML, CSS y JavaScript.

---

## Primera entrega: fichas de receta en Excel

La primera entrega documenta dos fichas relacionadas: una receta principal y la subreceta que utiliza.

- **REC001 — Ensalada César con pollo:** escandallo de una ración, coste de ingredientes y uso de 40 ml de la subreceta SUB001.
- **SUB001 — Salsa César:** cálculo del coste del lote, rendimiento estimado, coste por ración y número aproximado de raciones.

### Qué permite analizar

- Calcular el coste de una receta a partir de las cantidades y los costes unitarios de sus ingredientes.
- Seleccionar ingredientes desde una lista vinculada a Inventario para reducir errores tipográficos y mantener consistencia en los datos.
- Estimar el rendimiento de un lote de SUB001 y su coste por ración.
- Imputar a REC001 el coste proporcional de los 40 ml de Salsa César utilizados.
- Aplicar un margen predeterminado según la categoría del plato. En el ejemplo, la categoría **Ensaladas** tiene configurado inicialmente un margen del 80 %, que puede modificarse.
- Cambiar el **margen objetivo** para explorar escenarios de precio recomendado. Por ejemplo: «Si quiero alcanzar un margen objetivo del 90 %, ¿qué precio de venta resultaría con estos costes?». Es un parámetro de análisis, no una afirmación de beneficio neto del negocio.
- Identificar alérgenos asociados a los ingredientes y reflejarlos en la tabla de ingredientes y en los indicadores de la ficha.

Las capturas de REC001 muestran distintos escenarios de margen objetivo para ilustrar cómo cambia el precio recomendado al modificar ese parámetro.

### Cálculo de la subreceta

En el escenario documentado, SUB001 utiliza 40 ml por ración. Se ha estimado un rendimiento de 400 ml por lote, equivalente a unas 10 raciones. Con los costes simulados de los ingredientes, la ficha calcula el coste del lote y el coste proporcional de cada ración. El rendimiento es una estimación de trabajo, no una medición de producción real.

Para las anchoas se ha supuesto, a efectos del ejercicio, que una lata de 100 g aporta aproximadamente 80 g escurridos. Este supuesto afecta al coste por gramo y debe confirmarse con el envase del producto que se utilice.

### Alérgenos y validación por marca

La ficha relaciona ingredientes con alérgenos y actualiza automáticamente los indicadores. **«Revisar» es una indicación intencionada** para ingredientes comerciales cuya composición puede variar según la marca, como la salsa Worcestershire. Antes de utilizar una marca concreta, hay que comprobar su etiqueta y completar la clasificación correspondiente. En el caso de la mayonesa utilizada en el ejemplo, se identifica el huevo.

La automatización facilita la consulta, pero la información debe contrastarse con el etiquetado del producto real antes de aplicarla en un establecimiento.

### Herramientas y lógica aplicada en esta entrega

- **Excel:** tablas, fórmulas de búsqueda, cálculo de costes y fichas de receta.
- **VBA:** actualización automática de los indicadores de alérgenos.
- **Criterio de hostelería:** relación entre ingredientes, rendimiento de producción, coste por ración y decisiones de precio.

### Alcance y limitaciones

El coste mostrado se construye con los ingredientes registrados en las fichas. Mano de obra, energía, mermas, envases y otros gastos generales no forman parte de este escandallo, salvo que se añadan expresamente al modelo.

La selección de ingredientes se apoya en Inventario. La trazabilidad y centralización completa del coste de las subrecetas está pendiente de revisión y mejora, por lo que no se presenta como una funcionalidad completamente cerrada en esta entrega.

## Estado y evolución del proyecto

GastroData se desarrolla por módulos y entregas progresivas. Esta primera documentación se centra en REC001 y SUB001. El proyecto global incluye también el análisis de datos en Power BI y la carta digital mediante QR, que se documentan y evolucionan en sus respectivos módulos.

El objetivo es construir un ecosistema de herramientas que conecte la operativa diaria de un negocio hostelero con el análisis de información y la digitalización de procesos, manteniendo diferenciados los resultados calculados, los supuestos de ejemplo y las funcionalidades todavía en desarrollo.
