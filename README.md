

Análisis Exploratorio de Datos (EDA) y Limpieza de Encuesta de Star Wars
Este proyecto se enfoca en el Análisis Exploratorio de Datos (EDA) y la limpieza de datos de un dataset proveniente de una encuesta sobre la franquicia de Star Wars. Como parte de mi experiencia aplicando para roles de Ingeniero Analista de Datos BI, este trabajo demuestra mi capacidad para transformar datos crudos en un formato listo para el análisis, identificar patrones iniciales y preparar la información para la construcción de dashboards y reportes.

Objetivos del Proyecto
Comprender la estructura de los datos: Realizar una inspección inicial para entender el tipo de datos, el número de registros y columnas, y la presencia de valores nulos.
Limpieza y preprocesamiento de datos:
Manejo de valores nulos, específicamente rellenando las respuestas "Sí/No" con un valor predeterminado de "No" cuando la información está ausente, asumiendo que la falta de respuesta implica una negativa.
Eliminación de columnas irrelevantes o con un alto grado de datos faltantes que no aportan valor significativo al análisis principal, enfocándose en las columnas más informativas para el BI.
Preparación para análisis futuros: Dejar el dataset en un estado óptimo para la exploración más profunda y la creación de visualizaciones de negocio.
Metodología
Carga y vista preliminar de los datos: Se cargó el dataset utilizando la librería pandas en Python. Se empleó df.info() para obtener un resumen de las columnas, tipos de datos y recuentos de valores no nulos.
Identificación y manejo de valores nulos: Se detectaron múltiples columnas con valores faltantes. Para las preguntas de tipo "Sí/No", se aplicó la función fillna('No') para asegurar la consistencia y completitud de estas columnas binarias, lo que es crucial para un análisis preciso de la opinión.
Selección y eliminación de columnas: Se identificaron y eliminaron columnas redundantes o con nombres genéricos (Unnamed: X) que contenían información fragmentada o duplicada de otras preguntas más completas. También se eliminaron las preguntas originales correspondientes a esas columnas fragmentadas, consolidando la información relevante en un conjunto de datos más limpio y manejable.
Resultados Clave
El proceso de limpieza redujo el dataset original de 38 columnas a 11 columnas, las cuales son más relevantes y están mejor estructuradas para el análisis. Las columnas clave resultantes incluyen:

RespondentID
Have you seen any of the 6 films in the Star Wars franchise?
Do you consider yourself to be a fan of the Star Wars film franchise?
Are you familiar with the Expanded Universe?
Do you consider yourself to be a fan of the Expanded Universe?æ
Do you consider yourself to be a fan of the Star Trek franchise?
Gender
Age
Household Income
Education
Location (Census Region)
Este dataset transformado es ahora más compacto y enfocado, lo que facilita el siguiente paso en el pipeline de BI, como el análisis demográfico de los fans, la correlación entre el fandom de Star Wars y Star Trek, y la exploración de otras variables sociodemográficas.

Tecnologías Utilizadas
Python: Lenguaje principal para la manipulación de datos.
Pandas: Librería fundamental para el análisis y la manipulación de DataFrames.
