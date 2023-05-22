# **Evaluación Sprint 1 Módulo 3**
## Elisa Jimenez y Lidya Descals
### **Machine Learning**


---

En este repositorio podéis encontrar los ejercicios de la evaluación correspondientes al sprint 1 del módulo 3.

>Las librerías con las que se ha trabajado en este repositorio son:
>
>- [NumPy](https://numpy.org/)
>- [Pandas](https://pandas.pydata.org/) 
>- [Matplotlib](https://matplotlib.org/)
>- [Seaborn](https://seaborn.pydata.org/)
>- [SciPy](https://scipy.org/)
>- [Statsmodels](https://www.statsmodels.org/stable/index.html)
>- [Sklearn](https://scikit-learn.org/stable/)
>- [Imblearn](https://imbalanced-learn.org/stable/)
>- [Researchpy](https://researchpy.readthedocs.io/en/latest/)
>- [Itertools](https://docs.python.org/3/library/itertools.html)
>- [Regex](https://docs.python.org/3/library/re.html)

---

El repositorio consta de tres carpetas:


- **regresion-lineal**

    - Esta carpeta contiene 16 archivos en formato Jupyter Notebook, que detallan el proceso seguido para realizar una serie de modelos de regresión lineal. 
    
        Primero, hubo que seleccionar nuestras variables de un conjunto de datos general, realizar una exploración analítica y visual, y a continuación limpiar ese nuevo dataset para dejarlo preparado para su uso. 
        
        Posteriormente, realizamos sobre el conjunto una serie de test estadísticos para comprobar si cumplía con los requisitos para poder ejecutar un modelo de regresión lineal, pero no pudimos normalizar la variable respuesta. No obstante, con el propósito de practicar, continuamos realizando los siguientes pasos, tanto los que serían necesarios para realizar un modelo de Decision Tree o un Random Forest (como la estandarización de las variables predictoras numéricas o el encoding de las variables predictoras categóricas) como los que no, como es el caso del ANOVA. 
        
        Por último, llevamos a cabo los modelos de regresión lineal, el Decision Tree y el Random Forest, y comparamos sus métricas en el último Jupyter Notebook.

        Es importante destacar que el proceso de trabajo que se puede ver en estos archivos ha sido modificado en varias ocasiones a medida que íbamos aprendiendo cosas nuevas y solucionando dudas, causando esto que, al rehacer el encoding con intención de ver si las métricas mejoraban con un nuevo enfoque, el trabajo que bifurcara en dos pruebas distintas con diferentes planteamientos respecto a la codificación. 

        Los resultados finales, aunque mejores a medida que íbamos puliendo detalles, nunca llegan a constituir un modelo predictivo fiable, posiblemente por el tamaño del conjunto de datos.



- **regresion-logistica**
  
    - Esta carpeta contiene 6 archivos en formato Jupyter Notebook, que muestran el desarrollo de un modelo predictivo de regresión logística. 

        De nuevo, al igual que en el modelo de regresión lineal, comenzamos explorando nuestro dataset, tanto analítica como visualmente.

        A continuación procedimos a realizar la estandarización de las variables predictoras numéricas y el encoding de las variables predictoras categóricas, así como el paso de nuestra variable respuesta de tipo object a integer.

        A diferencia de la regresión lineal, para este modelo tuvimos que usar un método para balancear el conjunto, aunque la diferencia entre el grupo mayoritario y el minoritario no era demasiado grande y hubiera sido interesante, de tener más tiempo, ver cómo otros métodos de balanceo (o incluso su ausencia) podrían haber afectado al resultado final.

        En último lugar, del mismo modo que en el modelo de regresión lineal, procedimos a ejecutar los modelos de regresión logística, Decision Tree y Random Forest. Las métricas de los tres modelos, así como nuestras conclusiones al respecto, se pueden encontrar en el último Jupyter.

        En este caso, los resultados finales sí son satisfactorios, con unas métricas robustas y estables que nos indican que el modelo predictivo es fiable.


    
- **datos**:

    - **datos-regresion-lineal**

        Esta carpeta consta de 10 archivos, 9 de ellos en formato .csv y un .png. Los archivos en formato .csv son los diferentes conjuntos de datos que hemos ido utilizando y generando durante el proceso de desarrollo del modelo de regresión lineal. El archivo .png es una gráfica (concretamente un heatmap) que se nos pedía en un ejercicio que guardásemos.

    - **datos-regresion-logistica**

         Esta carpeta consta de 4 archivos, dos de ellos en formato .csv y otros dos en formato .pkl . Se trata de los difentes conjuntos de datos que hemos ido utilizando y generando durante el proceso de desarrollo del modelo de regresión logística. El archivo original se descargó en .csv, pero a medida que trabajábamos con él nos era más útil guardarlo en formato pickle. Sin embargo, el último archivo, referente a las métricas, es de nuevo un .csv .


---
---



>## **Columnas originales del dataset SocioEconomic Country Profiles**
>
>A continuación se detallan los nombres originales de las columnas del dataset usado para los modelos de regresión logística. Hemos decidido conservarlos dado que, al renombrar las columnas como parte del proceso de limpieza, nos parecía más práctico eliminar las aclaraciones que se dan aquí entre paréntesis. 
>
>- Country
>- Region
>- Population in millions (2017)
>- Population density (per km2, 2017)
>- Urban population (% of total population)
>- GDP per capita (current US$)
>- Health: Total expenditure (% of GDP)
>- Health Care Index	
>- Health: Physicians (per 1000 pop.)
>- Quantity of Physicians (per 1000 pop.)
>- Quality Of Life Index	
>- Purchasing Power Index
>- Safety Index
>- Pop. using improved drinking water: urban(%)	
>- Pop. using improved drinking water: rural (%)	
>- Pollution index
>- Life expectancy at birth, total (years)
