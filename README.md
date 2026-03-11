# La Campeona Empanadas
### Análisis de ventas y predicción de demanda

Especialización en Ciencia de Datos e Inteligencia Artificial · UTEC – MIT · 2025–2026  
**Autora:** Catalina Vaz Martins

---

## Descripción

Análisis integral de los datos de ventas de **La Campeona Empanadas**, una cadena con dos sucursales en Montevideo (Cordón y Punta Carretas). El dataset cubre el período enero 2024 a febrero 2026 y fue exportado directamente desde el sistema POS del negocio.

El proyecto abarca desde la limpieza y preparación de datos hasta modelos predictivos de demanda, pasando por análisis exploratorio, georreferenciación de pedidos y segmentación de clientes.

## Contenido

El notebook `la_campeona.ipynb` está organizado en las siguientes secciones:

1. **Carga y limpieza de datos** — unificación de 4 archivos fuente, tratamiento de nulos, variables derivadas
2. **Análisis exploratorio** — evolución temporal, ticket promedio, análisis por día, turno, sucursal y canal
3. **Análisis de sabores** — ranking de variedades, distribución por sucursal
4. **Mapa de delivery** — geocodificación de 27.500 pedidos, análisis por barrio
5. **Segmentación de clientes** — KMeans + PCA sobre 847 clientes frecuentes (≥10 pedidos)
6. **Modelos predictivos** — Random Forest para predicción de demanda por sabor, sucursal y día

## Resultados destacados

- **107.000 pedidos** válidos analizados en el período
- Tendencia de crecimiento sostenido con estacionalidad en diciembre–enero
- **Pocitos** es el barrio con mayor volumen de delivery (8.397 pedidos)
- 3 segmentos de clientes identificados, diferenciados principalmente por canal de compra
- Modelo Random Forest: **MAE 9 unidades · R² 0.62**
- Las variables más predictivas fueron los promedios móviles (ma_7, ma_14, ma_30) y el día de la semana

## Stack

```
Python · Pandas · Scikit-learn · LightGBM · Random Forest · Folium · KMeans · PCA · Matplotlib · Seaborn
```

## Fuente de datos

Datos reales exportados desde el sistema POS (SQL Server) del negocio. No se incluyen en el repositorio por contener información comercial sensible.
