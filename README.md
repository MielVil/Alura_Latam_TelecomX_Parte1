# Alura_Latam_TelecomX_Parte1
# 📊 Análisis de Evasión de Clientes en TelecomX LATAM

Este proyecto analiza la **evasión de clientes (Churn)** en una compañía de telecomunicaciones, con el objetivo de identificar los factores más asociados a la cancelación del servicio y proponer estrategias de retención.

---

## 🛠️ Contenido del proyecto
- **TelecomX_LATAM_Miel.ipynb** → Notebook con la limpieza de datos, análisis exploratorio y visualizaciones.
- **README.md** → Documento explicativo del proyecto.

---

## 🎯 Objetivo
Comprender qué características de los clientes y servicios contratados están más relacionadas con la **alta tasa de cancelaciones**, para orientar acciones estratégicas que fortalezcan la fidelización.

---

## 🧹 Limpieza y Tratamiento de Datos
- Eliminación de registros con valores nulos o inconsistentes.  
- Conversión de variables categóricas (“Sí/No”) a binarias (1 y 0).  
- Renombración de columnas para mayor claridad.  
- Cálculo de proporciones garantizando que, por cada variable, los porcentajes de **Churn=Yes** y **Churn=No** sumen 100%.  

---

## 🔎 Análisis Exploratorio

### Variables categóricas
- **Contratos mensuales**: 42.7% de evasión, mucho más alta que en contratos anuales (11.3%) y bianuales (2.8%).  
- **Método de pago**: clientes con **cheque electrónico** presentan la mayor tasa de evasión (45.3%), mientras que pagos automáticos con banco o tarjeta retienen mejor (83–85%).  
- **Género**: no se observaron diferencias relevantes (~26% de evasión en ambos casos).

### Variables numéricas y binarias
Al analizar los clientes con valor = 1 en cada variable, las **5 con mayor porcentaje de Churn=Yes** fueron:  
1. `meses_contrato` → **61.99%**  
2. `factura_online` → **33.57%**  
3. `tv` → **30.07%**  
4. `pelis` → **29.94%**  
5. `multi_lines` → **28.61%**

Otros hallazgos:  
- **Mayores de 65 años** muestran menor tasa de evasión (25.5%).  
- **Clientes con pareja** tienden a permanecer más (52.8% No Churn).  
- La mayoría de las evasiones se concentran en clientes que han pagado menos de $1000 y con menos de 6 meses de contrato.

---

## 💡 Conclusiones e Insights
- Los **contratos cortos** y los **pagos manuales** (cheque electrónico) son factores de riesgo clave.  
- La **edad** influye: los adultos mayores muestran menor propensión a cancelar.  
- La evasión es más probable en las **primeras etapas del contrato** (0–6 meses).  
- Existe una relación fuerte entre **compromiso financiero y retención**: a mayor inversión acumulada, menor evasión.  
- La **factura electrónica** resalta como una variable de alto riesgo de churn.  

---

## 📌 Recomendaciones
- **Contratos**: incentivar el cambio hacia planes anuales o bianuales mediante descuentos o beneficios exclusivos.  
- **Pagos**: fomentar el uso de pagos automáticos con promociones o bonificaciones.  
- **Atención al cliente**: reforzar la experiencia durante los **primeros 6 meses**, identificando como grupo de riesgo a los clientes jóvenes, con contrato mensual y bajo gasto acumulado.  
- **Segmentación**: diseñar planes de fidelización específicos para adultos mayores (alto nivel de retención) y clientes con factura electrónica (alto nivel de evasión).  

---

## 📈 Tecnologías utilizadas
- Python (pandas, matplotlib, seaborn)  
- Jupyter Notebook  
