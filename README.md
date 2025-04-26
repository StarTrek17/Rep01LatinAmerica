# Rep01LatinAmerica
primer repositorio de IEEE LatinAmerica

![PngGraphicalAbstract](https://github.com/user-attachments/assets/a19645a7-b196-4bc4-b72c-e13abe1a2e6f)


Resources and extra documentation for the manuscript "Replacing Missing Data" published in IEEE Latin America Transactions. The code is organized by the type of process:
I.-    Repositorio de datos
       I.1.-   Repositorio ISBSG
II.-   Calidad de datos
       II.1     MySql. Filtros de datos ISBSG
III.-  Muestra de datos de experimentación
       III.1    Lenguaje R. Selección de muestra aleatoria de 400 proyectos M400
IV.-   Remplazar datos faltantes M400
       IV.1     MySql. La moda en variables categóricas
       IV.2     MySql. Variable numérica líneas de código
       IV.3     MySql. Variable numérica tamaño máximo de equipo 
V.-    Normalizar muestra M400 de datos completos
       V.1      Lenguaje R. Normalizar muestra M400
VI.-   Modelo de predicción de esfuerzo
       VI.1     Lenguaje R. Modelo de variable independiente de esfuerzo NWEL1
       VI.2     Lenguaje R. Coeficientes de interrelación entre variable independiente y dependientes
       VI.3     Lenguaje R. Modelo NWEL1 ajustado
VII.-  Precisión del modelo de predicción de esfuerzo
       VII.1    MySql.-   Coeficientes de interrelación en M400
       VII.2    MySql.-   Esfuerzo de trabajo estimado NWEL1est
       VII.3    MySqñ.-   Métricas de precisión de NWEL1est
       VII.4    MySql.-   Precisión del estimado NWEL1est con la muestra M400
________________________________________
Dataset and subsets
The database files are in the folder "Dataset - Replacing Missing Data in a Set of Historical Projects". In this folder, you will find the references to original ISBSG database, the subsets used for training process in the "Training T-Subset" folder and the subsets used for validation process in the "Validation V-Subset" folder. In this folders, all the subsets are in txt format for copying and pasting into the code.
Codes
Pré processing
The code for preprocessing is in the folder "MySql - Pre-processing code," where you can find the script used to prepare the database for use in the MySql process. In this Mysql notebook, you just need to use the previously described CSV T-subset and V-subset.
Predict
The prediction codes are in two folders: "R - Algorithms for prediction model" which contains the effort prediction models using R, and "Excell - Algorithms for other predictions," which contains the calculus for MMRE, PRED(25)  and MAE validation metrics.

