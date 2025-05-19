# Preparación de Datos - Ciencia de Datos

Este proyecto forma parte de una monografía para la especializacion de Analitica y Ciencia de Datos de la Universidad de Antioquia. Se centra en la preparación de un conjunto de datos de productos alimenticios.

## Objetivo

- Limpiar y transformar un conjunto de datos nutricionales.
- Filtrar productos procesados y ultraprocesados mediante criterios textuales.
- Estandarizar variables nutricionales para análisis.
- Integrar datos numéricos y categóricos para futuras etapas de modelado o visualización.

## Estructura del Proyecto

- `Preparacion_Datos.ipynb`: Notebook principal con todo el flujo de preparación, limpieza y transformación.

## Tecnologías Utilizadas

- Python 3.x
- Pandas
- NumPy
- Scikit-learn
- Matplotlib / Seaborn
- Expresiones regulares (re)
- Unidecode

## Pasos Realizados

1. **Carga y exploración del dataset**  
2. **Limpieza de datos** (eliminación de registros vacíos y columnas irrelevantes)  
3. **Imputación de valores faltantes** (media o cero según contexto)  
4. **Normalización de variables numéricas** (`StandardScaler`)  
5. **Generación de variable objetivo `apto`**  
   - Apto = 1 si:
     - `sugars_100g` ≤ 5  
     - `saturated_fat_100g` ≤ 3  
     - `sodium_100g` ≤ 120  
6. **Exportación del dataset limpio (`dataset_limpio.csv`)**

## Ejecución

1. Clona este repositorio.
2. Descargar dataset de drive: https://drive.google.com/file/d/1vH7PDNwF9WzQ0TMhh-vPafP8JIj50HUV/view?usp=sharing
3. Asegúrate de tener todas las dependencias instaladas:

3. Abre y ejecuta el notebook `Preparacion_Datos.ipynb` en JupyterLab o VSCode.

## Resultados Esperados

- Un DataFrame preparado, con datos consistentes, sin valores nulos críticos, y listo para modelado o análisis estadístico.

---

El notebook también incluye:

- Histogramas de variables como `sugars_100g`
- Boxplots para detección de outliers
- Matriz de correlación entre nutrientes
- Visualización de la distribución de clases (`apto` vs `no apto`)

---

## Autor

Anderson Fabian Blanco Jaimes

