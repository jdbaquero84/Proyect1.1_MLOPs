# Proyecto MVP para Plataforma de Videojuegos

<div align="center">
    <img src="https://github.com/jdbaquero84/Proyect1.1_MLOPs/blob/master/show1.jpg" alt="Descripción de la Imagen 1" width="300"/>
    <img src="https://github.com/jdbaquero84/Proyect1.1_MLOPs/blob/master/show2.png" alt="Descripción de la Imagen 2" width="300"/>
    <img src="https://github.com/jdbaquero84/Proyect1.1_MLOPs/blob/master/show3.jpg" alt="Descripción de la Imagen 3" width="300"/>
</div>

## Resumen

Se trata de un MVP (Producto Mínimo Viable) usando bases de datos de una plataforma de videojuegos, con sus análisis exploratorios de datos (EDA) y procesos de extracción, transformación y carga (ETL) respectivos. Usando Render, se implementaron 5 endpoints y un sistema de recomendación basado en la similitud del coseno. El objetivo principal fue entregar una API que permite realizar diversas consultas sobre los datos de la plataforma de videojuegos.

## Tecnologías Utilizadas

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-D00000?style=for-the-badge&logo=keras&logoColor=white)
![SciPy](https://img.shields.io/badge/SciPy-8CAAE6?style=for-the-badge&logo=scipy&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-3776AB?style=for-the-badge&logo=seaborn&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)
![Render](https://img.shields.io/badge/Render-46E3B7?style=for-the-badge&logo=render&logoColor=white)

## Objetivo

El objetivo de este proyecto es proporcionar una API funcional y eficiente que permita realizar consultas detalladas sobre los datos de videojuegos, utilizando un modelo de recomendación basado en la similitud del coseno. Esta herramienta busca facilitar el acceso a información clave para usuarios y desarrolladores, mejorando la toma de decisiones y la experiencia del usuario.

## Similitud del Coseno

La similitud del coseno es una métrica utilizada para medir la similitud entre dos vectores en un espacio multidimensional. En el contexto de los sistemas de recomendación, se utiliza para comparar la similitud entre productos (en este caso, videojuegos) basándose en sus características. La fórmula de la similitud del coseno es:

$$
\text{Similitud del Coseno} = \frac{\vec{A} \cdot \vec{B}}{\|\vec{A}\| \|\vec{B}\|}
$$

donde:
- \(\vec{A}\) y \(\vec{B}\) son los vectores de características de los dos productos a comparar.
- \(\vec{A} \cdot \vec{B}\) es el producto punto de los vectores.
- \(\|\vec{A}\|\) y \(\|\vec{B}\|\) son las magnitudes de los vectores.

La similitud del coseno proporciona un valor entre -1 y 1, donde 1 indica que los productos son idénticos, 0 indica que no tienen similitudes y -1 indica que son completamente opuestos. Esta técnica es muy útil para recomendaciones porque toma en cuenta la dirección de los vectores y no la magnitud, lo que la hace robusta a diferentes escalas de datos.

<div align="center">
    <img src="https://github.com/jdbaquero84/Proyect1.1_MLOPs/blob/master/imagen1.png" alt="Descripción de la Imagen 2" width="300"/>
    <img src="https://github.com/jdbaquero84/Proyect1.1_MLOPs/blob/master/imagen2.jpg" alt="Descripción de la Imagen 3" width="300"/>
</div>

## Funcionalidades del API

Las consultas que se pueden realizar a través de la API son las siguientes:

1. **Cantidad de productos gratis por año y por empresa desarrolladora**:
   - Permite obtener el número de productos gratuitos lanzados por año y la empresa que los desarrolló.

2. **Cantidad de dinero gastada por el usuario, porcentaje de recomendación en las opiniones y número de items**:
   - Proporciona información sobre el gasto total del usuario, el porcentaje de recomendación basado en las opiniones de los usuarios y el número total de items.

3. **Top 3 de desarrolladores con juegos más recomendados por año**:
   - Devuelve los tres desarrolladores con los juegos más recomendados cada año.

4. **Diccionario de reseñas de usuarios por desarrollador**:
   - Según el desarrollador, se devuelve un diccionario con el nombre del desarrollador como llave y una lista con la cantidad total de registros de reseñas de usuarios categorizados como positivos o negativos.

5. **Sistema de recomendación**:
   - Ingresando el ID de un producto, se recibe una lista con 5 juegos recomendados similares al ingresado, basado en la similitud del coseno.

## Implementación

La implementación del proyecto incluye los siguientes componentes:
- **EDA (Análisis Exploratorio de Datos)**: Procesos y técnicas utilizadas para analizar y resumir los datos de la plataforma de videojuegos.
- **ETL (Extracción, Transformación y Carga)**: Procesos de manejo de datos para preparar la información necesaria para el análisis y la implementación del modelo.
- **Render**: Utilizado para desplegar y manejar los endpoints de la API.

[Ver fastAPI aquí](https://proyect1-1-mlops.onrender.com/docs#/)

