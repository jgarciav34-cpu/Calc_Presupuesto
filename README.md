# Calc_Presupuesto
Caso 3: Calculadora de Presupuesto Mensual

##  Descripción del proyecto
Aplicación que permite registrar ingresos, gastos y generar un balance mensual. El objetivo es ayudar al usuario a gestionar sus finanzas personales de manera simple y rápida.

---

##  Objetivos
- Registrar transacciones de ingresos y gastos.
- Calcular automáticamente el balance mensual.
- Mostrar un resumen claro y entendible.
- Permitir edición o eliminación de transacciones.
- Facilitar la exportación de reportes (v2).

---

##  Requerimientos

### ✔ Requerimientos Funcionales
- Gestión de transacciones (crear, editar, eliminar).
- Resumen mensual dinámico.
- Validación automática.
- Exportación de reporte mensual (v2).

### ✔ Requerimientos No Funcionales
- Respuesta en <2 segundos.
- Interfaz clara y adaptable.
- Validación estricta de datos.

---

##  Tabla de Pruebas Funcionales

| ID | Prueba | Entrada | Resultado esperado |
|----|--------|---------|---------------------|
| CP01 | Registrar ingreso | Monto 120 | Ingreso agregado |
| CP02 | Gasto inválido | Monto “abc” | Error y rechazo |
| CP03 | Calcular balance | 500-300 | Balance = 200 |

---

##  Tipo de Mantenimiento Propuesto
**Perfectivo**, para mejorar la funcionalidad y experiencia del sistema mediante nuevas capacidades como exportación de reportes y gráficos.

---

##  Reflexión sobre Control de Versiones
GitHub permite mantener un historial claro del avance del proyecto, comparar versiones, corregir errores y colaborar eficazmente. Markdown facilita documentar de forma ligera, estructurada y compatible con GitHub.

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
