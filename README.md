# 📊 Proyecto M0 – Descubriendo el Éxito Comercial

Este proyecto forma parte del Bootcamp de **Data Analytics en SoyHenry**.  
El objetivo fue analizar los datos históricos de ventas de **45 tiendas de retail** para identificar patrones, tendencias y oportunidades de mejora en la gestión comercial.

---

## 📂 Datasets utilizados
- **stores.csv** → Información de cada tienda (Store, Type, Size).  
- **sales.csv** → Registros históricos de ventas semanales por tienda y departamento.  
- **features.csv** → Variables externas: clima, precio de combustible, markdowns, CPI, desempleo y feriados.  

---

## 🛠️ Procesos aplicados

### 1. Limpieza y normalización
- Conversión de la columna **Type** a valores numéricos (A=1, B=2, C=3).  
- Normalización de **Size** creando la columna `Size_Normalized` con valores entre 0 y 1 → comparación justa entre tiendas grandes, medianas y pequeñas.  
- Filtros activados en encabezados para exploración rápida y detección de inconsistencias.  
- Reducción de decimales en **Temperature** y **Fuel_Price** para mayor claridad visual.  
- Formato numérico uniforme en `Size` para mejorar legibilidad y comparaciones.  

### 2. Creación de la base según el DER
Se verificó integridad de llaves primarias y foráneas:  
- **Stores:** Store, Type_Num, Size_Normalized, Location.  
- **Features:** Store, Date, Temperature, Fuel_Price, CPI, Unemployment, IsHoliday.  
- **Sales:** ID_Sales, Store, ID_Dept, Date, Weekly_Sales.  

✔️ No existen registros huérfanos en *Sales*.  

---

## 📈 Insights principales

1. **Ventas Totales y Promedio Semanal**  
   - Ventas totales: **$4,448,332,867**  
   - Semanas únicas: 95  
   - Promedio semanal: **$46,824,556**  

2. **Impacto de semanas festivas**  
   - Promedio en feriados: $17,055  
   - Promedio en no feriados: $15,754  
   - Incremento: **+8 %** durante semanas festivas.  

3. **Departamentos líderes**  
   - Dept 1 → $844M (19 %)  
   - Dept 3 → $717M (16 %)  
   - Dept 7 → $630M (14 %)  
   📌 Los 5 primeros departamentos concentran **+75 % de las ventas**.  

4. **Tiendas con mayor aporte**  
   - Store 36 → $230M (5.2 %)  
   - Store 40 → $225M (5.1 %)  
   - Store 14 → $223M (5.0 %)  
   📌 Las 5 principales tiendas suman **casi 25 % del total**.  

5. **Tendencia mensual**  
   - Mes más fuerte: **Diciembre** (hasta $288M en 2011).  
   - Confirma la relevancia de campañas navideñas.  

6. **Crecimiento Semana a Semana (WoW)**  
   - Dept 7: +7.5 %  
   - Dept 3: +6.9 %  
   📌 Categorías con mayor crecimiento relativo.  

---

## 🔑 KPIs calculados
- **Ventas Totales** → $4,448,332,867  
- **Promedio Semanal** → $46,824,556  
- **Boost Factor (Feriados)** → +8 %  
- **Top Departamentos** → Depts 1, 3, 7, 5 y 8  
- **Top Tiendas** → Stores 36, 40, 14, 2 y 20  

---

## 📌 Conclusiones
- **Depto 1** concentra el 19 % de las ventas → mantener inventario sólido y promociones constantes.  
- **Tienda 36** lidera con 5.2 % → oportunidad de replicar su estrategia en otras sucursales.  
- **Diciembre** es el mes clave → reforzar campañas navideñas y promociones estacionales.  
- **Feriados** generan un alza promedio del 8 % → planificar estrategias de marketing alineadas a estos días.  
- **Depts 7 y 3** muestran mayor crecimiento WoW → monitoreo constante para aprovechar su impulso.  

---

## 🚀 Tecnologías y herramientas
- **Excel / Google Sheets** (limpieza, normalización, KPIs).  
- **Modelado relacional** (DER, integridad de datos).  
- **Tablas dinámicas y fórmulas avanzadas** (SUMAR.SI, PROMEDIO.SI, CONTAR.UNICOS).  

---

✍️ *Este proyecto representa el primer paso en el análisis de datos aplicado al negocio, combinando limpieza, modelado y visualización para generar insights comerciales accionables.*
