# Calc_Presupuesto
Caso 3: Calculadora de Presupuesto Mensual 

## Descripción del proyecto
Aplicación que permite registrar ingresos, gastos y generar un balance mensual. El objetivo es ayudar al usuario a gestionar sus finanzas personales de manera simple y rápida.

---

## Objetivos
Los principales objetivos se basan en la versión más reciente (V2) del Documento de Requerimientos
* **Gestión de Transacciones:** Crear, editar y eliminar transacciones de ingresos y gastos.
* **Resumen Dinámico:** Actualización automática cada vez que se agrega o elimina un registro.
* **Exportación:** Permitir al usuario generar un archivo descargable del balance mensual a **PDF**.
* **Historial:** Proporcionar una lista de transacciones filtrable por fecha, tipo y monto.
* **Límite de Registros:** Establecer un máximo de 500 entradas activas por usuario.

---

## Requerimientos

### ✔ Requerimientos Funcionales (V2)
| ID | Requerimiento | Descripción |
|----|---------------|-------------|
| RF1 | Gestión de transacciones (crear/editar/eliminar) | El sistema deberá validar automáticamente los campos antes de permitir el registro. |
| RF2 | Resumen mensual dinámico | Actualización automática cada vez que se agrega o elimina un registro. |
| RF3 | Exportación del balance mensual a PDF | El usuario podrá generar un archivo descargable. |
| RF4 | Historial de transacciones | Lista filtrable por fecha, tipo y monto. |
| RF5 | Límite de registros | Máximo 500 entradas activas por usuario. |

### ✔ Requerimientos No Funcionales (V2)
| ID | Requerimiento | Descripción |
|----|---------------|-------------|
| RNF1 | Tiempo de respuesta | El sistema debe garantizar un tiempo de respuesta máximo de **1 segundo** por cada operación realizada. |
| RNF2 | Interfaz adaptable | La interfaz debe estar diseñada para adaptarse correctamente tanto a pantallas de ordenador como a dispositivos móviles. |
| RNF3 | Validación estricta de datos | Validación estricta de datos antes de cualquier operación. |
| RNF4 | Robustez ante fallos | El sistema debe estar preparado para evitar cierres inesperados y la consiguiente pérdida de datos. |
| RNF5 | Registro en GitHub | Registrar y usar control de versiones en GitHub facilita el seguimiento y gestión de los cambios realizados. |

---

## Tabla de Pruebas Funcionales
La siguiente tabla simula los resultados obtenidos durante la ejecución de las pruebas unitarias y de validación:

| ID Caso | Tipo de Prueba | Requerimiento Asociado | Datos de Entrada | Resultado Esperado | Resultado Obtenido |
|---------|----------------|------------------------|------------------|--------------------|--------------------|
| CP-U1   | Unitario       | RF1, RF2, RF3          | Ingreso: \$2000.00; Gasto: \$500.00 | El Balance Neto debe ser: **\$1500.00** | \$1500.00  |
| CP-U2   | Unitario       | RNF3                   | Intentar ingresar Gasto: **-\$100.00** | El sistema debe mostrar un **mensaje de error** e **impedir** el registro. | Mensaje de error: "Monto debe ser positivo". Registro no permitido.  |
| CP-V1   | Validación     | RF3, RF4               | Ingresos: Sueldo (\$1500), Venta (\$500). Gastos: Alquiler (\$800), Comida (\$300), Transporte (\$50). | Balance Neto: **\$850.00**. La lista debe mostrar 5 ítems. | Balance: \$850.00. La lista muestra los 5 ítems correctamente. 

---

## Tipo de Mantenimiento Propuesto
**Tipo sugerido:** Perfectivo.

**Razón:** El sistema ya cumple el funcionamiento básico, pero puede mejorarse agregando nuevas capacidades y optimizando la experiencia de usuario.

**Propuestas Perfectivas Específicas**:
* Añadir exportación a PDF y Excel.
* Agregar gráficos dinámicos de barras y pastel.
* Implementar notificaciones de gastos altos.

---

## Reflexión sobre Control de Versiones
**GitHub y Markdown:**
* GitHub permite mantener un historial claro del avance del proyecto, comparar versiones, corregir errores y colaborar eficazmente.
* Markdown se utiliza porque es una forma sencilla de escribir y dar formato a textos. Es fácil de leer, de escribir y de mantener, facilitando la documentación de forma ligera, estructurada y compatible con GitHub.

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
