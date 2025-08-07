# Analisis-historico-Juegos-Olimpicos-1896-2016

Curso: Data Science 2

Fecha: Agosto 2025

Alumno: Duarte Juliana Ines

Dataset : Olimpiadas 1896-2016

**Audiencia**

El análisis de este conjunto de datos resulta especialmente valioso para periodistas deportivos y medios de comunicación, ya que les permite enriquecer sus coberturas con información precisa, visualizaciones interactivas, gráficos comparativos e infografías basadas en evidencia histórica. Este tipo de recurso aporta profundidad a las historias deportivas, permite identificar tendencias significativas y ofrece un enfoque más analítico y riguroso en la narrativa de los Juegos Olímpicos. Asimismo, los comités olímpicos nacionales y las federaciones deportivas pueden utilizar esta información para hacer un seguimiento detallado del rendimiento de sus atletas, identificar patrones de éxito, establecer metas de mejora y tomar decisiones estratégicas respaldadas por datos concretos.

Por ultimo, tanto atletas como entrenadores pueden beneficiarse directamente del análisis. Para los atletas, acceder a estadísticas históricas y comparativas les permite evaluar su progreso frente a referentes internacionales, conocer marcas anteriores y entender en qué disciplinas o contextos han sobresalido otros deportistas. Por su parte, los entrenadores pueden utilizar esta información como insumo para diseñar planes de entrenamiento más específicos, ajustar estrategias según el análisis de desempeño pasado, y detectar oportunidades de mejora basadas en datos reales y objetivos.

**Motivación**

Se desea llevar a cabo el analisis de este Datasets ya que actualmente soy jugadora federada de Basquet Femenino en primera división, por lo que siempre trato de informarme, analizar y conocer metricas tanto propias del basquet como en otros deportes en general.

**Introducción y descripción de datos**

Este conjunto de datos contiene registros detallados de los eventos olímpicos y de los atletas que participaron en ellos desde el año 1896 hasta 2016. Cada fila en el conjunto de datos representa a un atleta individual e incluye varios atributos relacionados con su información personal, el país que representan, los detalles del evento olímpico en el que participaron y los resultados que lograron. A continuación, se describe cada columna incluida en el conjunto de datos:

Nombre: El nombre completo del atleta.
Género: El género del atleta, generalmente representado como 'M' para masculino y 'F' para femenino.
Edad: La edad del atleta en el momento de su participación en los Juegos Olímpicos.
Altura: La altura del atleta en centímetros.
Peso: El peso del atleta en kilogramos.
Equipo: El nombre del equipo o delegación que el atleta representa, usualmente corresponde a su país.
Código del País: El código de tres letras que representa el país asociado al atleta (por ejemplo, USA para Estados Unidos, GBR para Gran Bretaña).
Juego: El evento olímpico o deporte específico en el que compitió el atleta.
Año: El año en que el atleta participó en los Juegos Olímpicos.
Temporada: La temporada de los Juegos Olímpicos (ya sea Verano o Invierno).
Ciudad: La ciudad sede donde se llevaron a cabo los Juegos Olímpicos.
Deporte: La categoría deportiva general en la que compitió el atleta (por ejemplo, Atletismo, Natación, Gimnasia).
Evento: El evento específico dentro del deporte en el que compitió el atleta (por ejemplo, 100m Libre, Salto de Longitud, Maratón).
Medalla: El tipo de medalla que ganó el atleta, si ganó alguna (Oro, Plata, Bronce). Si el atleta no ganó una medalla, este campo estará vacío.

**Fuente**

https://www.kaggle.com/datasets/harshvgh/olympics?resource=download.

**Hipotesis general**

"La mayoría de los participantes en las Olimpiadas se concentra en un rango etario promedio de 23 años, con una edad máxima de alrededor de 50 años, ademas en el Top 10 de los deportes con mayor cantidad de medallas, la participación masculina continúa siendo predominantemente superior, aunque en los últimos años la proporción de hombres y mujeres se ha equilibrado en comparación con décadas anteriores. Por otro lado, la media de las alturas difieren considerablemente entre géneros, y no se observa una relación clara entre altura y peso en la mayoría de los casos"

Para el desarrollo de la misma sera necesario analizar muchos de los factores claves del Dataset elegido ya que es necesario investigar en primer medida el rango etario de los participantes (que se realizara por rango para poder identificar mejor la distribución de cada grupo), luego distinguir el genero de los mismos, analizar la contextura fisica de ellos tanto peso como altura y finalmente introducir la información de las medallas ganadas. Ademas se puede analizar información complementaria que ayude a entender el transfondo de lo que se busca en la hipotesis planteada.

**Objetivos a evaluar como guía para el analisis de graficos - Hipotesis especificas**

1) Evaluar si la mayoría de los atletas olímpicos se encuentran en el rango de edad de 18 a 25 años, reflejando el pico de rendimiento físico en deportes competitivos y finalizando su actividad a los 50 años, y evaluar si la participación de menores de 18 años representa la proporción más pequeña debido a las altas exigencias del rendimiento.

2) Evaluar si la altura media (percentil 50) de los hombres es significativamente mayor que la de las mujeres y comparar la dispersión de alturas (amplitud del rango intercuartilico - IQR) para determinar si es mayor entre los hombres o mujeres; además, analizar la simetría de la distribución de la altura en mujeres respecto a los hombres y comparar el percentil 75 de las mujeres con el percentil 25 de los hombres para identificar posibles coincidencias.

3) Descubrir los paises que lideran el medallero olimpico y con una mayor proporción de medallas de oro. Ademas evaluar la distribución de las medallas en los 10 paises del Top e identificar el pais con menor cantidad de medallas de plata

4) Evaluar la relación entre altura y peso de los atletas, si se demuestra un aumento en peso conforme incrementa la altura, con patrones diferentes entre hombres y mujeres, y con algunos atletas que se desvían significativamente de la tendencia general, evaluar que sexo es mas disperso.

5) Evaluar si los deportes de equipo estan liderados por el género masculino en el top 3 de disciplinas con más medallas, contribuyen significativamente al total de medallas, con un sesgo de género; en particular, se piensa que el fútbol destaca en participación masculina y el hockey en femenina, mientras que en deportes como el básquet la participación de mujeres es casi nula.

6) Evaluar la participación femenina en las Olimpiadas, como ha crecido de manera constante desde 1960, y analizar si actualmente ha alcanzado la igualdad con la participación masculina, mientras analizar si ambos géneros han mostrado un crecimiento sostenido en su representación olímpica.

**Contexto comercial**

El análisis de este conjunto de datos olímpicos tiene un alto valor comercial y social, especialmente en el ámbito deportivo y en organizaciones vinculadas al deporte de alto rendimiento. Los datos históricos de rendimiento y características de los atletas permiten a instituciones deportivas, clubes y federaciones identificar patrones de éxito, entender tendencias de desarrollo físico en diversas disciplinas y evaluar el impacto de factores demográficos y físicos sobre los logros deportivos. Esto es particularmente valioso en un contexto donde la mejora continua en la preparación de los atletas es clave para alcanzar el éxito y en el que la información detallada sobre los competidores y sus características físicas proporciona una ventaja estratégica. Además, permite a estas organizaciones ajustar sus programas de entrenamiento y selección de atletas para optimizar el rendimiento, y dirigir sus recursos en función de los perfiles más exitosos por deporte, género y país.

**Contexto analitico**

Desde una perspectiva analítica, el proyecto implica la implementación de un modelo de machine learning enfocado en clasificar y predecir patrones de rendimiento en función de múltiples variables, como edad, género, contextura física, ciudad, deporte y país de origen. Este modelo permitirá evaluar hipótesis sobre las características comunes entre los atletas exitosos y medir el impacto de factores como la altura, el peso y la nacionalidad en la obtención de medallas. Además, se empleará para detectar si existen patrones significativos en la evolución de la participación femenina, los deportes de equipo con mayor sesgo de género, las edades óptimas de rendimiento en diferentes disciplinas y demás. Estos análisis ayudarán a mejorar la toma de decisiones en la preparación de atletas, personalización de entrenamientos y estrategias de selección, así como a entender mejor la evolución de la diversidad en los Juegos Olímpicos, respondiendo a preguntas clave sobre equidad y representación en el deporte de alto rendimiento.
