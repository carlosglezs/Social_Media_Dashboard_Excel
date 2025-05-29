
# 📊 Proyecto de Análisis de Campañas en Redes Sociales

## 🧾 Descripción

Este proyecto tiene como objetivo analizar el rendimiento de diversas campañas publicitarias realizadas en múltiples redes sociales, utilizando métricas clave como ROI, CTR, CPC, CPA, impresiones, clics y conversiones. Se realizó un tratamiento previo de los datos, una transformación de las variables categóricas y numéricas, y se desarrolló un dashboard interactivo para facilitar la toma de decisiones estratégicas.

---

## 🗂 Estructura del Proyecto

```
/
├── Data_raw/                         # Datos originales
│   ├── Social_Media_Advertising.csv
│
├── Data/                             # Datos procesados y transformaciones
│   ├── redes_sociales_categoricas.xlsx
│   ├── redes_sociales_numericas.xlsx
│   └── redes_sociales_transformacion.xlsx
│
├── Dashboard.xlsx                    # Dashboard interactivo de KPIs y análisis visual
├── Recap.docx                        # Documento con el análisis descriptivo y conclusiones
├── README.md                         # Este archivo
```

---

## 📥 Fuente de Datos

**Fuente**: [Kaggle]  
**Nombre del dataset**: [Social Media Advertising]

---

## 🧹 Proceso de Limpieza y Transformación

- Eliminación de filas duplicadas.
- División de la columna `target_audience` en `gender` y `age`.
- Estandarización de etiquetas (e.g., `ALL AGES` → `unknown`).
- Conversión de campos monetarios y de duración a formato numérico.
- Creación de nuevas métricas derivadas:
  - CTR = (Clicks / Impressions) × 100
  - CPC = Acquisition_Cost / Clicks
  - Conversions = Conversion_rate × Clicks
  - CPA = Acquisition_Cost / Conversions
  - Profit = (ROI × Acquisition_Cost) - Acquisition_Cost

---

## 📈 Análisis Realizado

### Variables Numéricas
- **ROI** muestra gran disparidad, con muchas campañas negativas y algunas muy rentables.
- **Clicks e Impressions** presentan distribución sesgada con outliers.
- **CTR** y **Conversion Rate** tienen comportamientos concentrados pero con efectos notables en el ROI.

### Variables Categóricas
- Mayor ROI en campañas sin segmentación (edad/género = "all"/"unknown").
- Pinterest se identifica como una red con pésimo desempeño.
- “Product Launch” como objetivo de campaña muestra mejor ROI, aunque “Brand awareness” genera mayor beneficio neto.
- El idioma español tiene un ligero ROI superior.

### Variables Temporales
- Mejor mes: Abril.
- Peor mes: Febrero.

---

## 📊 Dashboard

Incluye:
- KPIs: ROI, Impressions, Clicks, Conversions, Profit.
- Gráficos tipo funnel (CTR y CPA).
- Gráfico de líneas con evolución mensual del ROI.
- Segmentadores por edad, segmento de cliente y objetivo de campaña.

---

## 🧠 Conclusiones Relevantes

- 💸 **Pinterest debe ser descartada** como canal de inversión publicitaria.
- 🎯 **No todo depende del ROI:** objetivos como *Brand awareness* aportan valor por volumen.
- 👥 **Campañas no segmentadas** demuestran mayor rendimiento económico, posiblemente por ser más genéricas o eficientes en coste por usuario.

---

## 👤 Autor

**[Tu nombre aquí]**

---

## 📅 Fecha de Actualización

29 de mayo de 2025

---

## 📜 Licencia

Este proyecto está bajo la licencia [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/).  
Esto significa que puedes compartir y adaptar el material, siempre que se cite adecuadamente, no se use para fines comerciales y se mantenga la misma licencia en los derivados.

Fuente original de datos: [Kaggle](https://www.kaggle.com/)
