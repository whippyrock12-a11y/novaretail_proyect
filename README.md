#📊 NovaRetail+: Análisis de Comportamiento y Factores de Ingreso

🛍️ Explorando los impulsores de rentabilidad en el E-commerce Este repositorio contiene el análisis estadístico y exploratorio realizado para NovaRetail+, una plataforma de comercio electrónico líder en Latinoamérica, utilizando datos de comportamiento de usuario registrados hasta el cierre de 2024.

El objetivo principal es identificar qué factores del comportamiento del cliente (frecuencia de visitas, uso de dispositivos, satisfacción) tienen mayor asociación con el ingreso anual generado, permitiendo al equipo de Crecimiento y Retención tomar decisiones basadas en datos.

**📂 Contenido del repositorio**

Project-NovaRetail.ipynb: Notebook principal con el ciclo completo de análisis: carga, limpieza de tipos de datos, análisis descriptivo y cálculo de coeficientes de correlación.

▶️ Cómo ejecutar el análisis Puedes visualizar y ejecutar el notebook directamente en Google Colab: https://colab.research.google.com/drive/1VPXQOuoQtA0i1MwSW7ymvFOcMJ300Itp?usp=sharing

**🧠 Objetivos del análisis**

Limpieza y Tipificación: Corrección de tipos de datos (como la variable edad) y validación de 15,000 registros para asegurar un análisis preciso.

Perfilamiento Demográfico: Análisis de la distribución por regiones y tipos de dispositivo para entender la penetración del mercado.

Análisis Correlacional Multivariable:

Pearson & Spearman: Para relaciones lineales y monótonas entre variables numéricas (Visitas vs. Compras).

Punto Biserial: Para medir el impacto de ser miembro Premium o el Abandono sobre los ingresos.

V de Cramér: Para identificar asociaciones entre variables categóricas (Región vs. Dispositivo).

**📊 Principales Hallazgos (Insights)**

Dominio Mobile: El 65.45% de los usuarios acceden vía móvil, lo que valida la necesidad de una estrategia Mobile-First.

Potencial Premium: Solo el 13.92% de la base es Premium. Dado que el abandono (15.07%) es ligeramente superior, existe una oportunidad crítica para fortalecer la retención en este segmento.

Engagement vs. Conversión: Los clientes visitan el sitio ~10 veces al mes pero solo compran 1.2 veces en promedio. Existe una correlación moderada (Pearson 0.29) que sugiere que aumentar las visitas favorece la compra.

Suscripción e Ingresos: Se detectó una asociación casi nula entre la suscripción y los ingresos totales (Punto-biserial 0.063), indicando que el modelo Premium actual no necesariamente atrae a los clientes de mayor ticket promedio.

**🛠️ Tecnologías utilizadas**

Python

Pandas: Limpieza de datos y manipulación de DataFrames.

Seaborn & Matplotlib: Heatmaps de correlación y visualización de distribuciones.

SciPy: Implementación de pruebas estadísticas de Point-Biserial y Chi-cuadrado (Cramér V).
