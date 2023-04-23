# Sharks-DataCleaning Project.

![Ironhack logo](https://i.imgur.com/1QgrNNw.png) Primer proyecto como Data Analyst en [Ironhack](https://www.ironhack.com/) 🦈:

<a name="readme-top"></a>

#                                                 PROJECT SHARK

&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;<img src="https://github.com/OrianAmpuero/Project-Shark/blob/main/IMG/Shark-png.png" width="500" height="250">

<details>
  <summary>CONTENIDO:📝</summary>
  <ol> 
    <li><a href="#estructura">Estructura</a></li>
    <li><a href="#descripción-del-proyecto">Proyecto</a></li>
      <li><a href="#sobre-el-csv">CSV</a></li>
    <li><a href="#pasos-a-seguir">Pasos a Seguir</a></li>
      <li><a href="#herammientas">Herramientas</a></li>
    <li><a href="#insights">Insights</a></li>
    <li><a href="#fuente-de-datos">Fuente de Datos</a></li>

    
      </ol>
</details>


## 📁ESTRUCTURA


- |__ DATA/                         # contiene el csv limpio  
- |
- |__ IMG/                          # contiene imagénes referentes al proyecto y gráficos de los datos   
- |
- |__ SRC/                          # contiene el proceso de limpiea del csv
- |
- |__ .gitignore                    # archivo para ignorar documentos (csv original)    
- |
- |__ README.md  
    



## 🦈 PROYECTO 

El objetivo de este primer proyecto es aplicar lo aprendido en dos semanas con Python trabajando en limpieza y manipulación de datos con Pandas para un archivo CSV que trata de ataques de tiburones, con un deadline de tres días, y así poder sacar un buen estudio del mismo con nuestra propia hipotesis.



## 📋 SOBRE EL CSV

El conjunto de datos completo fue descargado el 29-09-2016; cada fila corresponde a un ataque de tiburón. 
Las columnas son:

- Case Number
- Date
- Year
- Type
- Country
- Area
- Location
- Activity
- Name
- Sex
- Age
- Injury
- Fatal (Y/N)
- Time
- Species
- Investigator or Source



## ✔️ PASOS A SEGUIR

   1) Importar los datos que se encuentran en este [SHARK LINK!](https://www.kaggle.com/datasets/teajay/global-shark-attacks).
   
   2) Se limpia el csv para quitar nulos y valores inconsistentes, eliminar duplicados, colocar los tipo de datos correctos, llevar un orden, limpiar           filas, etc...
      
   3) Tener un objetivo, para poder realizar la limpieza acorde al objetivo, separar información en varias columnas para poder trabajarlas
      mejor y asi tener un analisis mas preciso. 

   4) Utilizar todas las herramientas que sean posibles para dejar el archivo "tidy" y aplicar lo aprendido sobre el mismo archivo. 
   
   5) Presentar resultados de investigación, con visualizaciones y breakdowns.
   

## 🛠️ HERRAMIENTAS/INSTALACIONES 
<b> &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;Jupyter Notebook, Python, Pandas, Re, Matplotlib, Numpy. </b>
    
    !pip install pandas
    !pip install numpy
    !pip install ipython
    !pip install seaborn
    %matplotlib inline
   
   

## 📊 INSIGHTS 

Mi objetivo es lo siguiente:

1 - Ver el numero de registros que  hay en el archivo. Como podemos ver 

Aqui brindo toda la información de la Data Frame, de la cual vamos a trabjarla y sacar el mas alto rendimiento de ella.

![INFO - ARCHIVO CSV, SHARKS](..Screen_shots/info_general.jpg)

2 - En que temporada del año son los ataques mas frecuentes.



3 - Pais con el número mas elevado de ataques.



4 - Comparar quien sufrió mas los ataques, ya si son Hombres o Mujeres.



5 - Cuantos casos fueron registrados como Fatales, etc...



6 - Cueles fuerons las actividades que mas sufrieron dichos ataques.



7 - Que tipo de tiburon tiene mas protagonismo en este report.



8 - Numero de ataques por año, de los ultimos 15 años. 



## 💻 FUENTE DE DATOS 

- [GLOBAL SHARK](https://www.kaggle.com/datasets/teajay/global-shark-attacks).
- [NUMPY](https://numpy.org/doc/1.18/).
- [PANDAS](https://pandas.pydata.org/).
- [PYTHON](https://docs.python.org/3/library/functions.html).
- [PLOTLY](https://plotly.com/python/).
- [MATPLOTLIB](https://matplotlib.org/). 
- [SEABORN](https://seaborn.pydata.org/).





<p align="center">👆<a href="#readme-top">SUBIR</a>👆</p>
