# Clasificación MNIST con un MLP en PyTorch

**Douglas · PDDS · IA machine learning**

Tarea: diagnóstico de underfitting y overfitting mediante curvas de aprendizaje.

- [Notebook resuelto, con respuestas y salidas](tarea_mlp_pytorch_resuelta.ipynb).
- [Abrir la entrega en Google Colab](https://colab.research.google.com/github/DouglasPrez/machine-learning-mlp-pytorch-mnist/blob/main/tarea_mlp_pytorch_resuelta.ipynb).
- [Notebook base del catedrático](base/tarea_mlp_pytorch_v2.ipynb).
- [Fuente original](https://colab.research.google.com/drive/1Q4hYTiOuLlSTDseO_yDd0e4jKkNEdh8N).

## Contenido

División reproducible de un pool de 10,000 imágenes: 8,000 para entrenamiento y
2,000 para validación. Las 10,000 imágenes del test oficial se reservan hasta
seleccionar el modelo final.

Los diez ejercicios comparan capacidad, épocas, early stopping manual, dropout,
weight decay, cantidad de datos, learning rate, Batch Normalization y activación.
El modelo final se elige entre tres intentos usando solamente la validación.

## Reproducir

En Colab, abrir el enlace anterior y ejecutar todas las celdas en orden.
Colab suele incluir las librerías; si faltan, usar la línea de instalación de la
sección 2. Las versiones locales exactas están en `requirements.txt`.

En un entorno local:

```bash
python -m venv .venv
# Activar .venv según el sistema operativo.
python -m pip install -r requirements.txt
python -m ipykernel install --user --name mlp-mnist --display-name "MLP MNIST"
```

Abrir el notebook con Jupyter o VS Code, elegir el kernel del entorno y usar
**Restart Kernel and Run All**. Se requiere conexión para la primera descarga
de MNIST. La ejecución registrada se realizó en CPU, con semilla 42 y cuatro
hilos de PyTorch. Las cifras pueden variar entre dispositivos o versiones.

## Evidencia

El notebook conserva sus salidas, tablas y gráficas. La carpeta `evidencias/`
incluye el resumen CSV, los historiales de cada época y la evaluación final JSON.
Las respuestas se redactan a partir de esos resultados observados.

El código de la sección 5 se conserva sin modificaciones. Se completan los
campos de la tarea y se agregan ajustes de entorno, selección documentada de
tres intentos y exportación de evidencia. La evaluación del test se ejecuta una
vez después de elegir el modelo; no se usa para reajustarlo.
