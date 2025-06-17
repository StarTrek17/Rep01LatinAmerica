# Rep01LatinAmerica
primer repositorio de IEEE LatinAmerica

![PngGraphicalAbstract](https://github.com/user-attachments/assets/a19645a7-b196-4bc4-b72c-e13abe1a2e6f)


# Rep01LatinAmerica
primer repositorio de IEEE LatinAmerica

![PngGraphicalAbstract](https://github.com/user-attachments/assets/a19645a7-b196-4bc4-b72c-e13abe1a2e6f)


Resources and extra documentation for the manuscript "Replacing Missing Data" published in IEEE Latin America Transactions. The code is organized by the type of process:

I.-    Repositorio de datos.
       Este proceso decide cual será el repositorio de donde se extraen los datos de experimentación.
       I.1.-   Repositorio ISBSG.
               El proceso selecciona al repositorio ISBSG como el repositorio de datos de investigación.
               
II.-   Calidad de datos.
       Durante este proceso se depuran los datos del repositorio de acuerdo a criterios de calidad ISBSG.
       II.1     MySql. Filtros de datos ISBSG.
                Pone en ejecución los criterios de calidad sugeridos por ISBSG.
       II.2	    Datasets.
       
III.-  Muestra de datos de experimentación 
       Del conjunto general de datos ISBSG con calidad, se toma una muestra aleatoria de datos.
       III.1    Lenguaje R. Selección de muestra aleatoria de 400 proyectos M400.
                Del dataset ISBSG depurado por calidad, se selecciona una muestra aleatoria
                de 400 proyectos.
       III.2	    Datasets.
       
IV.-   Remplazar datos faltantes M400.
       Cubre los huecos de información producidos por la presencia de datos faltantes en la muestra aleatoria,
       tanto para variables categóricas como para variables numéricas.
       IV.1     MySql. La moda en variables categóricas.
                Rellena los datos faltantes presentes en las variables categóricas.
       IV.2     MySql. Variable numérica líneas de código.
                Rellena los datos faltantes presentes en la variable numérica LOC.
       IV.3     MySql. Variable numérica tamaño máximo de equipo.
                Rellena los datos faltantes presentes en la variable numérica MAXTEASZE.              
       IV.4	    Datasets.
       
V.-    Normalizar muestra M400 de datos completos.
       La muestra de datos completos, resultado del relleno de datos faltantes, requiere uniformizar
       sus valores mediante un proceso de normalización facilitado por el lenguaje R.
       V.1      Lenguaje R. Normalizar muestra M400.
                Se utiliza la función de valor mínimo-máximo para normalizar cada variable
                de la muestra M400.
       V.2	    Datasets.
       
VI.-   Modelo de predicción de esfuerzo.
       Se define un modelo de relación entre la variable independiente NWELL1 y las
       variables dependientes obteniendo además los coeficientes de interrelación
       entre ambas variables para significar las variables más significativas que
       sirven para ajustar el modelo.
       VI.1     Lenguaje R. Modelo de variable independiente de esfuerzo NWEL1.  
                Define la relación entre la variable independiente de esfuerzo NWEL1
                y las variables dependientes.
       VI.2     Lenguaje R. Coeficientes de interrelación entre variable independiente y dependientes.
                Mediante una función del lenguaje R se determinan los coeficientes de interrelación
                del modelo y con ellos las variables más significativas.
       VI.3     Lenguaje R. Modelo NWEL1 ajustado.
                Utilizando las variables más significativas se ajusta el modelo de interrelación.
        VI.4	    Datasets.

VII.-  Precisión del modelo de predicción de esfuerzo.
       Utilizando métricas de precisión se logra determinar la exactitud y validez 
       del modelo propuesto de predicción de esfuerzo.
       VII.1    MySql.-   Coeficientes de interrelación en M400.
                Utilizando funciones MySql se define un conjunto de datos que incluye las variables 
                del modelo ajustado y sus coeficientes de interrelación respectivos.
       VII.2    MySql.-   Esfuerzo de trabajo estimado NWEL1est.
                Aplicando el modelo ajustado, se calcula el esfuerzo de trabajo estimado NWEL1est.
       VII.3    MySql.-   Métricas de precisión de NWEL1est.
                Aplicando métricas de precisión comunmente aceptadas, se obtiene la exactitud del modelo.
       VII.4    MySql.-   Precisión del estimado NWEL1est con la muestra M400.
                Verificando los valores obtenidos por las métricas, se concluye que nuestro
                modelo de predicción de esfuerzo es válido.
       VII.5    Datasets.
________________________________________
Dataset and subsets
The database files are in the folder "Dataset - Replacing Missing Data in a Set of Historical Projects". In this folder, you will find the references to original ISBSG database, the subsets used for training process in the "Training T-Subset" folder and the subsets used for validation process in the "Validation V-Subset" folder. In this folders, all the subsets are in txt format for copying and pasting into the code.
Codes
Pré processing
The code for preprocessing is in the folder "MySql - Pre-processing code," where you can find the script used to prepare the database for use in the MySql process. In this Mysql notebook, you just need to use the previously described CSV T-subset and V-subset.
Predict
The prediction codes are in two folders: "R - Algorithms for prediction model" which contains the effort prediction models using R, and "Excell - Algorithms for other predictions," which contains the calculus for MMRE, PRED(25)  and MAE validation metrics.





