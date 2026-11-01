## Sistema predictivo para el apoyo a la planificación operativa en empresas de transporte de pasajeros

### Proyecto de Trabajo Final

Trabajo presentado para la materia **Seminario de Trabajo Final** de la **Licenciatura en Ciencia de Datos** de la **Universidad del Gran Rosario**.

#### Autores
- González Dupouy, Gustavo Gabriel
- Pretzsch, Néstor Alejandro

#### Cuerpo docente
- Prof. Alejandro Hernández
- Prof. Brian Alcides Gauna
- Prof. Jorge Fernández

---

### Descripción del proyecto

Este repositorio reúne los archivos utilizados para el desarrollo del Proyecto de Trabajo Final **“Sistema predictivo para el apoyo a la planificación operativa en empresas de transporte de pasajeros”**.
El trabajo aborda el desarrollo de un sistema predictivo aplicado a la planificación operativa de **ETAP**, a partir del análisis de registros históricos de viajes especiales y de variables externas que pueden aportar información al proceso de predicción.
El análisis se desarrolla en Python y se documenta en un notebook de Jupyter, donde se realiza el tratamiento de los datos, el análisis exploratorio, la construcción y evaluación de modelos y la generación de pronósticos.

### Objetivo

Desarrollar y evaluar un sistema predictivo que permita estimar la cantidad mensual de viajes especiales y utilizar los resultados como apoyo para la planificación operativa de una empresa de transporte de pasajeros.

### Metodología

El proyecto se estructura siguiendo la metodología **CRISP-DM**, contemplando las etapas de comprensión del problema, comprensión y preparación de los datos, modelado, evaluación y presentación de los resultados.
Para el análisis predictivo se consideran diferentes enfoques de series temporales y aprendizaje automático, entre ellos:
- Prophet
- SARIMA
- Random Forest
- XGBoost
La comparación entre modelos permite analizar su desempeño y seleccionar el enfoque más adecuado para la generación de pronósticos.

### Fuentes de datos

El proyecto utiliza registros históricos de viajes especiales y variables complementarias provenientes de distintas fuentes. Entre los archivos incluidos en el repositorio se encuentran datos asociados al nivel general de precios, tipo de cambio, actividad hotelera y registros históricos de la empresa.

### Estructura del repositorio

| Archivo | Descripción |
|---------|-------------|
| `Historial Viajes Especiales.xlsx` | Base histórica de viajes especiales utilizada como fuente principal del análisis. |
| `INDEC Historial.csv` | Datos históricos utilizados como variable externa en el análisis. |
| `IPC.csv` | Información correspondiente al Índice de Precios al Consumidor (IPC). |
| `Ocupacion Hotel.csv` | Información de ocupación hotelera utilizada como variable complementaria. |
| `Tipo de cambio (BCRA).xls` | Datos históricos del tipo de cambio utilizados como variable externa. |
| `Seminario_de_Trabajo_Final.ipynb` | Notebook principal del proyecto. Contiene el procesamiento de datos, análisis, modelado, evaluación y pronósticos. |
| `Tesis Gonzalez Dupouy - Pretzsch rev.4.docx` | Documento escrito del Proyecto de Trabajo Final. |

### Tecnologías utilizadas

El desarrollo del proyecto se realizó principalmente con:
- Python
- Jupyter Notebook / Google Colab
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Prophet
- Statsmodels
- XGBoost

### Ejecución del análisis

El análisis se encuentra centralizado en el archivo:
"Seminario_de_Trabajo_Final.ipynb"
Para reproducir el trabajo, deben estar disponibles los archivos de datos incluidos en este repositorio y ejecutarse las celdas del notebook en el orden establecido.

### Documento final

El desarrollo metodológico, los fundamentos, resultados y conclusiones del proyecto se encuentran documentados en el archivo de la tesis disponible en este repositorio.

### Fe de erratas: proyección Random Forest 2026–2027

Los totales anuales de Random Forest publicados en la tesina (apartados 9.3 y 10.3 y Tabla 14) no coinciden con la salida guardada del notebook.

| Año  | Tesina | Notebook (salida guardada) | Tesina − notebook | Diferencia s/ notebook |
|------|-------:|---------------------------:|------------------:|-----------------------:|
| 2026 | 410    | 377,6                      | 32,4              | 8,58 %                 |
| 2027 | 413    | 359,7                      | 53,3              | 14,82 %                |

- **Meses con mayor diferencia:** diciembre de 2026 (+13,3), septiembre de 2027 (+18,0) y diciembre de 2027 (+9,7).
- **Sin diferencias:** la línea base Naïve (rezago 12) coincide en los 24 meses, con 377 viajes por año.
- **Referencia en el notebook:** sección «Proyección mensual 2026–2027» (celda 39), tablas `df_proyeccion` y `df_totales_anuales`.
- **Qué corregir en la tesina:** reemplazar 410 y 413 por los totales del notebook, 377,6 y 359,7.

### Consideraciones sobre los datos

Los datos utilizados tienen fines académicos y forman parte del desarrollo del Trabajo Final. Su inclusión en este repositorio debe interpretarse dentro de ese contexto y respetando las condiciones de uso correspondientes a cada fuente de información.

---

**Universidad del Gran Rosario Licenciatura en Ciencia de Datos Seminario de Trabajo Final**
