[ 🌐 عربي ](README.ar.md) | [ 🇩🇪 Deutsch ](README.de.md) | [ 🇫🇷 Français ](README.fr.md) | [ 🇳🇱 Nederlands ](README.nl.md) | [ 🇪🇸 Español ](README.sp.md) | [ 🇬🇧 English ](README.md)

# Consola de gobernanza de inventario DTC transfronteriza
## Depuración de señales de demanda, control de obligaciones de preventa y planificación de compras para marcas basadas en Shopify

![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)
![Platform](https://img.shields.io/badge/Platform-Browser%20%7C%20Excel-success)
![Tool](https://img.shields.io/badge/Tool-Inventory%20Decision%20Support-orange)

**Convierta datos de pedidos de Shopify ruidosos en decisiones de compra en minutos—directamente en el navegador o en el libro de Excel, sin registro, sin instalación y sin suscripción recurrente.**

**Sin registro. Sin instalación. Gratis en su navegador.**

Pruebe la versión de navegador gratis. Si necesita la versión de Excel, puede comprarla con una garantía de devolución de dinero de 30 días sin preguntas.
>
> 🌐 **Abrir en el navegador** → [*Versión HTML en vivo*](https://hyvoid.github.io/Cross-Border-DTC-Inventory-Governance-Console/)
>
> 📥 **Descargar la versión de Excel**  
> *(Publicación de GitHub / descarga desde el [Sitio web](https://www.theseusworkshop.com/))*

---

## Qué le ayuda a monitorear

En lugar de consultar informes desconectados de Shopify, Inventory Planner y hojas de cálculo, esta consola reúne las señales operativas en un marco de decisión único.

Permite ver:

- Las obligaciones de preventa pendientes que no deben contarse como inventario disponible.
- La demanda real tras eliminar la distorsión de las preventas y las devoluciones esperadas.
- Las cantidades de compra que reflejan las obligaciones reales de inventario en lugar de ventas infladas.
- La distribución del inventario entre el Reino Unido, EE. UU., la UE y Australia según la contribución de la demanda.
- Las brechas de sincronización entre Shopify, Inventory Planner y los registros de compras antes de que se conviertan en errores de planificación.
- Las prioridades de compra semanales apoyadas en datos operativos conciliados en lugar de ajustes manuales de hojas de cálculo.

---

## Flujo de trabajo de inicio rápido

El libro está diseñado en torno a un flujo de trabajo de **configurar una vez, actualizar periódicamente** en lugar de un mantenimiento constante de hojas de cálculo.

### 1. Configurar parámetros operativos

Abra la hoja **Config** y defina las reglas operativas, tales como:

- el plazo de entrega
- la ventana de devolución
- la proporción de asignación de mercados
- el factor de seguridad de preventas

Estos valores suelen cambiar solo cuando cambian las políticas del negocio.

---

### 2. Importar datos empresariales existentes

Exporte sus datos operativos existentes desde Shopify y Inventory Planner.

Pegue o actualice:

- Shopify Orders
- Shopify Returns
- Current Inventory
- Purchase Status

No se requiere ninguna reestructuración ni actualización manual de fórmulas.

---

### 3. Revisar decisiones actualizadas automáticamente

Navegue directamente a las hojas de análisis.

El libro actualiza de inmediato:

- las obligaciones de preventa pendientes
- el análisis de devoluciones por cohorte
- la demanda corregida
- las recomendaciones de compra
- la asignación por país
- el estado de conciliación

No se necesita ningún cálculo manual.

---

### 4. Actualizar semanalmente

Cada ciclo de planificación simplemente reemplaza las tablas de entrada brutas.

Todo lo que está aguas abajo se actualiza automáticamente.

No hay reconstrucción del libro, ni copia de fórmulas, ni mantenimiento estructural.

**Defina algunos parámetros operativos. Importe sus datos existentes. Revise las recomendaciones. Actualice siempre que haya nuevos datos empresariales.**

---

## Por qué construí esto

Muchos problemas de planificación de inventario no se deben a algoritmos de previsión deficientes.

Se deben a señales de demanda deficientes.

Para las marcas que operan varias tiendas Shopify, especialmente los negocios de moda con preventas intensivas y altas tasas de devolución, las ventas declaradas suelen contener señales que nunca deberían convertirse en demanda de compra.

Una preventa se registra como venta antes de que exista el inventario.

Un artículo devuelto puede no reingresar al inventario hasta semanas después.

Los planificadores de inventario reciben con frecuencia ventas históricas sin entender ninguna de las dos condiciones.

El resultado es previsible:

- comprar el doble para la misma demanda,
- sobreestimar las necesidades futuras de inventario,
- acumular inventario innecesario,
- aumentar el capital de trabajo sin aumentar los ingresos.

---

Construí este proyecto porque observé repetidamente que los analistas pasaban horas limpiando datos antes de poder siquiera comenzar a tomar decisiones de compra.

En lugar de crear otro panel de control, quise empaquetar el propio proceso de razonamiento en un libro reutilizable.

Por ejemplo:

**Antes**

Un SKU vende **500 unidades** durante un lanzamiento.

La planificación tradicional supone que la demanda es igual a 500.

Las recomendaciones de compra se generan a partir de esa cifra.

---

**Después**

El libro descubre:

- 120 unidades siguen siendo preventas no cumplidas.
- Las devoluciones esperadas equivalen a 48 unidades.
- La demanda corregida se convierte en **332 unidades**.

La conversación sobre compras cambia de inmediato.

En lugar de discutir con qué rapidez reponer 500 unidades, los equipos operativos discuten si 332 unidades son suficientes después de considerar el plazo de entrega y el stock de seguridad.

Esa es una decisión fundamentalmente diferente—no porque las fórmulas hayan cambiado, sino porque la señal de demanda se volvió confiable.

---

## Problemas comunes de planificación de inventario que resuelve

| Problema | Sin esta herramienta | Con esta herramienta |
|----------|-------------------|----------------|
| Las preventas inflan la demanda | Las compras duplican inventario ya comprometido | Las obligaciones pendientes se aíslan antes de la previsión |
| Las devoluciones distorsionan las ventas históricas | Las previsiones suponen que todas las ventas se convierten en demanda permanente | La modelización de devoluciones por cohorte estima el inventario recuperable |
| Varios países compiten por el inventario | La asignación manual crea niveles de stock inconsistentes | La asignación sigue proporciones de contribución de mercado configurables |
| Las decisiones de compra dependen de sistemas desconectados | Los analistas comparan Shopify, Inventory Planner y el ERP manualmente | La conciliación automatizada resalta las cantidades discrepantes |
| La planificación semanal requiere reconstruir hojas de cálculo | La copia de fórmulas introduce errores ocultos | Los datos brutos se actualizan mientras los cálculos permanecen sin cambios |
| Los problemas de inventario se descubren demasiado tarde | Los errores de compra aparecen después de crear la orden de compra | La conciliación expone las discrepancias antes de emitir las órdenes |

---

## Para quién es esto

Este proyecto está diseñado para organizaciones que gestionan decisiones de inventario en múltiples mercados donde las señales de demanda se ven influidas por preventas, devoluciones y ejecución internacional.

Los usuarios típicos incluyen:

- marcas de moda DTC
- equipos de operaciones de Shopify
- planificadores de inventario
- analistas de cadena de suministro
- equipos de planificación de mercancía
- gerentes de operaciones de comercio electrónico

Es especialmente valioso donde las decisiones de compra dependen de entender la diferencia entre las **ventas declaradas** y la **demanda real de inventario**.

**No** está destinado a reemplazar plataformas ERP, sistemas de gestión de almacenes ni software de inventario empresarial.

En cambio, proporciona una capa analítica ligera entre los sistemas operativos y las decisiones de compra.

No se requiere experiencia en hojas de cálculo. Abra la versión de navegador o el libro de Excel, importe sus datos operativos y comience de inmediato a revisar las recomendaciones de compra.

---

## Acerca de

Construyo libros analíticos ligeros para situaciones empresariales en las que simplemente hay demasiadas piezas en movimiento para razonarlas mentalmente.

En lugar de reemplazar software empresarial, estas herramientas organizan la información necesaria para tomar la siguiente decisión operativa con confianza.

La **Consola de gobernanza de inventario DTC transfronteriza** es un ejemplo de este enfoque: transformar datos operativos fragmentados en un marco de apoyo a la decisión repetible que puede actualizarse siempre que haya nueva información.

## Detalles técnicos

<details>
<summary><strong>Para revisores técnicos, practicantes de Excel y colaboradores</strong></summary>

---

## Arquitectura del libro

El libro sigue una arquitectura estricta de **entrada → depuración → decisión → validación → salida**. Cada hoja tiene una única responsabilidad, lo que hace que el proceso analítico sea transparente y auditable.

| Capa | Hoja | Propósito | Consumidor de salida |
|--------|-----------|---------|-----------------|
| Configuración | Config | Reglas del negocio, plazo de entrega, proporciones de asignación, ventana de devolución | Todas las hojas de cálculo |
| Entrada bruta | Raw_Orders | Exportaciones de pedidos de Shopify | Motor de demanda |
| Entrada bruta | Raw_Returns | Exportaciones de devoluciones de Shopify | Modelo de devoluciones |
| Depuración | Preorder_Liability | Obligaciones de preventa pendientes | Demanda corregida, planificador de compras |
| Depuración | Cohort_Return_Model | Comportamiento de devoluciones por cohorte | Demanda corregida |
| Decisión | Corrected_Demand | Demanda real de compra | Inventory Planner |
| Decisión | PO_Planner | Recomendaciones de compra | Equipo de compras |
| Decisión | Location_Allocator | Asignación por país | Almacén y logística |
| Validación | Reconciliation | Verificación entre sistemas | Operaciones |
| Presentación | Executive_Dashboard | Indicadores de gestión | Dirección |

### Flujo de datos general

```text
Shopify Orders
                     \
                      \
                       --> Raw_Orders ------------------\
                                                        \
                                                         \
Inventory Planner Export --> Current Inventory -----------> PO Planner
                                                          /
                                                         /
Shopify Returns --> Raw_Returns --> Cohort Return Model-/

                     Config Parameters
                             │
                             ▼
                 Preorder Liability Engine
                             │
                             ▼
                 Corrected Demand Engine
                             │
                             ▼
                Purchase Recommendation
                             │
                             ▼
                  Country Allocation
                             │
                             ▼
                    Reconciliation
                             │
                             ▼
                 Executive Dashboard
```

A diferencia de las hojas de cálculo tradicionales, donde los cálculos se dispersan por múltiples hojas, este libro separa las responsabilidades operativas en capas analíticas independientes.

Esa separación permite rastrear cada recomendación de compra hasta los datos operativos que la originaron.

---

## Tres trampas analíticas que atrapan incluso a planificadores de inventario experimentados

---

## Trampa 1 — Tratar las preventas como demanda completada

### Decisión

El equipo de compras aumenta la producción tras observar ventas inusualmente fuertes.

### Supuesto oculto

Se supone que las ventas declaradas representan la demanda de clientes cumplida.

En realidad, una gran proporción de esas ventas sigue siendo preventas pendientes.

### Por qué esto cambia la recomendación

| Métrica | Visión tradicional | Visión corregida |
|---------|-----------------|----------------|
| Ventas | 1.000 | 1.000 |
| Preventas pendientes | ignoradas | 280 |
| Demanda de compra | 1.000 | 720 |

Sin separar las obligaciones pendientes, los planificadores de inventario compran productos que los clientes ya se han comprometido a comprar.

Esto genera compras duplicadas.

### Por qué este razonamiento es incorrecto

Las ventas describen la actividad comercial.

La compra debería responder a las obligaciones físicas de inventario.

No siempre son lo mismo.

Especialmente en lanzamientos de moda, financiación colectiva y plazos de fabricación largos.

### Enfoque corregido

Las preventas pendientes se aíslan antes de que la demanda entre en el modelo de compra.

Solo la demanda cumplida contribuye a los requisitos futuros de compra.

### Resultado de la decisión

En lugar de aumentar la producción en 1.000 unidades,

las operaciones compran inventario para aproximadamente 720 unidades,

lo que reduce la inversión innecesaria en inventario sin dejar de proteger los compromisos con los clientes.

<details>
<summary>Lógica de la fórmula</summary>

```excel
Outstanding Liability

=
Total Preorder Sold
-
Fulfilled Preorders
```

Implementado con fórmulas de matriz dinámica y SUMIFS.

</details>

---

## Trampa 2 — Medir las devoluciones por mes natural

### Decisión

La dirección concluye que las tasas de devolución han bajado porque las devoluciones de este mes parecen menores.

### Supuesto oculto

Se supone que las devoluciones ocurridas durante un mes natural pertenecen a las ventas realizadas en ese mismo mes.

Ese supuesto casi nunca es cierto.

Las devoluciones están ligadas a las cohortes de compra, no a los períodos de información.

### Por qué esto cambia la recomendación

Ejemplo:

| Mes | Ventas | Devoluciones del calendario |
|--------|-------|-----------------|
| Enero | 8.000 | 220 |
| Febrero | 6.500 | 640 |

La información tradicional sugiere que los productos de febrero tienen peor rendimiento.

Sin embargo, la mayoría de las devoluciones de febrero pertenecen en realidad a las compras de enero.

### Por qué este razonamiento es incorrecto

El comportamiento del cliente sigue la antigüedad del pedido.

Los informes siguen las fechas del calendario.

Esas líneas de tiempo rara vez coinciden.

### Enfoque corregido

Los pedidos se agrupan por cohorte de compra.

Las devoluciones se miden:

- dentro de 14 días
- dentro de 30 días
- dentro de 45 días

El perfil de devoluciones resultante refleja el comportamiento real del cliente en lugar de artefactos de información.

### Resultado de la decisión

En lugar de reducir las compras de febrero,

la empresa descubre que los productos de enero experimentaron devoluciones tardías,

mientras que la demanda de febrero se mantiene saludable.

<details>
<summary>Lógica de la fórmula</summary>

```excel
Unique Cohort Months

=SORT(
UNIQUE(
TEXT(Order_Date,"yyyy-mm")
))
```

Combinado con MAP(), LET() y SUMIFS() para calcular las ventanas de devolución de forma dinámica.

</details>

---

## Trampa 3 — Comprar a partir de ventas brutas en lugar de demanda corregida

### Decisión

Inventory Planner recibe ventas históricas exportadas.

Las previsiones parecen razonables.

Aun así, la compra genera inventario excedente.

### Supuesto oculto

Se supone que las ventas históricas ya representan una demanda limpia.

Rara vez lo hacen.

Las ventas históricas suelen incluir:

- preventas pendientes
- devoluciones esperadas
- picos de lanzamiento temporales

### Antes

```text
Historical Sales

980
```

Inventory Planner prevé a partir de 980.

### Después de la depuración

```text
Historical Sales          980

Outstanding Liability    -170

Expected Returns          -62

Corrected Demand          748
```

### Por qué este razonamiento es incorrecto

Los algoritmos de previsión amplifican la calidad de la entrada.

No pueden reparar señales históricas deficientes.

Basura que entra sigue produciendo basura de aspecto seguro.

### Enfoque corregido

La demanda se corrige antes de entrar en el software de previsión.

Inventory Planner recibe demanda de compra en lugar de actividad comercial.

### Resultado de la decisión

Las recomendaciones de compra se vuelven considerablemente más estables.

El capital de trabajo disminuye manteniendo los niveles de servicio al cliente.

<details>
<summary>Lógica de la fórmula</summary>

```excel
Corrected Demand

=
Raw Sales
-
Outstanding Liability
-
Expected Returns
```

Implementado con LET(), XLOOKUP(), SUMIFS() y matrices dinámicas.

</details>

---

## Escenario de ejemplo

Una marca de moda con sede en el Reino Unido lanza una nueva chaqueta a través de cuatro tiendas Shopify que sirven al Reino Unido, EE. UU., la UE y Australia.

En dos semanas, Shopify declara **2.450 unidades vendidas**, lo que sugiere un lanzamiento muy exitoso. Con base únicamente en las ventas brutas, el equipo de compras considera cursar una orden de reposición urgente.

El libro cuenta una historia diferente.

En primer lugar, la hoja **Preorder_Liability** identifica **540 unidades** que se han vendido pero aún no se han cumplido. Estas representan compromisos existentes con clientes, no demanda de mercado adicional.

A continuación, el **Cohort_Return_Model** evalúa el comportamiento histórico de devoluciones de productos comparables. Lanzamientos anteriores muestran una tasa de devolución definitiva del **11,8 %**, lo que indica que aproximadamente **289 unidades** se espera que regresen al inventario tras la entrega.

El motor **Corrected_Demand** recalcula entonces la señal de compra:

| Concepto | Cantidad |
|------|---------:|
| Ventas declaradas | 2.450 |
| Preventas pendientes | -540 |
| Devoluciones esperadas | -289 |
| Demanda corregida | **1.621** |

En lugar de comprar contra la cifra principal de ventas, **PO_Planner** usa la demanda corregida junto con el plazo de entrega, el stock actual y los parámetros de seguridad para recomendar una cantidad de reposición significativamente menor.

La recomendación se distribuye automáticamente entre los almacenes del Reino Unido, EE. UU., la UE y Australia según las proporciones de asignación configuradas.

Por último, la hoja **Reconciliation** compara las obligaciones de Shopify con los datos de sincronización de Inventory Planner. Si las obligaciones pendientes difieren entre los sistemas, el libro emite una advertencia **INVESTIGATE** antes de que se cursen las órdenes de compra.

El resultado es una decisión de compra apoyada en evidencia operativa conciliada en lugar de totales de ventas brutas, lo que reduce el inventario excedente sin dejar de mantener los compromisos de ejecución con los clientes.

---

### Referencia de fórmulas

<details>
<summary>Config</summary>

| Fórmula / lógica | Propósito | Notas |
|-----------------|---------|------|
| Configuración manual | Define los parámetros operativos | Se mantiene solo cuando cambian las reglas del negocio |
| Proporción de asignación de mercados | Distribución del inventario por país | La usa Location_Allocator |
| Plazo de entrega | Planificación de compras | Se incluye en el cálculo del inventario objetivo |
| Ventana de devolución | Análisis por cohorte | Controla el momento esperado de las devoluciones |
| Factor de seguridad de preventas | Colchón de compra | Ajustable por mercado |

</details>

---

<details>
<summary>Preorder_Liability</summary>

### Generar lista de SKU únicos

```excel
=SORT(
UNIQUE(
Raw_Orders[SKU]
))
```

**Propósito**

Crea una lista maestra de SKU dinámica directamente a partir del historial de pedidos importado.

---

### Obligaciones de preventa pendientes

```excel
=LET(

SKU_List,A2#,

Preorder_Sold,

SUMIFS(
Raw_Orders[Quantity],
Raw_Orders[SKU],SKU_List,
Raw_Orders[Sales_Type],"Preorder"
),

Preorder_Fulfilled,

SUMIFS(
Raw_Orders[Quantity],
Raw_Orders[SKU],SKU_List,
Raw_Orders[Sales_Type],"Preorder",
Raw_Orders[Fulfillment_Status],"Fulfilled"
),

Preorder_Sold-
Preorder_Fulfilled

)
```

**Propósito**

Calcula las obligaciones de inventario que ya se han vendido pero que aún no se han entregado físicamente.

Estas cantidades se excluyen intencionalmente de la demanda de compra futura.

---

</details>

---

<details>
<summary>Cohort_Return_Model</summary>

### Generar meses de cohorte

```excel
=SORT(
UNIQUE(
TEXT(
Raw_Orders[Order_Date],
"yyyy-mm"
)
))
```

---

### Cálculo de devoluciones por cohorte

Implementado con

- LET()
- MAP()
- SUMIFS()

El cálculo mide las devoluciones en relación con la fecha de pedido original en lugar de los períodos de información del calendario.

Las ventanas de devolución incluyen:

- 14 días
- 30 días
- 45 días

Esto produce una estimación estable del comportamiento de devolución definitivo.

---

### Tasa de devolución definitiva

```text
Ultimate Return Rate

=

Total Returned Quantity

/

Original Cohort Sales
```

El libro usa el comportamiento por cohorte en lugar de porcentajes de devolución mensuales porque las decisiones de compra dependen del comportamiento del cliente y no de los períodos de información.

</details>

---

<details>
<summary>Corrected_Demand</summary>

### Señal de demanda corregida

```excel
=LET(

RawSales,

SUMIFS(...),

Outstanding,

XLOOKUP(...),

ExpectedReturns,

RawSales*
AverageReturnRate,

ROUND(

RawSales
-
Outstanding
-
ExpectedReturns,

0)

)
```

### Propósito

Transforma la actividad comercial en demanda de compra.

En lugar de prever directamente a partir de las ventas históricas, el libro elimina:

- las preventas pendientes
- el inventario que se espera que regrese mediante devoluciones de clientes

La señal resultante es adecuada para Inventory Planner o software de previsión similar.

</details>

---

<details>
<summary>PO_Planner</summary>

### Requisito de compra neto

```text
Net Requirement

=

Target Inventory

-

Current Stock

+

Outstanding Liability
```

---

### Cantidad de compra recomendada

```excel
=IF(

NetRequired<=0,

0,

MROUND(

NetRequired,

MOQ

)

)
```

### Propósito

Recomienda automáticamente cantidades de compra respetando las cantidades mínimas de pedido de los proveedores.

En lugar de exigir redondeo manual, las recomendaciones de compra son inmediatamente aptas para cursar órdenes de compra.

</details>

---

<details>
<summary>Location_Allocator</summary>

### Asignación por país

```excel
=ROUND(

Total_PO

*

Allocation_Ratio,

0
)
```

Cada almacén de destino recibe inventario según proporciones de contribución de mercado configurables.

El modelo de asignación puede ampliarse fácilmente a países adicionales sin cambiar los cálculos posteriores.

</details>

---

<details>
<summary>Reconciliation</summary>

### Verificación de sincronización

```excel
=IF(

Gap=0,

"PASS",

"INVESTIGATE"

)
```

donde

```text
Gap

=

Shopify Unfulfilled

-

Inventory Planner Liability
```

Propósito:

Resalta de inmediato los problemas de sincronización antes de que las decisiones de compra dependan de datos inconsistentes.

</details>

---

## Reglas de validación

| Campo | Regla de validación | Comportamiento ante error |
|------|-----------------|----------------|
| Market | Debe existir en la tabla Config | La búsqueda devuelve la asignación predeterminada o una advertencia de validación |
| SKU | No puede estar vacío | La fila se excluye de los cálculos |
| Order_ID | Debe ser único | Advertencia de transacción duplicada |
| Return_ID | Debe ser único | Advertencia de devolución duplicada |
| Order Date | Se requiere una fecha válida | El registro se ignora hasta que se corrija |
| Return Date | No puede ser anterior a Order Date | Se genera un indicador de validación |
| Quantity | Debe ser mayor que cero | La fila se excluye |
| Return Quantity | No puede superar la cantidad original | Advertencia de validación |
| Sales Type | Solo Normal o Preorder | La categoría no válida se resalta |
| Fulfillment Status | Fulfilled / Unfulfilled | Los valores no válidos se excluyen |
| Allocation Ratio | El total debe ser igual al 100 % | Advertencia de asignación por país |
| Lead Time | Entero no negativo | El cálculo de compra se detiene |
| Return Window | Entero positivo | Advertencia de cálculo de cohorte |
| MOQ | Mayor que cero | La recomendación de compra se desactiva |
| Current Inventory | No puede ser negativo | Advertencia de inventario |
| Outstanding Liability | No puede superar las ventas de preventa | Alerta de conciliación |
| Recommended Purchase Quantity | Redondeada al MOQ | Se ajusta automáticamente |
| Synchronization Gap | Debe ser igual a cero | Se muestra el estado INVESTIGATE |

</details>

---

## Otras herramientas de esta serie

Estos libros siguen la misma filosofía de diseño: sistemas ligeros de apoyo a la decisión construidos para problemas operativos recurrentes en lugar de reemplazar software empresarial.

- **Previsión de inventario y planificación de reposición** — Previsión de la demanda, cálculo del punto de reposición y análisis de riesgo de inventario.
- **Construction Estimating System** — Estimación de ensamblajes, bibliotecas de costos, preparación de ofertas y presupuestación de proyectos.
- **Marketing Budget Allocation Simulator** — Planificación por escenarios para inversiones de marketing multicanal.
- **Multi-Currency Trade Finance Dashboard** — Informes financieros transfronterizos y análisis de rentabilidad.
- **Coffee Shop Operations Audit Toolkit** — Revisión del rendimiento de las tiendas y análisis del cumplimiento operativo.
- **Project Management & Progress Billing Console** — Seguimiento de hitos, facturación y control presupuestario.

Se publicarán más libros analíticos a través del repositorio de GitHub y nuestro [Sitio web](https://www.theseusworkshop.com/).

---

## Licencia

Este proyecto está licenciado bajo la **Apache License 2.0**.

Usted es libre de:

- usar el libro con fines personales o comerciales.
- modificar el marco analítico para adaptarlo a los requisitos operativos.
- distribuir versiones modificadas de conformidad con la Apache License 2.0.

Consulte el archivo **LICENSE** para ver el texto completo de la licencia.

---

## Notas finales

Este libro está posicionado intencionadamente como una **capa de apoyo a la decisión**, no como reemplazo de plataformas ERP, WMS o de planificación empresarial.

Su propósito es sencillo:

- capturar datos operativos de los sistemas existentes,
- eliminar las distorsiones analíticas antes de planificar,
- generar recomendaciones de compra que reflejen las obligaciones reales de inventario,
- proporcionar cálculos transparentes que pueden inspeccionarse, reproducirse y auditarse.

En lugar de añadir un panel de control más, el libro productiviza una metodología de planificación de inventario repetible que puede actualizarse en minutos y que pueden entender tanto los usuarios operativos como los revisores técnicos.
