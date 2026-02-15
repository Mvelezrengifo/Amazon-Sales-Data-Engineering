Amazon Sales – Data Engineering & Dimensional Modeling
Executive Summary

Este proyecto implementa un proceso completo de ingeniería de datos sobre un dataset transaccional de ventas tipo e-commerce (Amazon Sales).

Se realizó auditoría de calidad, limpieza estructurada, validación de métricas financieras, modelado dimensional tipo estrella y generación de métricas estratégicas utilizando Spark y SQL.

El notebook documenta el flujo completo desde la exploración inicial hasta la construcción del modelo analítico final.

Business Context

Un entorno de ventas online requiere:

Validar consistencia financiera de ingresos.

Detectar problemas de calidad en datos.

Estandarizar información transaccional.

Construir un modelo analítico escalable.

Generar métricas estratégicas por producto, cliente y tiempo.

El objetivo fue diseñar una solución estructural que permita análisis confiable y extensible.

Data Audit & Quality Validation

Se ejecutó una auditoría técnica inicial del dataset:

Null Validation

Conteo de valores nulos por columna.

Validación de campos críticos: Price, Quantity, Revenue.

Confirmación de integridad en claves naturales.

Duplicate Detection

Identificación de posibles duplicados usando claves naturales (OrderID / combinación relevante).

Validación de unicidad en transacciones.

Financial Formula Validation

Se validó la consistencia de ingresos:

Revenue = Price * Quantity

Creación de columna calculada.

Comparación contra campo Revenue original.

Identificación de posibles desviaciones.

Esta validación demuestra control de integridad financiera.

Data Transformation Layer

Se realizaron transformaciones estructurales:

Normalización de tipos de datos.

Creación de columna Profit.

Limpieza de inconsistencias detectadas.

Preparación para modelado dimensional.

Las transformaciones fueron ejecutadas en Spark dentro del notebook.

Dimensional Modeling

Se implementó un modelo estrella compuesto por:

Dimensions

dim_product

dim_customer

dim_date

Fact Table

fact_sales

Se separaron claves naturales y se construyó estructura analítica optimizada para consultas agregadas.

Este diseño permite:

Análisis temporal eficiente.

Segmentación por cliente y producto.

Escalabilidad futura.

Business Metrics Layer

Se desarrollaron métricas estratégicas:

Revenue total.

Profit total.

Top productos por ventas.

Ventas mensuales.

Ventas por categoría.

Consultas ejecutadas vía SQL dentro del notebook.

Architecture Flow

Raw Dataset
→ Data Profiling
→ Quality Validation
→ Data Cleaning
→ Dimensional Modeling
→ Aggregated Metrics

Technical Highlights

Validación financiera estructural.

Separación correcta de dimensiones y tabla de hechos.

Modelado estrella implementado desde Spark.

Queries optimizadas para análisis de negocio.

Pipeline completo documentado en un único artefacto técnico.

Conclusion

Este proyecto demuestra capacidad para:

Auditar calidad de datos.

Implementar transformaciones estructuradas.

Diseñar arquitectura analítica tipo estrella.

Generar métricas alineadas a negocio.

Preparar datasets para consumo analítico o BI.

El notebook representa un flujo completo de ingeniería de datos aplicado a un entorno de ventas transaccionales.