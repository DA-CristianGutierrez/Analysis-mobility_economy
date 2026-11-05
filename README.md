# Analysis-mobility_economy

Este repositorio contiene el análisis realizado durante el Sprint 5 del caso mobilidad y economia en América Latina.

El dataset `TomTom Traffic Index` incluye 1.004.464 registros de mobilidad y el dataset `OECD Cities` contiene 30 registros que representan el PIB en cada país incluido, con problemas de calidad diseñados para simular datos reales de ambas mediciones.

## 📂 Contenido del repositorio

- `S5 ladb_mobility_economy_project_student`
  → Notebook principal con limpieza, unión de las fuentes de información, distribuciones-gráficos y conclusiones.

## ▶ Cómo abrir el notebook en Google Colab

Haz clic en el siguiente botón:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/DA-CristianGutierrez/b0e23c933ff0dd9c657177d8a0e14155/s5-ladb_mobility_economy_project_student.ipynb)

o:

1. Abre el archivo `.ipynb` en GitHub
2. Haz clic en **Open in Colab**

## 📘 Cómo reproducir el análisis

1. Abre `S5 ladb_mobility_economy_project_student`
2. Ejecuta las celdas en orden
3. El notebook carga automáticamente el dataset desde `/data/` o desde un enlace público (según corresponda)

## 🧠 Objetivo del análisis

- Identificar problemas de calidad de datos
- Segmentar y agrupar datos y unir fuentes de información
- Analizar la correlación y patrones entre ambos datasets
- Generar insights para determinar inversiones necesarias
  
----------------------------------------------------------------------------------------------------------------------------------------
## Análisis de relación entre tráfico y productividad económica

En este proyecto analicé la existencia entre indicadores de tráfico en cuanto a movilidad urbana y productividad económica (PIB) en las principales ciudades de Latinoamérica en el año 2024. Realicé un cruce de información entre ambas fuentes de información mediante Python y Pandas para determinar si había una correlación directa. Finalmente identifiqué en qué ciudades es conveniente invertir en infraestructura de transporte con el fin de mejorar la calidad de vida de las personas y aumentar la productividad económica.
Herramientas y tipo de proyecto

•	Problema: Identificar en qué ciudades invertir en infraestructura de transporte para mejorar la productividad y el bienestar de la población.
•	Acción: Crucé datos de tráfico de TomTom con indicadores económicos de la OECD usando Python y Pandas.
•	Resultado o aprendizaje: Identifiqué la relación directa entre el retraso por congestión y la caída en el desempeño económico urbano.


## 🛠️ Skills:
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3776AB?style=for-the-badge&logo=matplotlib&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-3776AB?style=for-the-badge&logo=seaborn&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)


## Metodología
•	Procesamiento de datos: se limpiaron y estandarizaron los datos, eliminando duplicados, renombrando columnas, transformando tipos de datos a formato fecha y decimales respectivamente.
•	Agrupación de datos: Se calcularon nuevas columnas empatando columnas clave en los dos DataFrames y se filtró y agrupó la información clave.
•	Unión de tablas: Se combinaron los dos Dataframes en una sola tabla para proceder con la visualización y análisis de los datos obtenidos.

## Visualizaciones destacadas
1.	Diagrama en tiempos de tráfico: Incialmente se encontró un valor atípico que se encuentra aislado del extremo superior o valores máximos en el diagrama. A su vez estos valores del extremo superior se alejan de la mediana y de los cuartiles evidenciando una brecha significativa entre las mediciones.  


<img width="739" height="566" alt="image" src="https://github.com/user-attachments/assets/360506c4-1ae0-4036-9e58-808defbdb17d" />

2.	Histograma del PIB per capita en 2024: Gran parte de las mediciones indican que la distribución se concentra más aproximadamente entre los 7.000 y los 17.000 USD per capita. Sin embargo, existe un número considerable de registros, los cuales se alejan de los más concentrados que no sobrepasan los 5.000 USD y otros que redondean los 25.000 USD.

<img width="748" height="492" alt="image" src="https://github.com/user-attachments/assets/0a2d0dea-f0d9-4fb4-bbc8-b87557143ef4" />


3.	Gráfico relación tráfico – Desarrollo PIB: Observamos ejemplo claros de países que tienen un gran desarrollo económico pero entre ellos difiere el promedio en tráfico, de la misma manera que sucede entre los países con un desarrollo económico bajo registrando altos y bajos niveles de tráfico. 


<img width="747" height="641" alt="image" src="https://github.com/user-attachments/assets/3a744388-db56-4635-a516-d91b2df7d067" />

## Conclusiones y recomendaciones
Correlación entre tráfico y desarrollo económico: no existe una estricta relación entre productividad económica y movilidad urbana ya que no existe una proporción uniforme en países que tienen valores similares en una métrica y en otra existen diferencias considerables.
Acciones recomendadas: 
•	Es necesario revisar las fuentes de información para descartar imprecisiones en los resultados. 
•	Considerar otras variables como el desarrollo de infraestructura en las ciudades evaluadas, así como la tendencia en las actividades económicas que se desarrollan respectivamente. 
•	De igual manera, considerar una inversión para el desarrollo de infraestructura en ciudades como Santiago, donde el tráfico es crítico y su baja economía pueda impedir una mejora en la calidad de transporte.
