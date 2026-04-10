🛒 Amazon Sales – Data Engineering & Dimensional Modeling
Proyecto integral de ingeniería de datos sobre un dataset transaccional de ventas tipo e-commerce, implementado con Spark + SQL.

📌 Descripción
Procesa un dataset de ventas online con más de 1M registros.

Incluye auditoría de calidad, limpieza estructurada y validación financiera.

Implementa un modelo dimensional tipo estrella para análisis escalable.

Genera métricas estratégicas alineadas al negocio.

🏢 Contexto Empresarial
Un entorno de ventas online requiere:

Validar consistencia financiera de ingresos.

Detectar problemas de calidad en datos.

Estandarizar información transaccional.

Construir un modelo analítico escalable.

Generar métricas estratégicas por producto, cliente y tiempo.

🔍 Auditoría de Datos y Validación
Valores nulos → conteo y control por columna.

Campos críticos → validación de Precio, Cantidad e Ingresos.

Duplicados → identificación con claves naturales (OrderID).

Validación financiera → ingresos calculados como Precio * Cantidad vs. campo original.

🧹 Transformaciones
Normalización de tipos de datos.

Creación de columna Profit.

Limpieza de inconsistencias detectadas.

Preparación para modelado dimensional.

🏗️ Modelado Dimensional (Estrella)
Dimensiones:

dim_product

dim_customer

dim_date

Tabla de hechos:

fact_sales

Este diseño permite análisis temporal eficiente, segmentación por cliente/producto y escalabilidad futura.

📈 Métricas Estratégicas
Ingresos totales.

Beneficio total.

Top productos por ventas.

Ventas mensuales.

Ventas por categoría.

⚙️ Flujo de Arquitectura
Código
Raw Dataset → Perfilado → Validación de Calidad → Limpieza → Modelado Dimensional → Métricas Agregadas
⭐ Aspectos Técnicos Destacados
Validación financiera estructural.

Separación correcta de dimensiones y tabla de hechos.

Modelo estrella implementado en Spark.

Consultas SQL optimizadas para análisis de negocio.

Pipeline completo documentado en un único notebook.

✅ Conclusión
Este proyecto demuestra capacidad para:

Auditar calidad de datos.

Implementar transformaciones estructuradas.

Diseñar arquitectura analítica tipo estrella.

Generar métricas alineadas al negocio.

Preparar datasets para consumo analítico o BI.

👤 Autor
Mauricio Vélez Rengifo  
Ingeniero de Datos | Desarrollador Backend

GitHub: Mvelezrengifo

LinkedIn: Mauricio Vélez
