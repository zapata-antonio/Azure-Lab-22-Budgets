# Lab 22 – Alertas de Presupuesto (Cost Management)

## Objetivo
Configurar un presupuesto en Azure para controlar el gasto y recibir avisos antes de llegar a un límite, evitando sorpresas en la factura.

---

## Qué he hecho en este laboratorio

1. He creado un presupuesto mensual de 10€ en Cost Management.
2. He configurado alertas automáticas para que me avisen al alcanzar el 50% del presupuesto.
3. He verificado que el presupuesto queda activo y visible en el panel de Cost Management.

---

## Arquitectura y concepto

Los Budgets de Azure permiten definir límites de gasto por periodo (mensual, trimestral, anual) y lanzar alertas cuando se alcanzan determinados umbrales.

Esto es una práctica básica de gobernanza financiera en cloud: no reduce el coste por sí mismo, pero ayuda a detectar desviaciones a tiempo y actuar (apagar recursos, optimizar SKUs, revisar gastos inesperados, etc.).

---

## Configuración utilizada

- Ámbito: Suscripción (Cost Management)
- Presupuesto: 10€ (mensual)
- Umbral de alerta: 50%
- Notificación: Email

---

## Validación funcional

Se ha comprobado que el presupuesto está creado, activo y con su línea de límite visible en el gráfico, y que la regla de alerta queda configurada con el umbral definido.

---

## Evidencias

### 01 – Presupuesto creado y visible en el gráfico
<img src="images/01-budget-overview.png" width="800">

Se muestra el presupuesto con el límite marcado en el gráfico (línea de presupuesto).

---

### 02 – Configuración de alertas (50%) con notificación por email
<img src="images/02-budget-alerts.png" width="800">

Se muestra la regla de alerta configurada al 50% del presupuesto y el método de notificación.

---

## Checklist de verificación

- [x] Presupuesto creado (10€)
- [x] Ámbito correcto (suscripción)
- [x] Alerta configurada al 50%
- [x] Notificación por email configurada
- [x] Evidencias guardadas y enlazadas en el README

---

## Qué le diría a un cliente o en entrevista

“La gobernanza cloud incluye el control de costes. Con budgets y alertas puedo detectar a tiempo cuándo un entorno se está desviando del gasto esperado y actuar antes de que llegue la factura.”

---

