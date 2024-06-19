# Bootcamp Tripleten
## Proyecto Sprint 14

Este repositorio contiene un proyecto en Python que entrena varios modelos de machine learning para clasificar reseñas de películas como positivas o negativas. Los modelos se basan en técnicas de procesamiento de lenguaje natural.

## Tabla de Contenidos

- [Descripción General](#descripción-general)
- [Características](#características)
- [Instalación](#instalación)
- [Modelos](#modelos)


## Descripción General

El objetivo de este proyecto es implementar y comparar diferentes modelos de machine learning para el análisis de sentimiento de reseñas de películas. Los modelos serán entrenados para clasificar las reseñas como positivas o negativas.

## Características

- Preprocesamiento de datos de texto
- Entrenamiento y evaluación de múltiples modelos
- Visualización del rendimiento de los modelos
- Comparación de resultados de los modelos

## Instalación

Para comenzar, clona el repositorio e instala las dependencias necesarias.

```bash
git clone git@github.com:joaquincardosorios/tripleten_14_ML_text.git
cd tripleten_14_ML_text
python3 -m venv .venv
source .venv/bin/activate # En Windows usa `.venv\Scripts\activate`
pip install -r requirements.txt
```

## Modelos

El proyecto utiliza varios modelos para la clasificación de reseñas de películas:

### Modelo Dummy (DummyClassifier)

El DummyClassifier es un modelo base que predice utilizando estrategias simples como la mayoría de clases o estrategias aleatorias. Se utiliza como punto de referencia para comparar con otros modelos más complejos.

### Modelo con NLTK, TF-IDF y Regresión Logística

Se utiliza NLTK (Natural Language Toolkit) para el procesamiento de texto y TF-IDF (Term Frequency-Inverse Document Frequency) para la extracción de características. Estas características se utilizan con un modelo de regresión logística para clasificar las reseñas como positivas o negativas.

### Modelo spaCy, TF-IDF y Regresión Logística

spaCy es utilizado para el procesamiento avanzado de lenguaje natural, mientras que TF-IDF se emplea para la extracción de características. Estas características se pasan a un modelo de regresión logística para la clasificación de sentimientos.

### Modelo spaCy, TF-IDF y LGBMClassifier

Se utiliza spaCy para el procesamiento de lenguaje natural y TF-IDF para la extracción de características. Estas características se utilizan con el LGBMClassifier, un modelo de Gradient Boosting, conocido por su eficiencia en conjuntos de datos grandes.

### Modelo BERT

BERT (Bidirectional Encoder Representations from Transformers) es un modelo de aprendizaje profundo basado en transformers que ha demostrado excelentes resultados en tareas de procesamiento de lenguaje natural, incluyendo la clasificación de sentimientos. Se utiliza para capturar representaciones contextuales de las reseñas de películas y realizar la clasificación de sentimientos.
