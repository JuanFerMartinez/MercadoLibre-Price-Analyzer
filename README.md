
# 🛒 MercadoLibre Price Analyzer

**MercadoLibre Price Analyzer** es una aplicación interactiva desarrollada en **Python + Flask + HTML/CSS** que permite:

- Realizar scraping diario de precios de productos en MercadoLibre  
- Detectar precios atípicos (outliers)  
- Analizar la evolución histórica de precios por producto  
- Visualizar todo de forma clara e intuitiva desde una interfaz web personalizada  

---

## 📦 Tecnologías utilizadas

### Backend
- Python 3.10+  
- Flask  
- Selenium  
- Pandas  
- Matplotlib  

### Frontend
- HTML  
- CSS   

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
MercadoLibre-Price-Analyzer/
│
├── backend/
│   ├── src/
│   │   ├── main_app.py            ← App en Streamlit (versión inicial)
│   │   ├── api.py                 ← ✅ API con Flask para exponer los datos
│   │   ├── scraper.py             ← Scraping de una sola categoría
│   │   ├── multi_scraper.py       ← Scraping de múltiples categorías
│   │   ├── scheduler.py           ← Ejecución automática diaria
│   │   ├── outliers.py            ← Detección de precios atípicos
│   │   ├── outliers_dashboard.py  ← Versión interactiva solo para outliers
│   │   ├── graficar_outliers.py   ← Visualización estática
│   │   ├── evolucion_multiples.py ← Construcción de CSVs de evolución
│   │   └── analisis.py            ← Gráficas de distribución y rankings
│   ├── data/                      ← Archivos generados automáticamente (.csv)
│   └── requirements.txt
│
├── frontend/
│   └── (Interfaz desarrollada en HTML + CSS por el frontend developer)
```

---

## ⚙️ Requisitos

Instala las dependencias necesarias para el backend:

```bash
pip install -r requirements.txt
```

> 💡 Asegúrate de tener `chromedriver.exe` dentro de `src/` y que sea compatible con tu versión de Google Chrome.

---

## ▶️ ¿Cómo ejecutar el backend (API)?

Desde la carpeta `backend/src`, corre:

```bash
python api.py
```

Esto iniciará la API en: `http://localhost:5000`  
Ejemplos de endpoints disponibles:

- `/api/ps5`
- `/api/laptop`
- `/api/silla gamer`
- `/api/categorias`

---

## 💻 ¿Quién desarrolla el frontend?

El frontend del proyecto está siendo desarrollado por **Duvan Mancilla**  
🔗 [LinkedIn de Duvan](https://www.linkedin.com/in/duvan-mancilla/)  
Tecnologías: **HTML, CSS**

---

## 📷 Screenshots

| Interfaz | Scraping | Análisis |
|----------|----------|----------|
| ![screenshot](screenshots/screenshot.png) | ![screenshot1](screenshots/screenshot1.png) | ![screenshot2](screenshots/screenshot2.png) |

---

## 📅 Automatización

El archivo `scheduler.py` ejecuta el scraping automáticamente cada día a las 09:00 a.m.

```bash
python src/scheduler.py
```

---

## 📤 Créditos

**Backend** desarrollado por **Juan Fernando Martínez Ruiz**  
📅 Año: 2025  
🔗 [LinkedIn de Juanfer](https://www.linkedin.com/in/juanfermartinez/)

---

## 📄 Licencia

MIT License
