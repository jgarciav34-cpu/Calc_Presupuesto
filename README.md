# Calc_Presupuesto
[cite_start]Caso 3: Calculadora de Presupuesto Mensual [cite: 12, 17]

## Descripción del proyecto
[cite_start]Aplicación que permite registrar ingresos, gastos y generar un balance mensual[cite: 1]. El objetivo es ayudar al usuario a gestionar sus finanzas personales de manera simple y rápida.

---

## Objetivos
[cite_start]Los principales objetivos se basan en la versión más reciente (V2) del Documento de Requerimientos[cite: 18]:
* [cite_start]**Gestión de Transacciones:** Crear, editar y eliminar transacciones de ingresos y gastos[cite: 21].
* [cite_start]**Resumen Dinámico:** Actualización automática cada vez que se agrega o elimina un registro[cite: 21].
* [cite_start]**Exportación:** Permitir al usuario generar un archivo descargable del balance mensual a **PDF**[cite: 21].
* [cite_start]**Historial:** Proporcionar una lista de transacciones filtrable por fecha, tipo y monto[cite: 21].
* [cite_start]**Límite de Registros:** Establecer un máximo de 500 entradas activas por usuario[cite: 21].

---

## Requerimientos

### ✔ Requerimientos Funcionales (V2)
| ID | Requerimiento | Descripción |
|----|---------------|-------------|
| RF1 | Gestión de transacciones (crear/editar/eliminar) | [cite_start]El sistema deberá validar automáticamente los campos antes de permitir el registro[cite: 21]. |
| RF2 | Resumen mensual dinámico | [cite_start]Actualización automática cada vez que se agrega o elimina un registro[cite: 21]. |
| RF3 | Exportación del balance mensual a PDF | [cite_start]El usuario podrá generar un archivo descargable[cite: 21]. |
| RF4 | Historial de transacciones | [cite_start]Lista filtrable por fecha, tipo y monto[cite: 21]. |
| RF5 | Límite de registros | [cite_start]Máximo 500 entradas activas por usuario[cite: 21]. |

### ✔ Requerimientos No Funcionales (V2)
| ID | Requerimiento | Descripción |
|----|---------------|-------------|
| RNF1 | Tiempo de respuesta | [cite_start]El sistema debe garantizar un tiempo de respuesta máximo de **1 segundo** por cada operación realizada[cite: 24]. |
| RNF2 | Interfaz adaptable | [cite_start]La interfaz debe estar diseñada para adaptarse correctamente tanto a pantallas de ordenador como a dispositivos móviles[cite: 24]. |
| RNF3 | Validación estricta de datos | [cite_start]Validación estricta de datos antes de cualquier operación[cite: 24]. |
| RNF4 | Robustez ante fallos | [cite_start]El sistema debe estar preparado para evitar cierres inesperados y la consiguiente pérdida de datos[cite: 24]. |
| RNF5 | Registro en GitHub | [cite_start]Registrar y usar control de versiones en GitHub facilita el seguimiento y gestión de los cambios realizados[cite: 24]. |

---

## Tabla de Pruebas Funcionales
[cite_start]La siguiente tabla simula los resultados obtenidos durante la ejecución de las pruebas unitarias y de validación[cite: 16]:

| ID Caso | Tipo de Prueba | Requerimiento Asociado | Datos de Entrada | Resultado Esperado | Resultado Obtenido |
|---------|----------------|------------------------|------------------|--------------------|--------------------|
| CP-U1   | Unitario       | RF1, RF2, RF3          | Ingreso: \$2000.00; Gasto: \$500.00 | El Balance Neto debe ser: **\$1500.00** | [cite_start]\$1500.00 [cite: 15] |
| CP-U2   | Unitario       | RNF3                   | Intentar ingresar Gasto: **-\$100.00** | El sistema debe mostrar un **mensaje de error** e **impedir** el registro. | Mensaje de error: "Monto debe ser positivo". [cite_start]Registro no permitido. [cite: 15] |
| CP-V1   | Validación     | RF3, RF4               | Ingresos: Sueldo (\$1500), Venta (\$500). Gastos: Alquiler (\$800), Comida (\$300), Transporte (\$50). | Balance Neto: **\$850.00**. La lista debe mostrar 5 ítems. | Balance: \$850.00. [cite_start]La lista muestra los 5 ítems correctamente. [cite: 15] |

---

## Tipo de Mantenimiento Propuesto
[cite_start]**Tipo sugerido:** Perfectivo[cite: 1].

[cite_start]**Razón:** El sistema ya cumple el funcionamiento básico, pero puede mejorarse agregando nuevas capacidades y optimizando la experiencia de usuario[cite: 1].

**Propuestas Perfectivas Específicas**:
* [cite_start]Añadir exportación a PDF y Excel[cite: 5].
* [cite_start]Agregar gráficos dinámicos de barras y pastel[cite: 5].
* [cite_start]Implementar notificaciones de gastos altos[cite: 5].

---

## Reflexión sobre Control de Versiones
**GitHub y Markdown:**
* [cite_start]GitHub permite mantener un historial claro del avance del proyecto, comparar versiones, corregir errores y colaborar eficazmente[cite: 2].
* [cite_start]Markdown se utiliza porque es una forma sencilla de escribir y dar formato a textos[cite: 1]. [cite_start]Es fácil de leer, de escribir y de mantener, facilitando la documentación de forma ligera, estructurada y compatible con GitHub[cite: 2].

---

## Estructura del Repositorio
---

##  Estructura del Repositorio
```
/Caso_Seleccionado
│── README.md
│── requerimientos/
│── pruebas/
│── mantenimiento/
│── investigacion/
└── evidencias/
```
