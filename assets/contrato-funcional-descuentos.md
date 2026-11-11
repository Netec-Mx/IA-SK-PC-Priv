# Contrato funcional didáctico: cálculo de descuentos

> **Naturaleza del documento:** especificación del ejercicio de las Prácticas 6 y 7. Describe una función didáctica; no define impuestos, moneda, precios de producción ni reglas comerciales de una organización.

## Función

`calcular_total(total, descuento_porcentaje=0)`

## Requisitos

- Mantener la compatibilidad con las llamadas existentes que proporcionan solo `total`.
- `total` debe ser numérico, no booleano y no negativo.
- `descuento_porcentaje` es opcional; si se omite, su valor es `0`.
- El descuento debe ser numérico, no booleano y estar entre `0` y `100`, inclusive.
- Un tipo incorrecto produce `TypeError`; un valor negativo para `total` o un descuento fuera del rango produce `ValueError`.
- Calcular el total descontado como `total * (1 - descuento_porcentaje / 100)` y redondear el resultado a dos decimales.

## Ejemplos de comportamiento

| Llamada | Resultado esperado |
|---|---:|
| `calcular_total(125.50)` | `125.50` |
| `calcular_total(200, 10)` | `180.00` |
| `calcular_total(50, 0)` | `50.00` |
| `calcular_total(50, 100)` | `0.00` |
| `calcular_total(50, -1)` | `ValueError` |
| `calcular_total(50, 101)` | `ValueError` |

Los valores mostrados con dos decimales expresan la precisión del resultado; los ejemplos pueden aparecer como números sin ceros finales en la salida de Python.

## Regresión de redondeo

La Práctica 7 introduce deliberadamente una regresión al quitar la precisión de dos decimales de la expresión de redondeo. Para `calcular_total(125.50, 10)`, el resultado debe ser `112.95`; un resultado de `113` indica la regresión del ejercicio. La corrección del fallo restaura el redondeo a dos decimales.

## Límites

- No se especifica una política de redondeo financiera más allá del uso de `round(..., 2)` indicado en el ejercicio.
- No infiera reglas de impuestos, moneda, descuentos acumulables, límites de precio ni tratamiento de valores no finitos que no estén definidos aquí.
- Las pruebas generadas no deben modificar el código de producción fuera del alcance autorizado por el laboratorio.

## Trazabilidad

Derivado del contrato de la [Práctica 6](../Capitulo03/Practica6.md) y del fallo controlado de redondeo de la [Práctica 7](../Capitulo03/Practica_7_Windows.md).
