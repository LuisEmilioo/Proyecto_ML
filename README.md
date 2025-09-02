        ![Espectrograma Cuphead](https://github.com/LuisEmilioo/Proyecto_ML/blob/main/SPCTGRMA.jpg?raw=true)
# 🎶 Clasificación de Sonidos con Espectrogramas

Este proyecto utiliza técnicas de Machine Learning y Deep Learning para la clasificación de sonidos a partir del dataset [UrbanSound8K](https://urbansounddataset.weebly.com/urbansound8k.html).  
El enfoque principal es convertir los audios en representaciones visuales (espectrogramas) que permiten a una red neuronal convolucional (CNN) identificar patrones característicos de cada clase de sonido.

---

## 🚀 Objetivos
- Preprocesar datos de audio (archivos WAV).
- Extraer propiedades básicas de los audios (canales, sample rate, bit depth).
- Transformar los audios en espectrogramas para su análisis.
- Entrenar un modelo de red neuronal para clasificar diferentes tipos de sonidos urbanos.
- Evaluar el rendimiento del modelo con métricas estándar.

---

## 🛠️ Tecnologías y Librerías
- **librosa**: procesamiento y análisis de audio.
- **matplotlib**: visualización de espectrogramas.
- **numpy**: manejo de arreglos numéricos.
- **pandas**: manejo de datasets.
- **sklearn**: codificación de etiquetas, división de datos y métricas de evaluación.
- **keras / tensorflow**: construcción y entrenamiento de redes neuronales.
- **os / struct**: manejo de archivos WAV y propiedades técnicas.

---

## 📂 Dataset
Se emplea el dataset **UrbanSound8K**, que contiene **8732 clips de audio** etiquetados en 10 categorías de sonidos urbanos, como:
- Sirenas 🚨  
- Claxon de coches 🚗📢  
- Ladridos 🐕  
- Perforadoras 🔨  
- Música 🎵  

Para pruebas iniciales, se utilizó una muestra de 200 registros.

---

## 🔎 Flujo del Proyecto
1. **Carga de datos**: lectura del CSV con metadatos de los audios.  
2. **Extracción de propiedades**: número de canales, frecuencia de muestreo y profundidad de bits.  
3. **Transformación a espectrogramas**: representación visual de cada audio.  
4. **Preprocesamiento**: normalización y codificación de etiquetas.  
5. **Construcción del modelo CNN**:
   - Capas convolucionales para detectar patrones.
   - MaxPooling para reducir dimensionalidad.
   - Dropout para evitar sobreajuste.
6. **Entrenamiento** del modelo con los espectrogramas.  
7. **Evaluación** mediante métricas como precisión, recall y f1-score.  

---

## 📊 Resultados
- El modelo logra distinguir varias clases de sonidos urbanos con un desempeño inicial aceptable.  
- Existen retos en mejorar la precisión, especialmente en clases con menor representación en el dataset.  

