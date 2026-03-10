# Challenge-Alura-Telecom-X
Penúltimo challenge de la formación Data Science de Alura LATAM

# 📊 Análisis de Evasión de Clientes (Churn) - Telecom X

![Status](https://img.shields.io/badge/Status-Finalizado-success)
![Python](https://img.shields.io/badge/Python-3.9+-blue)
![Pandas](https://img.shields.io/badge/Library-Pandas-orange)
![Seaborn](https://img.shields.io/badge/Visualization-Seaborn-green)

## 📝 Descripción del Proyecto
Este proyecto se enfoca en el análisis de datos de **Telecom X** para identificar los factores que influyen en la deserción de clientes (*Churn*). A través de un proceso de ETL y Análisis Exploratorio de Datos (EDA), se detectaron patrones críticos en el comportamiento de los usuarios, permitiendo formular recomendaciones estratégicas basadas en evidencia para reducir la pérdida de ingresos.

## 🛠️ Stack Tecnológico
* **Lenguaje:** Python 3.x
* **Entorno:** Google Colab
* **Librerías Principales:** * `Pandas`: Manipulación y limpieza de datos.
    * `NumPy`: Operaciones numéricas y manejo de valores nulos.
    * `Matplotlib` & `Seaborn`: Visualización de datos estadísticos.
    * `Requests` / `JSON`: Ingesta de datos desde fuentes semiestructuradas.

## 🚀 Flujo de Trabajo (Pipeline)

### 1. Ingesta y Normalización
Los datos originales se encontraban en formato **JSON anidado**. Se realizó un proceso de aplanamiento (*flattening*) para transformar la estructura jerárquica en un DataFrame relacional listo para el análisis.

### 2. Limpieza y Transformación (Data Wrangling)
* **Tratamiento de Nulos:** Identificación y corrección de valores ausentes en la facturación total (`TotalCharges`).
* **Tipado de Datos:** Conversión de variables de tipo objeto a numérico para análisis estadístico.
* **Feature Engineering:** Creación de la métrica `Cuentas_Diarias` para normalizar el costo del servicio por día.
* **Estandarización:** Traducción de variables al español y binarización de categorías críticas (Yes/No a 1/0).

### 3. Análisis Exploratorio (EDA)
Se realizaron cruces de variables para validar hipótesis de negocio:
* **Variables Categóricas:** Análisis de deserción según tipo de contrato y servicios de internet.
* **Variables Numéricas:** Estudio de la distribución de antigüedad (*Tenure*) y cargos mensuales mediante diagramas de caja (Boxplots) y densidad.



## 📈 Hallazgos Principales
* **Vulnerabilidad Contractual:** Los clientes con contratos mes a mes presentan la tasa de evasión más alta.
* **Segmento Crítico:** Los usuarios de fibra óptica con facturas superiores al promedio tienen un riesgo de fuga incrementado en un 30%.
* **Periodo de Retención:** La mayor probabilidad de churn ocurre en los primeros 12 meses de servicio.

## 💡 Recomendaciones Propuestas
1. Implementar programas de fidelización para clientes en su primer año.
2. Incentivar la migración de contratos mensuales a anuales mediante *upgrades* de servicio.
3. Auditar la calidad técnica de la infraestructura de Fibra Óptica en zonas de alta rotación.

## 📂 Estructura del Repositorio
* `Notebook_TelecomX.ipynb`: Notebook con el código completo, desde la carga hasta el informe final.
* `TelecomX_Data.json`: Dataset original utilizado en el análisis.
* `TelecomX_diccionario.md`: Diccionario de datos para referencia de variables.

---
**Desarrollado por:** [Tu Nombre]  
**Contacto:** [Enlace a tu LinkedIn o Correo]
