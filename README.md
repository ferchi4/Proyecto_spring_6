# Análisis de Videojuegos: Identificando Patrones de Éxito en el Mercado Global

Este proyecto analiza datos históricos de ventas de videojuegos para identificar patrones que determinan el éxito comercial, con el objetivo de orientar campañas publicitarias y estrategias de desarrollo.

## Objetivo

Identificar patrones que determinen el éxito de un videojuego mediante el análisis de ventas, plataformas populares, géneros rentables y diferencias regionales en preferencias de consumo.

## 🛠️ Tecnologías Utilizadas

*   **Python:** Lenguaje principal.
*   **Pandas, NumPy:** Manipulación y análisis de datos.
*   **Matplotlib, Seaborn:** Visualización de datos.
*   **SciPy:** Pruebas de hipótesis estadísticas (prueba t de Student).
*   **Jupyter Notebook:** Entorno de desarrollo interactivo.

## Dataset

El conjunto de datos (`games.csv`) contiene información de más de 16,000 videojuegos lanzados hasta 2016, incluyendo nombre, plataforma, año de lanzamiento, género, ventas por región, puntuaciones de críticos y usuarios, y clasificación ESRB.

## Pasos Clave del Análisis

1.  **Preparación de los Datos:** Limpieza de valores ausentes, estandarización de formatos, creación de columna `total_sales` (suma de ventas regionales).

2.  **Análisis Exploratorio:** Visualización de lanzamientos por año, identificación de plataformas con mayores ventas totales (PS2, X360, PS3, Wii) y análisis de ciclos de vida de plataformas (6-10 años).

3.  **Análisis del Mercado Actual (2012-2016):**
    *   **Plataformas líderes:** PS4, PS3 y X360 dominan; Sony lidera el mercado, Nintendo tiene menor presencia.
    *   **Distribución de ventas:** Boxplots muestran alta dispersión y valores atípicos (juegos muy exitosos) en todas las plataformas.
    *   **Impacto de reseñas:** Correlación baja a moderada entre puntuaciones y ventas; las reseñas no son el único factor determinante.
    *   **Rentabilidad por género:** Acción es el género más común, pero shooters y deportes son los más rentables por título.

4.  **Perfil del Usuario por Región:**
    *   **NA y EU:** Dominan consolas de sobremesa (Xbox, PlayStation) y géneros de acción y deportes.
    *   **Japón:** Preferencia por consolas portátiles (3DS, PSV) y juegos de rol.

5.  **Pruebas de Hipótesis Estadísticas:**
    *   **Hipótesis 1 (Xbox One vs. PC):** No hay diferencia significativa en calificaciones promedio de usuarios (p-value = 0.549).
    *   **Hipótesis 2 (Acción vs. Deportes):** Existe diferencia significativa en calificaciones promedio (p-value < 0.05).

## Resultados y Conclusiones

*   **Mercado dinámico:** Plataformas tienen ciclos de vida predecibles (6-10 años). Es crucial actualizarse con tendencias.
*   **Dominio regional:** Sony lidera en NA y EU con consolas de sobremesa; Nintendo tiene mayor presencia en portátiles, especialmente en Japón.
*   **Rentabilidad por género:** Shooters y deportes generan mayores ingresos por título, aunque acción es más común.
*   **Factores de éxito:** Reseñas no son los únicos predictores; plataforma, género, región y marketing juegan un papel fundamental.
*   **Estrategia recomendada:** Enfocar en plataformas líderes (PS4, XOne) y géneros de alto rendimiento (shooters, deportes) en mercados occidentales; considerar portátiles y juegos de rol en Japón.

##  Cómo Ejecutar el Proyecto

1.  Clona el repositorio : (https://github.com/ferchi4/Proyecto_spring_6)
2.  Instala las dependencias: `pip install pandas numpy matplotlib seaborn scipy jupyter`
3.  Ejecuta el archivo `proyecto6.ipynb` en Jupyter Notebook.
