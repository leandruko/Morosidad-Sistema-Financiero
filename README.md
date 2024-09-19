# Proyecto de Machine Learning y Análisis de Datos - Morosidad en el Sistema Financiero

## Descripción

Este proyecto tiene como objetivo realizar un análisis de datos y aplicar modelos de machine learning para predecir si un usuario será deudor en el sistema financiero en función de los datos históricos y tendencias. A través del análisis exploratorio de datos y la implementación de algoritmos de clasificación, buscamos encontrar patrones que nos permitan hacer predicciones precisas sobre la morosidad de los clientes.

## Dataset

- **Fuente del Dataset:** [Kaggle](https://www.kaggle.com/datasets/luishcaldernb/morosidad)
- **Descripción del Dataset:** 
    El dataset contiene información detallada sobre los usuarios y su historial financiero, incluyendo variables como:
    - **Edad:** Edad del usuario.
    - **Ingreso:** Ingreso mensual del usuario.
    - **Nivel Educativo:** Nivel de educación alcanzado por el usuario.
    - **Zona:** Lugar de residencia del usuario.
    - **Línea de Crédito Disponible:** Cantidad de crédito disponible.
    - **Deuda en el Sistema Financiero:** Total de la deuda que tiene el usuario en el sistema financiero.
    - **Score de Crédito:** Calificación de crédito del usuario.

## Estructura del Proyecto

1. **Introducción:**
   - Los bancos, como intermediarios financieros, prestan dinero a quienes cumplen con los requisitos establecidos. Sin embargo, cuando llega el momento, una parte de los prestatarios incumplen con sus obligaciones y se atrasan en los pagos. Para el mes de julio del presente año, la morosidad en el sistema financiero peruano se ubicó en 4.04%, en las Mypes fue de 8.07% y en las Cajas Rurales fue de 11.25% (RPP Noticias, 05 de julio de 2021). Según Jorge C. (Diario La República, 09 de febrero de 2020), profesor de la Pacífico Business School, comenta que una de las posibles causas es que la gente aglomera gastos […] pequeños e inconscientes a través de las líneas de crédito asignadas a sus trajetas (tasa promedio anual de 46%, y en retiro de efectivo es de 120% anual). La forma en que los bancos evalúan la posibilidad o no de un crédito es a través del Score de calificación crediticia del cliente. Un score mayor significa un perfil crediticio mejor. Otra forma de evaluación es por medio del nivel de ahorro, y este va de cero a doce, significando este último un 'alto nivel de ahorros'. El atraso histórico (en número de días) también juega un rol importante, así como la calificación absoluta del cliente como 'pagador al día' u 'cliente moroso'. De otro lado, la SBS también clasifica el riesgo de cada crédito: 'cero' es normal, y el nivel 'cuatro' es pérdida. Sin embargo ¿Cómo afectaría la morosidad al banco? "Un incremento en la morosidad aumenta el nivel de riesgo, por tanto crecen las provisiones solicitadas por el regulador (dinero inmovilizado, y que no puede ser prestado). Esta es una forma de afectación, como a la rentabilidad de la entidad financiera, por ejemplo" (Conexión Esan, 13 de diciembre de 2016). Viendo desde el punto de vista del banco, la pregunta sería ¿Qué insights podemos hallar en los datos históricos que nos permitan tomar mejores decisiones antes de efectuar los préstamos? Es así que este trabajo pretende hallar dichos insights, considerados aún invisibles, y relacionados a la morosidad bancaria peruana a través de la formulación de preguntas sencillas. La revisión, limpieza, transformación y modelación de datos servirán de apoyo en la búsqueda de conclusiones, y la guía en la toma de decisiones.
   
2. **Carga y Exploración de los Datos:**
   - Carga de las librerías y el dataset.
   - Análisis exploratorio inicial para entender la estructura de los datos.

3. **Preprocesamiento de Datos:**
   - Limpieza de los datos: eliminación de valores nulos y tratamiento de datos faltantes.
   - Codificación de variables categóricas y escalado de características numéricas.
   
4. **Análisis Univariado:**
   - Exploración individual de las variables del dataset, como la distribución de la edad, ingresos y nivel educativo.
   
5. **Análisis Bivariado:**
   - Análisis de las relaciones entre variables, como la relación entre el nivel educativo y la morosidad o entre la zona de residencia y el ingreso.
   
6. **Aplicación de Modelos de Machine Learning:**
   - Se han utilizado varios modelos de clasificación para predecir si un usuario será deudor o no. Los modelos incluyen:
     - **Regresión Logística**
     - **Árbol de Decisión**
     - **Máquina de Soporte Vectorial (SVM)**
   
7. **Evaluación del Modelo:**
   - Se evalúa el rendimiento de cada modelo mediante las métricas de precisión, recall, F1-score y la matriz de confusión.
   
8. **Conclusiones:**
   - Observaciones clave sobre los resultados obtenidos y las recomendaciones para futuras mejoras.

## Resultados

- **Regresión Logística:** 
   - Precisión del modelo: 0.71
   - Mejor para la clase de deudores, pero menos preciso para la clase no deudora.
   
- **Árbol de Decisión:** 
   - Precisión del modelo: 0.82
   - Buen balance entre precisión y recall para ambas clases.
   
- **SVM:** 
   - Precisión del modelo: 0.70
   - Similar a la Regresión Logística, con mejor desempeño en la clase de deudores.

## Requisitos

Para ejecutar este proyecto, es necesario tener instalados los siguientes paquetes:

- Python 3.x
- Librerías:
  - pandas
  - numpy
  - scikit-learn
  - matplotlib
  - seaborn

Instala todas las dependencias con el siguiente comando:

```bash
pip install -r requirements.txt
