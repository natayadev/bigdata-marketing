<img width="10%" alt="Cody" src="https://codigofacilito.com/assets/codys/programando-circle-83a5c0c48b92a40090f4d46f1b28b026630dd9ee8e51769cf223e53ca3eb32cb.png" />

# Big Data Marketing
Proyecto Final para el Bootcamp de Data Engineering de Codigo Facilito 🐊

<i>Automatización de Reportes de Análisis de Métricas de Redes Sociales para Big Data Marketing.</i>

## Fundamentación

En el mundo del marketing digital el análisis de métricas de redes sociales es fundamental para comprender el rendimiento de las estrategias de marketing y tomar decisiones informadas. Sin embargo, el proceso de recopilación, limpieza, transformación y presentación de estos datos puede resultar tedioso y propenso a errores cuando se realiza de forma manual, por lo tanto, surge la necesidad de automatizar este proceso para mejorar la eficiencia y la precisión del análisis.

## **Objetivos**

- Automatizar el proceso de recopilación, limpieza, transformación y presentación de datos de redes sociales para análisis de métricas.
- Implementar una arquitectura eficiente y escalable que permita gestionar grandes volúmenes de datos de diferentes fuentes.
- Generar reportes mensuales detallados de análisis de métricas de redes sociales para clientes de Big Data Marketing.
- Facilitar el acceso a insights valiosos sobre el rendimiento de las estrategias de marketing en redes sociales para la toma de decisiones informadas.

## **Arquitectura**

Se emplea una arquitectura basada en un proceso de extracción, transformación y carga (ETL) para la automatización del flujo de datos:

1. **Proceso de Extracción**
    - Los datos se extraen de archivos CSV y Excel que contienen las métricas de las redes sociales de diferentes plataformas: en este caso utilizaremos las métricas mensuales generadas por Instagram, LinkedIn y Twitter de distintos clientes organizamos por ficheros.
    - La extracción se realiza mediante scripts Python que consumen los archivos de su carpeta específica.
    - Se planifica una extracción manual y mensual de los datos para cada cliente.
2. **Proceso de Transformación**
    - Durante la transformación, se aplican reglas de limpieza, normalización y enriquecimiento de datos.
    - Scripts en Python se utilizan para realizar las transformaciones necesarias antes de cargar los datos en el data warehouse.
3. **Proceso de Carga**
    - Los datos transformados se cargan en un data warehouse, donde se estructuran y almacenan de manera centralizada.
    - La carga de datos en el data warehouse se realiza de manera programada y automática cada primer día del mes correspondiente.

**Mantenimiento:** Es crucial evaluar mensualmente los cambios en la estructura de los archivos fuente de las diferentes redes sociales. Las plataformas de redes sociales pueden cambiar el orden, agregar o eliminar algunas métricas, lo que puede afectar la ejecución del script.

Se debe prestar atención a los avisos y actualizaciones de las plataformas de redes sociales para garantizar la compatibilidad continua y la precisión de los datos.

**Control de Versiones:** Se utiliza GitHub para el control de versiones de código y documentación, facilitando la colaboración y el seguimiento de cambios.

**Gestión de Proyectos:** Procedimientos ágiles de gestión de proyectos se implementan para garantizar la entrega oportuna y efectiva del proyecto, con ayuda de herramientas como Notion y GitHub (Wiki, Issues, y Projects.
