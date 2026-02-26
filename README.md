# movilidad_urbana_y_productiva_económica_en_LATAM
El objetivo del banco es identificar en qué ciudades invertir en infraestructura de transporte para aumentar la productividad y el bienestar de la población. Se realizó un informe ejecutivo contestando a preguntas del Negocio:¿qué relación existe entre la movilidad urbana (congestión, tiempos de viaje) y la productividad económica (PIB per cápita)? y ¿Qué ciudad : Bogotá, Lima o Buenos Aires o alguna otra en particular, muestra la mayor correlación significativa entre altos niveles de congestión vehicular y bajos indicadores de productividad económica, sugiriendo ser una ciudad prioritaria para inversión en infraestructura de transporte? </p>
 Las variables clave utilizadas fueron los promedio de retraso total (en minutos) provocado por la congestión en todas las vias y el producto interno bruto per capita en dolares, el cual refleja el nivel de productividad economica por habitante en las ciudades de LATAM.</p>
 El año analizado fue 2024, se analizaron 15 ciudades de los paises: Brazil, Colombia, Argentina, México, Perú, Uruguay y Chile </p>

Las herramientas utilizadas fueron: Python-seaborn, matplotlib y JupiterNootbook </p>
# Metodologia: </p>
* <p align="justify"> Procesos principales: limpieza de datos (formatos, estandarización de columnas). En la limpieza de datos, se estandarizó los nombres de columnas para que conincidieran entre las dos tablas (todas en minusculas y separando palabras con guión bajo), varias columnas tenian diferente tipo, por ejemplo algunas columnas eran tipo object y se cambiaron a tipo float o integer y las columnas de datetime estaban como tipo object, tambien en algunas columnas se remplazo la , por el . para que los datos sean mas legibles, en la columna de unemployment se quito el %, en la columna de PIB se quitaron el . y la columna de population se calculo en cantidad absoluta </p>
* <p align="justify"> Menciona las validaciones visuales empleadas (distribuciones, outliers, tendencias generales). En el boxplot, se observa un marcado valor atipico en el comportamiento de los minutos de congestión, ya que esta fuera del rango intercuartil. En el histograma se observa mayor concentracion de PIB en rangos medios y muestran un sesgo al extremo derecho, lo que indica verias ciudades con PIB bajo </p>

# Hallazgos mas importantes: </p>
* <p align="justify"> Se observa que los paises existe cierta tendencia entre las ciudades con mayor PIB ya que presentan mayor movilidad vial como lo son México y SaoPaulo, sin embargo, no es una tendencia lineal ya que la ciudad de Montevideo tiene mayor productividad pero muy baja congestión vial, lo que nos señala que pueden existir otros factores que contribuyen a la alta congestión vial.
* <p align="justify"> La columna de JamsDelay podría requerir revisión adicional o un análisis más profundo ya que como lo muestra el boxplot marca valores atipicos.

A continuación se muestra el boxplot de tiempos de retraso (JamsDelay) </p>
<img width="520" height="476" alt="image" src="https://github.com/user-attachments/assets/fa699266-7e3a-4d1e-bb80-c66c0a57cacf" />


Conclusiones y recomendaciones: </p>
* <p align="justify"> Es necesario validar la informacion de retraso total en minutos, ya que muestra valores atipicos, durante el analisis, verificar si fue error de captura o en realidad un tema por las caracteristicas de la ciudad. La ciudad con mayor movilidad vehicular es la ciudad de México, seguido de Sao Paulo, lo que estas dos ciudades tienen en comun, es que cuentan con el mayor número de poblacion entre los paises de LATAM, lo que podria explicar esta relacion de movilidad urbana, es un tema que necesitara analisis adicionales.
* <p align="justify">  Las ciudades proritarias para inversión en infraestructura de transporte son ciudad de México y SaoPaulo, ya que son las que mayor congestión vial tienen, por lo que podria verse un aumento de PIB mejorando la movilidad.
