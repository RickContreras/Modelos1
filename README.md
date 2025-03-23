# 📊 Modelos1 - Pruebas Saber Pro

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
![Python Version](https://img.shields.io/badge/python-3.12.5-blue.svg)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange)
![scikit-learn](https://img.shields.io/badge/scikit--learn-v1.5.1-blue)
![pandas](https://img.shields.io/badge/pandas-v2.2.2-blue)
![numpy](https://img.shields.io/badge/numpy-v2.1.0-blue)


¡Bienvenido al repositorio del curso de **Modelos 1** de la Universidad de Antioquia! 🎓 Aquí encontrarás todo lo relacionado con nuestro proyecto sobre las **Pruebas Saber Pro** en Colombia.

# Tabla de Contenido
- [👥 Participantes](#-participantes)
- [📹 Videos de Entrega](#-videos-de-entrega)
- [📋 Overview](#-overview)
- [📊 Descripción del Conjunto de Datos](#-descripción-del-conjunto-de-datos)
- [📈 Evaluación](#-evaluación)
- [📁 Formato del Archivo de Envío](#-formato-del-archivo-de-envío)
- [🗂️ Estructura del Proyecto](#️-estructura-del-proyecto)
- [🔖 Citation](#-citation)


## 👥 Participantes

- **Nombre:** Ricardo Contreras

- **Nombre:** Estiven Ospina González

- **Nombre:** Daniel León

## 📹 Videos de Entrega

- **Entrega 2**: <a href="https://youtu.be/Lfo4AFsae6A?si=8ObGC-U9c6mgJhSp" target="_blank">https://youtu.be/Lfo4AFsae6A?si=8ObGC-U9c6mgJhSp</a>
- **Entrega 3**: <a href="https://youtu.be/mk9bLfLd_zI" target="_blank">https://youtu.be/mk9bLfLd_zI</a>

## 📋 Overview

Las **Pruebas Saber Pro** son exámenes estandarizados que se realizan en Colombia para evaluar la calidad y el nivel de conocimiento de los estudiantes de educación superior. Estas pruebas son una iniciativa del Gobierno de Colombia para monitorear y mejorar la calidad de la educación superior en el país.

Las pruebas abarcan cinco componentes genéricos:

- **Inglés**
- **Lectura Crítica**
- **Competencias Ciudadanas**
- **Razonamiento Cuantitativo**
- **Comunicación Escrita**

Nuestro objetivo es crear un modelo de clasificación que prediga el desempeño de cada estudiante en estas pruebas, categorizándolos en: **bajo**, **medio-bajo**, **medio-alto** o **alto**.

## 📊 Descripción del Conjunto de Datos

El conjunto de datos incluye varias columnas que describen diferentes aspectos de cada estudiante, tales como:

- **Información Socioeconómica**: Características como el estrato socioeconómico, la educación de los padres, etc.
- **Información Académica**: Detalles como el programa de estudio del estudiante, entre otros.

En total, contamos con registros de casi **700,000 estudiantes**.

## 📈 Evaluación

Esta es una tarea de clasificación multi-clase con 4 categorías. La métrica de desempeño que utilizaremos será el **accuracy**, es decir, el porcentaje de predicciones correctas que realiza nuestro modelo.

## 📁 Formato del Archivo de Envío

Para cada ID en el archivo `test.csv`, debemos predecir el desempeño en la variable `RENDIMIENTO_GLOBAL`. El archivo de envío debe tener un encabezado y seguir el siguiente formato:

```csv
  ID,RENDIMIENTO_GLOBAL
  550236,bajo
  98545,alto
  499179,medio-bajo
```

Es crucial que el archivo de envío contenga los mismos IDs que están en el test.csv, ya que estos son los estudiantes con los que se evaluará el rendimiento de nuestro modelo.

## 🗂️ Estructura del Proyecto
```bash
  Modelos1/
  ├── .devcontainer/
  │   ├── devcontainer.json
  ├── data/
  │   ├── train.csv
  │   ├── test.csv
  ├── .gitignore
  ├── 01 - exploración.ipynb
  ├── 02 - preprocesado.ipynb
  ├── 03 - modelo con preprocesado de tal forma y SVM.ipynb
  ├── 04 - modelo con preprocesado de otra forma y Random Forest.ipynb
  ├── 99 - modelo solución.ipynb
  ├── requirements.txt
  ├── README.md
```

## 🔖 Citation

- RLX. (2024). UDEA/ai4eng 20242 - Pruebas Saber Pro Colombia. Kaggle. https://kaggle.com/competitions/udea-ai4eng-20242
