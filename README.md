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

1. **Carga y exploración del dataset**: lectura del archivo, inspección de estructura y tipos.
2. **Filtrado por categorías**: identificación de productos con términos como "processed", "snack", "soda", etc.
3. **Limpieza de texto**: función robusta para normalizar nombres de productos y categorías.
4. **Imputación de valores faltantes**: aplicación de estrategias como la media o cero según contexto.
5. **Estandarización**: normalización de variables numéricas con `StandardScaler`.
6. **Integración final**: unión de datos limpios numéricos y textuales para crear `df_modelo`.

## Ejecución

1. Clona este repositorio.
2. Descargar dataset de drive: https://drive.google.com/file/d/1vH7PDNwF9WzQ0TMhh-vPafP8JIj50HUV/view?usp=sharing
3. Asegúrate de tener todas las dependencias instaladas:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn unidecode
```

3. Abre y ejecuta el notebook `Preparacion_Datos.ipynb` en JupyterLab o VSCode.

## Resultados Esperados

- Un DataFrame preparado, con datos consistentes, sin valores nulos críticos, y listo para modelado o análisis estadístico.

## Autor

Anderson Fabian Blanco Jaimes
Este trabajo fue desarrollado como parte de una monografía de Ciencia de Datos.

