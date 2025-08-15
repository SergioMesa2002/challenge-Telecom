# Análisis de Evasión de Clientes (Churn)

Este proyecto tiene como objetivo analizar los patrones de evasión de clientes (Churn) en una empresa proveedora de servicios. A través de un análisis exploratorio de datos, buscamos identificar las variables más relevantes que afectan la **evasión de clientes**, para tomar decisiones estratégicas que ayuden a reducir esta tasa.

## 🔹 Objetivo

El objetivo principal del análisis es comprender los factores que influyen en la **evasión de clientes (Churn)**. El análisis incluye la limpieza de datos, la creación de nuevas columnas, la exploración de datos y la visualización de patrones, lo cual proporcionará información útil para desarrollar estrategias de retención de clientes.

## 🔹 Pasos Realizados

### 1. **Limpieza y Tratamiento de Datos**
- **Importación de los datos**: Los datos fueron importados desde un archivo JSON.
- **Aplanado de estructura**: Se utilizó `json_normalize` para convertir las columnas anidadas en un formato más accesible.
- **Renombrado de columnas**: Se cambiaron los nombres de las columnas para eliminar prefijos innecesarios y facilitar la comprensión.
- **Transformación de datos categóricos**: Se transformaron las variables **`Yes/No`** a valores binarios (1 y 0).
- **Creación de nuevas columnas**: Se añadió la columna **`Cuentas_Diarias`**, que convierte el gasto mensual en un gasto diario promedio.

### 2. **Análisis Exploratorio de Datos**
- **Distribución de Churn**: Se exploró la distribución de la variable objetivo `Churn` para entender cuántos clientes se fueron y cuántos permanecieron.
- **Variables Categóricas**: Se analizó cómo variables como `Contract`, `PaymentMethod`, `InternetService`, entre otras, se distribuyen entre los clientes que se fueron y los que permanecieron.
- **Variables Numéricas**: Se analizó la relación entre variables numéricas como **`Factura_Total`** y **`Meses_Contrato`** con respecto a la evasión de clientes.

### 3. **Visualizaciones**
- **Gráficos de barras**: Se utilizaron gráficos de barras para mostrar la distribución de la evasión de clientes según diferentes variables categóricas (como `Contract`, `PaymentMethod`, etc.).
- **Boxplots**: Se generaron boxplots para visualizar cómo variables numéricas como **`Factura_Total`** y **`Meses_Contrato`** se distribuyen entre clientes que se fueron y los que permanecieron.

## 🔹 Resultados y Hallazgos

- **Clientes con contrato mensual** tienen una mayor tasa de evasión.
- **Métodos de pago como el cheque electrónico** están asociados con una mayor tasa de evasión.
- **Clientes con menos antigüedad** tienen más probabilidades de cancelar el servicio.
- Los **clientes con mayor gasto** tienden a quedarse más tiempo, lo que sugiere que **el gasto más alto está relacionado con mayor lealtad**.

## 🔹 Recomendaciones

1. **Fomentar contratos largos**: Ofrecer incentivos a los clientes con contrato mensual para que firmen contratos más largos.
2. **Cambiar métodos de pago**: Incentivar a los clientes a usar métodos de pago automáticos (tarjetas de crédito, transferencias bancarias).
3. **Aumentar la fidelidad de clientes nuevos**: Ofrecer beneficios a los clientes con menos antigüedad para mejorar la retención.
4. **Monitorear a clientes con bajo gasto**: Identificar a los clientes con menor gasto y mayor probabilidad de evasión, para ofrecerles promociones personalizadas.

## 🔹 Archivos

- **`TelecomX_Data.json`**: Archivo de datos original con la información de los clientes.
- **`TelecomX_diccionario.md`**: Diccionario que describe el significado de cada variable.
- **`TelecomX_LATAM.ipynb`**: Notebook con el análisis realizado, desde la limpieza de datos hasta la creación de visualizaciones.

## 🔹 Cómo Ejecutar el Proyecto

1. Asegúrate de tener **Python 3** y las siguientes librerías instaladas:
    - pandas
    - matplotlib
    - seaborn

2. Descarga o clona este repositorio y abre el archivo **`TelecomX_LATAM.ipynb`** en **Google Colab** o en **Jupyter Notebook**.

3. Ejecuta las celdas del notebook en orden para realizar el análisis completo, desde la carga de los datos hasta la creación de los gráficos.

## 🔹 Contribuciones

Si deseas contribuir al proyecto, puedes abrir un **issue** o enviar un **pull request** con mejoras al código o nuevas ideas de análisis.

---

**Autor**: Sergio Mesa 
**Fecha**: 15 de agosto 2025
