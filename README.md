# data-analysis-restaurant

# Proyecto: Análisis de Datos de Restaurante
Bienvenido al repositorio del proyecto de análisis de datos de un restaurant! 
Este proyecto tiene como objetivo explorar y extraer insights valiosos a partir de un conjunto de datos transaccionales y operativos de un restaurant. A través del análisis con SQL, busco identificar patrones de venta, optimizar la gestión de inventario y comprender el comportamiento del cliente. Todo con el objetivo de ofrecer recomendaciones basadas en datos para mejorar la eficiencia y la rentabilidad del negocio.

## Contexto y Motivación
En el competitivo mundo de la gastronomía, la toma de decisiones basada en datos es crucial. Este proyecto personal surge de la curiosidad por entender cómo la información contenida en las transacciones diarias de un restaurante puede transformarse en conocimiento accionable. Desde la popularidad de los platos hasta los horarios/fechas de mayor afluencia, pasando por la gestión de costos, cada dato es una oportunidad para optimizar las operaciones y mejorar la experiencia del cliente.

## Objetivos del Proyecto
- Entender el rendimiento de ventas: Identificar los platos más y menos vendidos, las horas pico y los días de mayor actividad.
- Optimizar el inventario: Analizar el consumo de ingredientes para evitar escasez o desperdicio.
- Analizar el comportamiento del cliente: Determinar la frecuencia de visitas, el gasto promedio y las preferencias de menú.
- Evaluar la rentabilidad: Calcular márgenes de ganancia por plato o categoría.
- Proponer recomendaciones: Ofrecer insights que ayuden al restaurante a tomar decisiones informadas sobre el menú, promociones y personal.

## Herramientas Utilizadas
- SQL (PostgreSQL v13)
- [Opcional: Herramienta de visualización] (por ejemplo, Tableau, Power BI, Google Data Studio, Matplotlib/Seaborn si usas Python)
- [Opcional: Lenguaje de scripting para ETL] (por ejemplo, Python para procesamiento de datos o carga)

## Estructura del Proyecto
Este repositorio está organizado en las siguientes carpetas lógicas para facilitar la navegación y comprensión del proyecto:

1. data/
Esta carpeta contiene los conjuntos de datos en bruto utilizados para el análisis. Aquí encontrarás los archivos CSV, Excel u otros formatos que sirvieron como fuente de información para la base de datos del restaurante.
Ejemplo: transacciones.csv, menu_items.xlsx, empleados.json

2. schema/
Aquí se encuentran los scripts SQL para la creación de la base de datos y sus tablas. Incluye las definiciones de las tablas (CREATE TABLE), las claves primarias y foráneas, y cualquier otra restricción de integridad de datos. También podrías encontrar un diagrama Entidad-Relación (DER) de la base de datos para una visualización clara del esquema.
Ejemplo: create_tables.sql, der_restaurante.png

3. etl_scripts/
Esta carpeta alberga los scripts SQL para la carga y transformación de datos (ETL). Aquí se definen las sentencias INSERT para poblar las tablas con los datos de la carpeta data/. Si se realizaron transformaciones complejas antes de la carga, los scripts correspondientes (SQL o Python) también irán aquí.
Ejemplo: load_data.sql, clean_and_transform_data.py

4. queries/
Contiene todas las consultas SQL desarrolladas para el análisis de datos. Estas consultas están organizadas lógicamente según los objetivos del proyecto y están bien comentadas para explicar su propósito y la lógica subyacente.
Ejemplo: ventas_por_plato.sql, consumo_ingredientes_mensual.sql, clientes_frecuentes.sql

5. analysis/
En esta carpeta se encuentra el informe o documento de análisis que resume los hallazgos clave, los insights obtenidos de las consultas SQL y las recomendaciones para el negocio. Puede ser un archivo Markdown, un Jupyter Notebook (si usaste Python para análisis o visualización), o un PDF/HTML generado. También se incluirán visualizaciones o dashboards relevantes aquí.
Ejemplo: informe_analisis_restaurante.md, dashboard_ventas.png, analisis_clientes.ipynb


## Cómo Replicar el Proyecto
Para configurar y ejecutar este proyecto en tu entorno local, sigue estos pasos:

### Clona el repositorio:
``` Bash
git clone https://github.com/luislarrainpelen/data-analysis-restaurant.git
cd data-analysis-restaurant
```

### Configura tu base de datos SQL:
Asegúrate de tener instalada y funcionando la versión de SQL que prefieras en local o también puedes utilizar una herramienta online como por ejemplo www.db-fiddle.com

### Workflow
Ejecuta los scripts en la carpeta schema/ para crear la base de datos y las tablas.
Ejecuta los scripts en la carpeta etl_scripts/ para cargar los datos.
Explora las consultas:
Navega a la carpeta queries/ y ejecuta las consultas para replicar los análisis.
Revisa el análisis:
Consulta el documento en la carpeta analysis/ para entender los resultados y las conclusiones.

## Próximos Pasos y Posibles Mejoras
Integrar datos de reseñas de clientes para un análisis de sentimiento.
Implementar modelos predictivos para la demanda de platos.
Desarrollar un dashboard interactivo en tiempo real para la gerencia del restaurante.
Automatizar el proceso de ETL.
