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

Aqui brindo toda la información de la Data Frame, de la cual vamos a trabjarla y sacar el mas alto rendimiento de ella. De cual contamos con mas de 
25 mil filas, y muchos datos nulos.

![info_general](https://user-images.githubusercontent.com/125477881/233842141-1fc28dba-2990-444d-bead-ebb57d0be23f.png)

2 - En que temporada del año son los ataques mas frecuentes??

Como podemos ver en el breakdown y la imagen, la temporada con mas ataques es en la época de calor, teniendo en el primer lugar verano seguido de la primavera. 
Para ello he tenido que limpiar la columan y traspasar los datos a otra nueva columna para poder hacer el analisis. Creé una función para que me 
agrupara los meses de año a su correspondiente temporada. 

Creamos una funcion para poder analizar el numero de casos por temporada.

***

def get_season(month):
    if month in ['12', '01', '02']:
        return 'Winter'
    elif month in ['03', '04', '05']:
        return 'Spring'
    elif month in ['06', '07', '08']:
        return 'Summer'
    elif month in ['09', '10', '11']:
        return 'Autumn'
df['Year Season'] = df['Year Season'].apply(get_season)

***

![analisis_por_estacion](https://user-images.githubusercontent.com/125477881/233842384-d4b20130-49b9-464f-adef-f70ff522acb1.jpg)
![visualizacion_por_estacion](https://user-images.githubusercontent.com/125477881/233842398-8de55c77-c7bf-4e2b-bedf-e3c32e93f26b.jpg)



3 - En la siguiente imagen, veremos el ranking de los 5 primeros paises con mas ataques por tiburones. Del cual USA es el pais con mas ataques que han sido 
registrados.

![analisis_por_country](https://user-images.githubusercontent.com/125477881/233842645-327da996-492b-463b-a250-eba124d0cd0f.jpg)
![visualizacion_por_country](https://user-images.githubusercontent.com/125477881/233842665-766a8e1d-50f2-4d77-9d1e-a5067178abf5.jpg)




4 - Comparar quien sufrió mas los ataques, ya si son Hombres o Mujeres.


![analisis_por_sex](https://user-images.githubusercontent.com/125477881/233842808-78a3e2e6-92fe-438e-b13a-307e2ad13935.jpg)
![visualizacion_por_sex](https://user-images.githubusercontent.com/125477881/233842812-dfb94396-f6e5-4c62-aa72-d967ab305c8e.jpg)




5 - Que casos hubieron o resgistraron? Hubo fallecidos? Casos grabes? En el siguiente breakdown mostrarä los mas repetidos que fueron recogidos.


![analisis_por_injury](https://user-images.githubusercontent.com/125477881/233842878-777c83cd-21fc-45ad-bd0c-0a55ac6b654d.jpg)



6 - Llegados a este punto, cueles fueron algunas de las actividades que mas sufrieron dichos ataques???

![analisis_por_activity](https://user-images.githubusercontent.com/125477881/233842944-6679f02d-150e-40cf-9c8e-8b2a7e70d5f0.jpg)
![visualizacion_por_activity](https://user-images.githubusercontent.com/125477881/233842957-196ee13a-f4c1-4643-8baf-88ff68ee3b8e.jpg)


7 - Que tipo de tiburon tiene mas protagonismo en este report.

![analisis_por_species](https://user-images.githubusercontent.com/125477881/233843005-3c83e62e-5c9f-4990-ab3d-4779cc69e411.jpg)


8 - Numero de ataques por año, de los ultimos 15 años, del cual en el año 2015 fue el año con mas registros de toda la historia. 

![analisis_por_year](https://user-images.githubusercontent.com/125477881/233843033-7ee6a276-2838-4910-9107-aa97aee9c66f.jpg)


## 💻 FUENTE DE DATOS 

- [GLOBAL SHARK](https://www.kaggle.com/datasets/teajay/global-shark-attacks).
- [NUMPY](https://numpy.org/doc/1.18/).
- [PANDAS](https://pandas.pydata.org/).
- [PYTHON](https://docs.python.org/3/library/functions.html).
- [PLOTLY](https://plotly.com/python/).
- [MATPLOTLIB](https://matplotlib.org/). 
- [SEABORN](https://seaborn.pydata.org/).





<p align="center">👆<a href="#readme-top">SUBIR</a>👆</p>
