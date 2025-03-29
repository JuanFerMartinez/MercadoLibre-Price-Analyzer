# 🛒 MercadoLibre Price Analyzer

**MercadoLibre Price Analyzer** es una aplicación interactiva desarrollada en **Python + Streamlit** que permite:

- Realizar scraping diario de precios de productos en MercadoLibre  
- Detectar precios atípicos (outliers)  
- Analizar la evolución histórica de precios por producto  
- Visualizar todo de forma clara e intuitiva  

---

## 📦 Tecnologías utilizadas

- Python 3.10+  
- Selenium  
- Pandas  
- Matplotlib  
- Streamlit  

---

## 🚀 Funcionalidades principales

✅ Scraping automático y manual de múltiples categorías  
✅ Análisis estadístico y visualización de precios  
✅ Detección de outliers (muy caros o muy baratos)  
✅ Evolución de precios en el tiempo  
✅ Tablas y gráficas interactivas  
✅ Exportación de resultados en CSV desde la app  

---

## 📁 Estructura del proyecto

```
Scraper-MercadoLibre/
│
├── data/                      ← Archivos generados automáticamente (productos, outliers, evolución)
│
├── src/
│   ├── main_app.py            ← ✅ App principal Streamlit
│   ├── scraper.py             ← Scraping de una sola categoría
│   ├── multi_scraper.py       ← Scraping de múltiples categorías
│   ├── scheduler.py           ← Ejecución automática diaria
│   ├── outliers.py            ← Detección de precios atípicos
│   ├── outliers_dashboard.py  ← Versión previa interactiva solo para outliers
│   ├── graficar_outliers.py   ← Visualización estática
│   ├── evolucion_multiples.py ← Construcción de CSVs de evolución
│   └── analisis.py            ← Gráficas de distribución y rankings
```

---

## ⚙️ Requisitos

Instala las dependencias necesarias:

```bash
pip install -r requirements.txt
```

O bien, manualmente:

```bash
pip install selenium pandas matplotlib streamlit schedule
```

> 💡 Asegúrate de tener `chromedriver.exe` en `src/` y compatible con tu versión de Google Chrome.

---

## ▶️ ¿Cómo ejecutar la app?

Desde la raíz del proyecto, ejecuta:

```bash
streamlit run src/main_app.py
```

---

## 📅 Automatización

El archivo `scheduler.py` ejecuta el scraping diariamente a una hora definida (por defecto 09:00 a.m.)

```bash
python src/scheduler.py
```

---

## 📤 Créditos

Proyecto desarrollado por **Juan Fernando Martínez Ruiz**  
📅 Año: 2025  
🔗 [LinkedIn](https://www.linkedin.com/in/juanfermartinez/)

---
