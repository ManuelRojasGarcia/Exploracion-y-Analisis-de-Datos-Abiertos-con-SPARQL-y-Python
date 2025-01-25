# 📊 Exploración y Análisis de Datos Abiertos con SPARQL y Python 

## 📚 Contenidos

1. [Introducción](#introducción)
2. [Apartado 5 - DBPedia](#apartado-5---dbpedia)
   - [Wrapper para SPARQL](#11-crear-un-wrapper-para-sparql)
   - [Conversión de resultados a DataFrame](#12-dataframes-funciones-auxiliares-y-cómo-utilizar-dbpedia)
3. [Apartado 6 - Proyecto libre con datos abiertos](#apartado-6---proyecto-libre-con-datos-abiertos)
   - [Selección del conjunto de datos](#1-selección-del-conjunto-de-datos)
   - [Exploración de los datos](#2-exploración-de-los-datos)
   - [Conclusiones](#3-resumen-y-conclusiones)
4. [Instalación y uso](#instalación-y-uso)
5. [Estructura del repositorio](#estructura-del-repositorio)
6. [Tecnologías utilizadas](#tecnologías-utilizadas)
7. [Licencia](#licencia)

---

## 📝 Introducción

Este repositorio contiene la resolución de la PEC 4, enfocada en el análisis de datos abiertos utilizando SPARQL para consultar la base de datos de DBPedia, así como un proyecto de exploración de datos abiertos del Instituto Nacional de Estadística (INE).

Se abordan los siguientes temas:

- **Consultas SPARQL a DBPedia**
- **Procesamiento de datos JSON en Pandas**
- **Visualización y análisis de datos abiertos**

---

## 🏛️ Apartado 5 - DBPedia

### 📄 1.1 Crear un wrapper para SPARQL

Se desarrolla un wrapper para interactuar con un endpoint SPARQL que permite realizar consultas sobre los datos de DBPedia, estructurándolos en un grafo para exploración.

**Tecnologías utilizadas:**
- `SPARQLWrapper` para conectar con la API de DBPedia.
- `pandas` para la manipulación de datos obtenidos.

### 📄 1.2 Dataframes, funciones auxiliares y cómo utilizar DBPedia

Se transforma el resultado de las consultas SPARQL de formato JSON a DataFrames de Pandas, facilitando el análisis posterior.

**Archivos relevantes:**
- `sparql_wrapper.py` (funciones para realizar consultas y formatear resultados).
- `dbpedia_analysis.ipynb` (notebook con ejemplos de consulta y análisis).

---

## 🌍 Apartado 6 - Proyecto libre con datos abiertos

### 📄 1. Selección del conjunto de datos

Se seleccionó un conjunto de datos de **viviendas turísticas en España** del portal del INE.

- **Motivo:** Analizar la evolución del turismo en España.
- **Fuente:** [INE - Viviendas Turísticas](https://www.ine.es/jaxiT3/Datos.htm?t=2881)
- **Formato:** CSV
- **Dimensión:** Datos desde el año 2000 hasta la actualidad.

### 📄 2. Exploración de los datos

Se realiza la carga y limpieza de datos, exploración de variables y generación de gráficas para identificar patrones.

**Tareas realizadas:**
- Carga de datos con `pandas`.
- Visualización con `matplotlib` y `seaborn`.
- Análisis de tendencias de crecimiento de viviendas turísticas por comunidad autónoma.

### 📄 3. Resumen y conclusiones

Se resumen los hallazgos clave sobre la evolución de viviendas turísticas y se proponen consideraciones futuras basadas en los datos analizados.

---

## ⚙️ Instalación y uso

Para ejecutar los scripts de este repositorio, instala las dependencias necesarias:

```bash
pip install pandas requests sparqlwrapper matplotlib seaborn
