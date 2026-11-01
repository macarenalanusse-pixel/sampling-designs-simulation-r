# Comparación de diseños muestrales mediante simulación en R

**Asignatura:** Muestreo y Planificación de Encuestas I  
**Carrera:** Licenciatura en Estadística  
**Institución:** Universidad de la República (Udelar), Uruguay  
**Autoras:** Valentina Rodríguez Blanco, Macarena Perdomo y Sol Astengo.

## Descripción

Este proyecto compara el comportamiento de distintos diseños probabilísticos de muestreo para estimar el total de automóviles y camionetas de los hogares de Rivera, Uruguay. El análisis se realizó en **R**, utilizando simulaciones para estudiar el sesgo empírico, la varianza, el error cuadrático medio, la precisión y los intervalos de confianza de los estimadores.

La unidad de análisis es el **hogar** y la variable de interés es `HOGCE13` (cantidad de automóviles o camionetas del hogar). El informe académico presenta un total poblacional de **14.097 vehículos**.

## Metodología

Se compararon cuatro diseños:

- Muestreo simple sin reemplazo (SI).
- Muestreo simple con reemplazo (SIR).
- Muestreo estratificado, utilizando la cantidad de habitaciones del hogar para definir estratos.
- Muestreo por conglomerados, con conglomerados definidos mediante la combinación de sección y segmento censal.

Se realizaron **1.000 simulaciones por diseño**, con un tamaño muestral aproximado de **1.500 hogares**. También se estudió un estimador alternativo para el muestreo por conglomerados.

## Principales resultados

- El **diseño estratificado** presentó la menor varianza empírica entre los cuatro diseños iniciales comparados.
- El diseño por conglomerados mostró una dispersión considerablemente mayor.
- El estimador alternativo para conglomerados redujo la variabilidad respecto al estimador inicial, según los resultados del informe.

Para los valores numéricos, gráficos, supuestos y conclusiones completos, consultar el informe original.

## Herramientas

- **R** para procesamiento, selección de muestras y simulaciones.
- Paquetes: `ggplot2`, `sampling`, `survey`, `haven`, `tidyverse` y `patchwork`.
- **Quarto** para elaborar el informe reproducible.

## Archivos del proyecto

- `Proyecto.pdf`: informe académico original.
- `Proyecto(2).qmd`: archivo Quarto original del informe.
- `ScriptProyecto.R`: script principal ejecutado desde Quarto.

> **Datos:** El script original carga `Rivera.RData`. El conjunto de datos no se incluye inicialmente en este repositorio hasta verificar las condiciones de uso y publicación. Sin ese archivo no es posible reproducir completamente el análisis. Esta limitación no modifica el contenido del trabajo académico original.

## Autoría y contexto

Trabajo académico grupal realizado por **Valentina Rodríguez Blanco, Macarena Perdomo y Sol Astengo** en la asignatura **Muestreo y Planificación de Encuestas I**, perteneciente a la **Licenciatura en Estadística de la Universidad de la República (Udelar), Uruguay**.

El informe y el código se presentan como parte del trabajo académico original, sin modificar sus resultados. Cualquier extensión posterior deberá identificarse por separado.

## Referencia bibliográfica

Gutiérrez Rojas, H. Andrés (2016). *Estrategias de muestreo: diseño de encuestas y estimación de parámetros*. Ediciones de la U.
