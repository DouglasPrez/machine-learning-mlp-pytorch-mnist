# Revisión de los criterios de entrega

Revisión: 12 de noviembre de 2026. Referencia: rúbrica del notebook base del
catedrático. Esta revisión comprueba cobertura; no asigna una calificación.

| Bloque de la rúbrica | Peso | Comprobación | Estado |
|---|---:|---|---|
| Sección 4: split correcto y respuestas | 10 | 8,000 muestras de train y 2,000 de validation, semilla 42, verificación sin solapamiento y cuatro respuestas, incluido el reto opcional. | Cubierto |
| Ejercicios 1–10: ejecución | 20 | Las celdas están ejecutadas en orden, con salidas y gráficas conservadas, sin salidas de error. | Cubierto |
| Ejercicios 1–10: diagnóstico con números | 30 | Cada ejercicio incluye diagnósticos, accuracy/loss de train y validation, y brecha. Las comparaciones incluyen todos los valores probados. | Cubierto |
| Ejercicios 1–10: respuestas y conclusión | 30 | Las 39 preguntas de los diez ejercicios tienen respuesta; cada ejercicio contiene una conclusión. Redacción de las respuestas en primera persona. | Cubierto |
| Reflexión final | 10 | Tabla de remedios con referencias a los ejercicios, analogía del estudiante, cambio de mayor efecto y función de train/validation/test. | Cubierto |
| **Total de criterios cubiertos** | **100** | **Sin apartados obligatorios pendientes.** | **Revisado** |

## Condiciones adicionales

- La sección 5 conserva el código original del catedrático.
- Se realizaron tres intentos finales; el límite era cinco.
- La elección del modelo se realizó con validación antes de evaluar el test.
- Se conserva la única evaluación de test de la ejecución registrada: 95.37 %.
- La revisión posterior cambió solamente respuestas en Markdown y documentación;
  no modificó código, salidas, métricas ni volvió a ejecutar el test.
- Se contrastaron los diagnósticos con los historiales, sin forzar que los
  resultados coincidieran con los efectos esperados de cada hiperparámetro.
- En el ejercicio 2, ocho neuronas se clasifican como sobreajuste leve: train
  94.12 %, validation 89.45 %, brecha 4.68 pp y val loss final 0.3818 frente
  a su mínimo 0.3700. La explicación distingue capacidad limitada de sobreajuste.
- El modelo final se describe con su brecha residual de 3.86 pp; no se afirma
  que eliminó completamente el sobreajuste.

## Alcance de la revisión

La rúbrica no establece una accuracy mínima obligatoria ni exige consumir los
cinco intentos. Evalúa ejecución, diagnósticos fundamentados, respuestas y
reflexión. La entrega aporta evidencia para esos criterios; la valoración de
las explicaciones y la calificación definitiva corresponden al catedrático.

El registro técnico se encuentra en `verificacion.json`; las métricas y curvas
por época se pueden contrastar con `historiales.json` y con el notebook ejecutado.
