# Aprendizaje Continuo con MNIST

## Descripción

Este proyecto explora el **aprendizaje continuo** mediante una red neuronal convolucional (CNN) entrenada con el conjunto de datos MNIST. El objetivo es estudiar el fenómeno del **olvido catastrófico**, que ocurre cuando un modelo pierde conocimiento de tareas anteriores al aprender nuevas tareas.

El conjunto de datos se divide en dos tareas:

* **Tarea A:** clasificación de los dígitos del 0 al 4.
* **Tarea B:** clasificación de los dígitos del 5 al 9.

## Métodos implementados

* **Naive:** entrenamiento secuencial sin mecanismos para conservar el conocimiento anterior.
* **Experience Replay:** reutilización de ejemplos de tareas anteriores durante el nuevo entrenamiento.
* **EWC (Elastic Weight Consolidation):** penalización de cambios en parámetros importantes para tareas previamente aprendidas.

## Tecnologías

* Python
* PyTorch y Torchvision
* NumPy y Pandas
* Matplotlib

## Instalación

Instala las dependencias con:

```bash
pip install torch torchvision matplotlib pandas numpy
```

## Ejecución

Abre y ejecuta el notebook de Jupyter en orden, desde la carga de los datos hasta la comparación final de resultados.

## Resultados

Se comparan la precisión de cada tarea antes y después del entrenamiento, el olvido de la Tarea A y la precisión promedio final. También se generan gráficos para visualizar el rendimiento y las diferencias entre los métodos.

## Objetivo

Comprender cómo distintas estrategias de aprendizaje continuo permiten equilibrar la adquisición de nuevos conocimientos con la conservación de los conocimientos previos.
