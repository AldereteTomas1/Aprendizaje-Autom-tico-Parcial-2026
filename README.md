## Parcial Aprendizaje Automático

# VIDEO: 
https://drive.google.com/file/d/1d6ZIqFShZ84ZzJFeuRQwD7MGD2MSuZWA/view?usp=drive_link


### Alumno: Alderete Tomás

## Modelo de Predicción: Árbol de Decisión

## Objetivo: 

Predecir si un paciente recién ingresado, tiene el sintoma de Ictericia.

## Objetivo2: 

Predecir si un paciente en la Semana 12 de sus análisis está curado.

## Objetivo 3:

Predecir si un paciente en la Semana 12 está curado, con la información del dataset completo.


### Pasos:
1. Importar las librerías de Python:
   - Pandas
   - Numpy
   - Matplotlib
   - Seaborn
   - Sklearn 

2. Realizar un análisis exploratorio de los datos:
   - Previsualización del dataset
   - Visualización de los Tipos de datos
   - Matriz de Correlación

3. Modificación del dataset:
   - Cambio de Nombres de columnas (traducción de Inglés a Español)
   - Eliminación de Columnas no utilizadas en el estudio 
   - Transformación de tipos Datos
   - Conteo de Nulos

4. EDA
   - Frecuencia de Edad
   - Frecuencia de los datos según género 

5. Objetivo 1:
   - Árbol de Decisión con metricas estandar
   - Árbol de Decisión con metricas mejoradas (con umbral bajo)
   - Árbol de Decisión con Reglas y umbral
  
6. Objetivo 2:
   - Árbol de Decisión con metricas estandar

7. Conclusiones:
   - Interpretación de los Resultados
  


### Dataset:
Columnas: 23
Registros: 1385

Información:
- Información del Paciente
- Sintomas
- Análisis / Estudios medicos

Columnas del dataset:
- Edad
- Género
- IMC 
- Fiebre
- Vómitos
- Dolor de Cabeza 
- Diarrea
- Fatiga y Dolor de Huesos
- Ictericia
- Dolor epigástrico
- Glóbulos blancos
- Glóbulos rojos
- Hemoglobina
- Plaquetas
- AST1
- ALT1
- ALT4
- ALT12
- ALT24
- ALT36
- ALT48
- RNA Base
- RNA 4
- RNA 12
- RNA EOT
- RNA EF
- Calificación histórica de referencia
- Calificación histórica  

### Resultados de EDA

## EDAD
Edad mínima: 32
Edad máxima: 61

Conclusión:
Los datos no presentan una concentración en una edad en específico, encontré una gran cantidad de datos acumulados en la máxima edad "61", en comparación al resto de edades, sin embargo, esto no es índice de que la enfermedad tiende a presentarse en pacientes mayores a 60 años

## GÉNERO

Hombre    707
Mujer     678

Conclusión:
Los datos tampoco presentan una concentración ningún género en particular

### Mejor Modelo de Predicción : 
Arbol de decisión del Objetivo1:

<img width="516" height="241" alt="image" src="https://github.com/user-attachments/assets/258644f3-ed97-4432-91ba-3ff55aea57cf" />

Conclusión: 
Luego de aplicar reglas en los síntomas, y de utilizar un data set nuevo y aleatorio, para poder poner a prueba, este mismo empezó a detectar patrones teniendo casi un 90% de precisión
Y también podemos observar que llegó a un poco más de 75% de promedio, lo que para la rama de salud es un resultado muy positivo.

### Peor Modelo de Predicción:
Arbol de decisión del Objetivo2:

<img width="499" height="206" alt="image" src="https://github.com/user-attachments/assets/eed49e4e-a73f-4f2e-b5b1-221cabed6f3b" />

Este modelo es el peor ya que tiene un mal promedio de predicción y a su vez encontramos que es muy similar a intentar predecir con azar. Esto se debe a que el objetivo en sí, está mal planteado, estoy observando sintomas del presente y queriendo adivinar el futuro, cosa que en la rama de salud es muy cambiante.
La idea que intenté plantear es muy interesante pero el resultado contiene muchos fallos

Mejorías :
- Aumentar la cantidad de registros
- Agregar pacientes SIN Hepatitis C
- Agregar Síntomas o columnas con diferentes enfermedades

 Mejoría Personal: 
- Debo mejorar el orden de las tareas y tener una organización más clara
- Debo de mejorar mis archivos, que sean más claros que información está intentando entregar

==============================

Modelos de Aprendizaje Automático

Project Organization
------------

    ├── LICENSE
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   └── raw            <- The original, immutable data dump.
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-jqp-initial-data-exploration`.
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
         └── figures        <- Generated graphics and figures to be used in reporting


--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
