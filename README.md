# Lab 22 – Alertas de Presupuesto (Cost Management)

## Objetivo
Configurar un presupuesto en Azure para controlar el gasto y recibir avisos antes de llegar a un límite, evitando sorpresas en la factura.

---

## Qué he hecho en este laboratorio

1. He creado un presupuesto mensual llamado `budget-lab22-10eur` con un límite de 10 USD.
2. He configurado una alerta automática al 50% del presupuesto (5 USD) para recibir notificación por correo.
3. He verificado que el presupuesto queda activo y visible en Cost Management.

---

## Arquitectura y concepto

Los Budgets de Azure permiten definir límites de gasto por periodo (mensual, trimestral, anual) y lanzar alertas cuando se alcanzan umbrales.

Es una práctica de gobernanza financiera: no reduce el gasto por sí mismo, pero ayuda a detectar desviaciones a tiempo y actuar (revisar recursos, optimizar, apagar entornos de pruebas, etc.).

---

## Configuración utilizada

- Presupuesto: 10 USD (mensual)
- Umbral de alerta: 50% (5 USD)
- Tipo de alerta: Coste real
- Notificación: email
- Ámbito: Cost Management (cuenta de facturación)

---

## Validación funcional

Se ha comprobado que el presupuesto está creado y visible, y que la alerta al 50% queda configurada correctamente.

---

## Evidencias

### 01 – Presupuesto creado y visible
<img src="images/01-budget-overview.png" width="800">

Se muestra el presupuesto `budget-lab22-10eur` con el límite configurado.

---

### 02 – Alerta configurada al 50%
<img src="images/02-budget-alerts.png" width="800">

Se muestra la condición de alerta al 50% (5 USD) y la configuración de destinatarios.

---

## Checklist de verificación

- [x] Presupuesto creado (10 USD)
- [x] Periodicidad mensual
- [x] Alerta configurada al 50% (5 USD)
- [x] Notificación por email configurada


---

## Qué le diría a un cliente o en entrevista

“La gobernanza cloud incluye el control de costes. Con budgets y alertas puedo detectar a tiempo cuándo un entorno se desvía del gasto esperado y actuar antes de que llegue la factura.”

---
