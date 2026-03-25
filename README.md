# EXAMENMODULO8DEEPLEARNING
Entrega Examen Modulo 8
# 👗 StyleNet: Clasificador Inteligente de Ropa (Deep Learning)

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-D00000?style=for-the-badge&logo=keras&logoColor=white)

Este proyecto desarrolla una solución basada en **Deep Learning** para el área de Ciencia de Datos de la tienda virtual **StyleNet**. El objetivo es automatizar la clasificación de imágenes de productos para mejorar la eficiencia operativa y reducir errores manuales de categorización.

## 📌 Situación Inicial
Actualmente, la categorización de prendas subidas por usuarios en StyleNet se realiza de forma manual. Este proyecto implementa una **Red Neuronal Convolucional (CNN)** capaz de identificar automáticamente 10 categorías de productos con una alta precisión.

## 🏗️ Arquitectura del Modelo
Se diseñó un modelo secuencial robusto con las siguientes características:
* **Extracción de Características:** Dos capas `Conv2D` (32 y 64 filtros) con `MaxPooling2D` y `BatchNormalization` para estabilizar el entrenamiento.
* **Regularización:** Se aplicó un **Dropout del 50%** para mitigar el sobreajuste (overfitting) y mejorar la generalización.
* **Clasificación:** Capas densas finales con activación **Softmax** para categorizar entre las 10 clases del dataset Fashion-MNIST.

**Total de parámetros:** 225,930.

## 📊 Rendimiento y Métricas
El modelo fue evaluado rigurosamente con los siguientes resultados:

| Métrica | Valor |
| :--- | :--- |
| **Exactitud en Entrenamiento** | 93.57% |
| **Exactitud en Validación** | 90.49% |
| **Exactitud en Test (Datos Invisibles)** | **90.28%** |

### Análisis Visual
* **Curvas de Aprendizaje:** El modelo muestra una convergencia rápida y estable hacia la época 10.
* **Matriz de Confusión:** Alta precisión en categorías como *Pantalones* (974) y *Sandalias* (987). Se identificaron confusiones menores entre *Camisas* y *Camisetas* debido a la resolución de 28x28 píxeles.

  ## 📉 Visualización del Entrenamiento

A continuación, se presentan las curvas de aprendizaje generadas durante las 10 épocas de entrenamiento del modelo de **StyleNet**.

### Entrenamiento del Modelo (Progreso General)
<p align="center">
  <img src="Entrenamiento del Modelo.png" alt="Progreso general del entrenamiento de StyleNet" width="600px">
</p>

### Métricas Detalladas: Precisión y Pérdida
<p align="center">
  <img src="Graficos Precision del Modelo y Perdida del Modelo.png" alt="Curvas de precisión y pérdida del modelo StyleNet" width="800px">
</p>

## 🔍 Análisis de Calidad: Matriz de Confusión

La siguiente matriz permite evaluar el desempeño del modelo clase por clase, identificando los aciertos y las confusiones marginales entre prendas similares.

<p align="center">
  <img src="Matriz de Confusion.png" alt="Matriz de Confusión del Clasificador StyleNet" width="700px">
</p>

## 🚀 Cómo ejecutar el proyecto
1. Clona este repositorio:
   ```bash
   git clone [https://github.com/tu-usuario/StyleNet-Classifier.git](https://github.com/tu-usuario/StyleNet-Classifier.git)

2- Intala las dependencias; pip install tensorflow matplotlib seaborn scikit-learn
**🛠️ Tecnologías Utilizadas**
Lenguaje: Python

Framework: TensorFlow / Keras

Visualización: Matplotlib & Seaborn

Dataset: Fashion-MNIST (Zalando Research)

👤 Autor
Cristóbal Hernández Labarca - Administrador Público ; Postitulo en DataScience.

