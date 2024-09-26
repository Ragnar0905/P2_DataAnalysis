# Análisis Exploratorio de Datos y KPI para Acceso a Internet 
 ![DALL·E 2024-09-26 08 57 52 - A modern and professional logo featuring a single 'H' for a telecommunications company  The design should incorporate subtle elements of telecommunica](https://github.com/user-attachments/assets/0679cc80-7069-48e1-988d-cb5fa920709b)

## Descripcion general
Bienvenidos este es un repositorio usado para la elboración de un estudio de una empresa de telecomunicaciones conocida en Argentina la cual nos pide realizar un **analisis exploratorio de los datos** (EDA), realizar diferentes **KPI's** para obtener información futura de sus ventas a traves de los años y de sus incrementos en ingresos, además para mayor visualización de los datos se organiza esto en una **herramienta de visualización** (PowerBI)

## Índice

- [Análisis Exploratorio de Datos y KPI para Acceso a Internet](#análisis-exploratorio-de-datos-y-kpi-para-acceso-a-internet)
  - [Descripcion general](#descripcion-general)
  - [Índice](#índice)
  - [Introducción](#introducción)
  - [Estructura del Repositorio](#estructura-del-repositorio)
  - [Análisis Exploratorio de Datos (EDA)](#análisis-exploratorio-de-datos-eda)
  - [KPI's Propuestos](#kpis-propuestos)
    - [KPI 1: Tasa de Penetración](#kpi-1-tasa-de-penetración)
    - [KPI 2: Crecimiento en Acceso a Internet](#kpi-2-crecimiento-en-acceso-a-internet)
    - [KPI 3: Aumento de Velocidad](#kpi-3-aumento-de-velocidad)
  - [Reporte de Análisis y Dashboards](#reporte-de-análisis-y-dashboards)
  - [Conclusiones](#conclusiones)
  - [Instalación y Uso](#instalación-y-uso)
    - [Requisitos](#requisitos)
    - [Instalación](#instalación)
  - [Contacto](#contacto)

![Portada_telecomunicaciones](https://github.com/user-attachments/assets/8ce6ce85-a27e-4685-86c3-2ba6911ae1c8)

---

## Introducción 

Este proyecto se centra en analizar la evolución del acceso a Internet por hogar, velocidad de conexión y diferentes tecnologías utilizadas, a lo largo de los años y trimestres, utilizando un archivo de datos en Excel. El objetivo es presentar un **Análisis Exploratorio de Datos (EDA)**, calcular **KPI's clave** para el monitoreo de tendencias, y visualizar los resultados de manera efectiva mediante **dashboards interactivos en Power BI**.

---

## Estructura del Repositorio

El repositorio está organizado de la siguiente manera:

- **data/**: Contiene el archivo de datos utilizado para el análisis (`Internet.xlsx`, `telefonia_fija.xlsx`, `Television.xlsx`).
- **notebooks/**: Scripts de Python utilizados para el **EDA** y el cálculo de **KPI's**.
    - `EDA_y_KPI.ipynb`: Codigo utilizado para realizar el analisis y visualización de los datos de manera exploratoria, además para calcular los **KPI's** propuestos.
- **dashboards/**: Contiene el archivo de Power BI (`Telecomunicaciones_Henry.pbix`) con las visualizaciones y dashboards interactivos.
- **README.md**: Este archivo de documentación que detalla el contenido y los análisis realizados.

---

## Análisis Exploratorio de Datos (EDA)

El **EDA** fue realizado utilizando **Python** con las librerías `pandas`, `seaborn`, y `matplotlib`. A continuación, se resumen los principales análisis y pasos realizados:

- **Carga y limpieza de datos**: Se importaron las hojas del archivo Excel y se realizó la limpieza básica, identificando valores faltantes, duplicados y outliers.
- **Visualizaciones exploratorias**:
    - Gráficos de **distribución** para ver la evolución de los accesos a Internet por trimestres y años.
    - **Boxplots** para identificar posibles outliers.
    - Gráficos de **barras** para comparar en los diferentes años y trimestres la tecnologia, velocidad, ingresos entre otros análisis.

El objetivo del EDA fue obtener una comprensión general de la estructura de los datos, identificar patrones y establecer una base sólida para el desarrollo de los **KPI's**.

---

## KPI's Propuestos

Se desarrollaron tres KPI's principales para medir diferentes aspectos del acceso a Internet:

### KPI 1: Tasa de Penetración
**Objetivo**: Medir el porcentaje de hogares con acceso a Internet por año y trimestre.

**Cálculo**:
\[
\text{Tasa de Penetración} = \frac{\text{Acceso a Internet}}{\text{Hogares Totales}} \times 100
\]

**Visualización**: La tasa de penetración se visualizó a través de gráficos de líneas para observar su evolución a lo largo de los años.

---

### KPI 2: Crecimiento en Acceso a Internet
**Objetivo**: Evaluar el crecimiento en el acceso a Internet para el próximo trimestre en relación al trimestre actual.

**Cálculo**:
\[
\text{Crecimiento en Acceso} = \frac{\text{Nuevo Acceso} - \text{Acceso Actual}}{\text{Acceso Actual}} \times 100
\]

**Visualización**: Se generaron gráficos de barras para comparar el crecimiento por año y trimestre, destacando picos y tendencias.

---


### KPI 3: Aumento de Velocidad
**Objetivo**: Evaluar el cambio porcentual en la velocidad promedio de acceso a Internet por trimestre.

**Cálculo**:
- Se asignaron valores ponderados a los rangos de velocidad de acceso (e.g., hasta 512 kbps, entre 1 Mbps y 6 Mbps).
- Se calculó una **Velocidad Promedio Ponderada** utilizando los accesos por rango y su respectiva ponderación.
- Finalmente, se midió el crecimiento porcentual de la velocidad promedio.

\[
\text{Velocidad Promedio} = \frac{\sum(\text{Accesos} \times \text{Velocidad})}{\text{Total de Accesos}}
\]

**Visualización**: Gráficos de líneas para mostrar el aumento en la velocidad promedio a lo largo de los trimestres.

---

## Reporte de Análisis y Dashboards

El **archivo de Power BI** (`Telecomuniaciones_Henry.pbix`) contiene varios dashboards interactivos con visualizaciones para analizar las tendencias y los KPI's:

1. **Tipos de Tecnología**: Muestra cómo diferentes tecnologías (ADSL, Cablemodem, etc.) han contribuido al acceso a Internet en diferentes años y trimestres.
2. **KPI's**: Visualiza cómo ha cambiado la tasa de penetración, el aumento de la velocidad y comparacion entre las penetraciones de Internet en los hogares a lo largo del tiempo.
3. **Velocidad Promedio**: Analiza la evolución de las velocidades de acceso a Internet y su cambio porcentual por trimestre y por provincia.
4. **Ingresos Totales**: Visualiza el incremento del precio del internet y compara que servicio ofrece mas ganancias para la empresa **Tv**, **Telefonia** e **Internet**

Cada visualización permite aplicar **filtros** para explorar los datos por provincia, tecnología, año y trimestre.

---

## Conclusiones

1. **Aumento en la Tasa de Penetración**: La tasa de acceso a Internet ha mostrado un crecimiento sostenido a lo largo de los años, con variaciones según el trimestre.
2. **Incremento de Velocidades Altas**: Se observó un aumento significativo en la adopción de velocidades superiores a 30 Mbps, lo que indica mejoras en la infraestructura y demanda de mayores velocidades.
3. **Variabilidad entre Tecnologías**: Cada tecnología de acceso (e.g., ADSL, Fibra óptica) muestra tendencias diferentes en cuanto a crecimiento, pero se logra observar como la tecnologia del cablemodem y la fibra optica estan agarrando fuerzas despues de la temporada de pandemia.

Estos hallazgos proporcionan una visión clara de las tendencias de acceso a Internet y ofrecen métricas valiosas para futuros análisis y toma de decisiones.

---

## Instalación y Uso

### Requisitos
- **Python 3.11** con las librerías `pandas`, `matplotlib`, y `seaborn`. **(Estas se encuentran en el archivo de Requirements.txt)**
- **Power BI Desktop**.

### Instalación
1. Clona el repositorio:
    ```bash
    git clone https://github.com/tu_usuario/nombre_repositorio.git
    ```

2. Instala las dependencias de Python:
    ```bash
    pip install pandas matplotlib seaborn
    ```
    O tambien puedes hacer con el requirements.txt
    ```bash
    pip install Requirements.txt
    ```

3. Abre el archivo de Power BI para explorar los dashboards:
    - Ubica el archivo `Telecomunicaciones_Henry.pbix` .
    - Ábrelo con **Power BI Desktop**.

---

## Contacto

Si tienes preguntas, comentarios, o deseas contribuir a este proyecto, no dudes en contactarme a [santiagomejiag.smg@gmail.com](mailto:santiagomejiag.smg@gmail.com).

---
