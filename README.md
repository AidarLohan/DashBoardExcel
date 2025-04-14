# DashBoard_Excel
 DataProject: Dashboard & Análisis de Datos
 
📌 Overview
	Este informe permite analizar a una población de 2000 usuarios en función de sus características de salud (como condiciones médicas y hábito de fumar), sus métricas físicas (edad, género, altura), así como su actividad física (tipo de entrenamiento, calorías quemadas, pulsaciones, duración, hidratación y sueño).

	Está diseñado para ofrecer una visión general del estado físico y los hábitos de actividad de los usuarios, con capacidad de segmentar por múltiples filtros interactivos.


📖 Descripción
	Este proyecto realiza un análisis exploratorio de una serie de registros de actividades físicas y métricas vitales de 3000 usuarios a lo largo de un año

	La muestra se compone de los siguientes campos para cada usuario y cada día de actividad:
	Información demográfica
		participant_id: Identificador único de los usuarios
		age: edad de los participantes (18-64 años)
		gender: Género (M/F/Other)
		height_cm: Altura en mm 
		weight_kg: Peso en Hectagramos
		bmi: Indice de masa corporal calculada a partir de altura y peso

	Métricas de actividad
		activity_type: Tipo de ejercicio realizado (Running, Swimming, Cycling, etc.)
		duration_minutes: Duración de la actividad realizada
		intensity: Intensidad de la actividad (Low/Medium/High)
		calories_burned: Estimación de las calorías quemadas
		daily_steps: Pasos diarios

	Health Indicators
		avg_heart_rate: Ritmo cardiaco medio durante la actividad
		resting_heart_rate: Ritmo cardiaco en reposo
		blood_pressure_systolic: Presión sanguínea sistólica
		blood_pressure_diastolic: Presión sanguínea diastólica
		health_condition: Condiciones de salud
		smoking_status: Fumador (Never/Former/Current)

	Lifestyle Metrics
		hours_sleep: Horas de sueño (en décimas de hora)
		stress_level: Nivel de stress diario (1-10)
		hydration_level: Cantidad de agua ingerida (en dl)
		fitness_level: Puntuación de fitness calculada en base a la actividad acumulada

🛠️ Herramientas Utilizadas
	- Excel 365

📁 Dashboard_Excel_/
│
├── 📊 Proyecto.xlsx             # Archivo principal del dashboard
├── 📁 datos/                    # Carpeta con los datos de entrada
│   └── 📁 Originales
|		└── health_fitness_dataset.csv
├── 📄 README.md                 # Este archivo

🧩 Secciones del Dashboard
	- Resumen General: Indicadores principales como edad media, número total de actividades, pulsaciones promedio, hidratación, horas de sueño, etc.
	- Distribuciones Demográficas: Por edad, género, altura y condiciones médicas.
	- Actividad Física: Número de entrenamientos, calorías quemadas, intensidad, tipo de actividad.
	- Cruces de Métricas: Comparativa entre pulsaciones y calorías, intensidad por tipo de actividad, entrenamientos por edad y género.

📊 Análisis de datos

	Tras un previo análisis se hacen las siguientes observaciones en la muestra de datos presentada:

	1- El peso, crece en todos los usuarios a lo largo del periodo analizado (1 año) de una forma exagerada.
	2- La proporción de hombres/mujeres está muy equilibrada, existiendo un 2,13% de los usuarios que no han definido el sexo.
	3- La distribución del tipo de actividad entre hombre/mujer están muy equilibrados.
	4- Hay un par de usuarios con registros de pasos negativos. Se eliminan de la muestra por inconsistentes.
	5- El índice bmi, no varía a lo largo de todo el periodo, siendo que está calculado a partir del peso que evoluciona de forma ascendente durante todo el periodo de análisis. Se elimina la columna.
	6- La columna restingHeartRate, tienen valores no coherentes, variando entre 511 y 800. Se elimina la columna
	7- Las presiones sanguíneas (sistólica y diastólica) son constantes durante todo el año.


📊 Resultados y Conclusiones
	- Las mujeres presentan un gasto calórico promedio superior al de los hombres.
	- La mayoría de los entrenamientos se concentran en personas de entre 40 y 49 años.
	- El 72% de los usuarios no reporta condiciones médicas significativas.
	- Un alto porcentaje de la población realiza actividad de intensidad media.
	- El grupo de edad <30 realiza más entrenamientos con alta intensidad.
	- No existe correlación entre las horas de sueño y las variables Stress, fitness, pulso medio de las actividades, calorías o tiempo de entreno
	- No existe tampoco correlación entre el stress y esas mismas variables.

✒️ Autor

	J.Raúl Beltrán Crespo (beltran.joseraul@gmail.com)

⚙️ Origen de Datos

Jija Taher

https://www.kaggle.com/datasets/jijagallery/fitlife-health-and-fitness-tracking-dataset
Originalmente el dataset tenía los datos de 3000 usuarios. Por cuestiones de gestión de archivos se eliminaron los usuarios con id del 2001 al 3000	