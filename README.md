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
├── data/ ← Archivos generados automáticamente (productos, outliers, evolución)
│
├── src/
│ ├── main_app.py ← ✅ App principal Streamlit
│ ├── scraper.py ← Scraping de una sola categoría
│ ├── multi_scraper.py ← Scraping de múltiples categorías
│ ├── scheduler.py ← Ejecución automática diaria
│ ├── outliers.py ← Detección de precios atípicos
│ ├── outliers_dashboard.py ← Versión previa interactiva solo para outliers
│ ├── graficar_outliers.py ← Visualización estática
│ ├── evolucion_multiples.py ← Construcción de CSVs de evolución
│ └── analisis.py ← Gráficas de distribución y rankings
```

