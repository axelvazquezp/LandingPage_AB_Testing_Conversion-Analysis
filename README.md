# Landing Page A/B Testing and Conversion Analysis – Sprint 9

Este repositorio contiene el análisis realizado durante el Sprint 9 para evaluar un experimento A/B implementado en la página de inicio (landing page) de la compañía. El proyecto trabaja con un dataset de 40,000 registros de usuarios expuestos a dos versiones de diseño (Versión A y Versión B), los cuales se limpian, procesan y evalúan estadísticamente para tomar una decisión de negocio basada en datos que optimice la conversión y el valor económico.

## Contenido del repositorio

* `Proyect_Sprint09_Landing_Experiment.ipynb`: Notebook principal que incluye la carga de datos, la conversión de tipos cronológicos (`date` a datetime), el análisis exploratorio y validación de categorías, la evaluación del gasto promedio mediante pruebas t de dos muestras y la comparación de tasas de conversión con pruebas z de proporciones, complementado con pruebas Chi-cuadrado para canales y tipos de usuario.

## Cómo abrir el notebook en Google Colab

Haz clic en el siguiente botón:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1MPpXypC3rVnMb8CK_PE1hdPU8gR0v45a#scrollTo=28940c28)

O también puedes usar este enlace directo: [Abrir en Google Colab](https://colab.research.google.com/drive/1MPpXypC3rVnMb8CK_PE1hdPU8gR0v45a#scrollTo=28940c28)

## Objetivo del análisis

* **Comparar el gasto promedio por usuario:** Aplicar la prueba estadística T de Student (ajustada por varianzas desiguales mediante la prueba de Levene) para determinar si los montos facturados por los clientes que convirtieron difieren de forma significativa entre la variante A y la variante B.
* **Evaluar la tasa de conversión global:** Realizar una prueba Z de dos proporciones independientes para validar si una de las dos versiones de la landing page incrementa de manera estadísticamente significativa la cantidad absoluta de usuarios convertidos.
* **Análisis de la influencia del canal de adquisición:** Utilizar la prueba de Chi-cuadrado de independencia para examinar si la fuente de tráfico por la que ingresan los usuarios (`traffic_source`) afecta o está asociada de manera directa con su probabilidad de conversión.
* **Determinar el impacto según el tipo de usuario:** Correr una prueba de Chi-cuadrado para identificar si el comportamiento histórico del cliente (`user_type`: Nuevo o Recurrente) representa un factor determinante en la tasa de éxito de la página de destino.
