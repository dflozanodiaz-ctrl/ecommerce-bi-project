# 📊 E-Commerce Sales Dashboard — Power BI Project

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![SQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)

## 📌 Descripción del Proyecto

Este proyecto de Business Intelligence analiza el rendimiento comercial de una empresa de e-commerce ficticia, con datos de ventas de 2022 a 2024. El objetivo es construir un dashboard interactivo en Power BI que permita tomar decisiones estratégicas basadas en datos.

---

## 🎯 Objetivos del Análisis

- Identificar los productos y categorías más rentables
- Analizar la evolución de ventas mensuales y anuales
- Evaluar el rendimiento por región/país
- Calcular KPIs clave: ticket promedio, margen bruto, tasa de conversión
- Detectar tendencias y estacionalidades

---

## 🗂️ Estructura del Repositorio

```
ecommerce-bi-project/
│
├── data/
│   └── sales_data.csv          # Dataset principal de ventas
│
├── sql/
│   └── queries.sql             # Consultas SQL para exploración y transformación
│
├── powerbi/
│   └── dax_measures.md         # Medidas DAX utilizadas en el dashboard
│
├── notebook/
│   └── exploratory_analysis.ipynb  # Análisis exploratorio en Python/Pandas
│
└── README.md
```

---

## 📐 Modelo de Datos (Esquema Estrella)

```
        dim_productos
             │
dim_tiempo ──┤
             ├── fact_ventas
dim_clientes─┤
             │
        dim_regiones
```

| Tabla | Tipo | Descripción |
|---|---|---|
| `fact_ventas` | Hechos | Transacciones de venta |
| `dim_productos` | Dimensión | Catálogo de productos |
| `dim_clientes` | Dimensión | Datos de clientes |
| `dim_tiempo` | Dimensión | Calendario completo |
| `dim_regiones` | Dimensión | Regiones y países |

---

## 📊 KPIs del Dashboard

| KPI | Descripción |
|---|---|
| **Ventas Totales** | Suma de ingresos en el período |
| **Ticket Promedio** | Ingreso medio por orden |
| **Margen Bruto** | (Ingresos - Costo) / Ingresos |
| **Órdenes Totales** | Cantidad de transacciones |
| **Clientes Únicos** | COUNT DISTINCT de clientes |
| **Crecimiento YoY** | Variación vs. año anterior |

---

## 🛠️ Herramientas Utilizadas

| Herramienta | Uso |
|---|---|
| **MySQL** | Exploración y limpieza de datos |
| **Python + Pandas** | Análisis exploratorio (EDA) |
| **Power BI Desktop** | Dashboard e informes |
| **DAX** | Medidas y KPIs calculados |

---

## 🚀 Cómo reproducir el proyecto

1. Clonar el repositorio:
```bash
git clone https://github.com/tu-usuario/ecommerce-bi-project.git
```

2. Ejecutar las queries SQL en MySQL Workbench o terminal para explorar los datos.

3. Abrir el notebook de Python para el análisis exploratorio:
```bash
jupyter notebook notebook/exploratory_analysis.ipynb
```

4. Abrir el archivo `.pbix` en Power BI Desktop y conectar al dataset CSV.

---

## 📈 Vista Previa del Dashboard

> El dashboard cuenta con 3 páginas:
> - **Resumen Ejecutivo**: KPIs principales y tendencia de ventas
> - **Análisis por Producto**: Ranking y rentabilidad
> - **Análisis Geográfico**: Mapa de ventas por región

---

## 👤 Autor

**[Tu Nombre]**  
Data Analyst | BI Developer  
[LinkedIn](https://linkedin.com) · [Kaggle](https://kaggle.com) · [GitHub](https://github.com)

---

## 📄 Licencia

MIT License — libre para usar y modificar con atribución.
