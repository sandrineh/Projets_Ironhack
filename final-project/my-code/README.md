# [Instagram : Prédiction des likes pour des comptes d'éditeurs et de libraires]

**[Sandrine Henry]**

**[IronHack Paris Juin 2019]**

## Overview

Sélection et apprentissage supervisé d'un modèle prédiction - XGBOOST - afin de déterminer le nombre de likes des publications sur Instagram. Et plus particulièrement pour deux acteurs du secteur du livre : les éditeurs et libraires.<br/>

* Technologies and tools :
	* Python
	* Statistical analysis
	* Data visualization
	* Jupyter Notebook
	* Tableau
	* Machine Learning
	* Natual Language Processing
    

## Data Preparation

### Dataset

Partie d'une base de données construite précédement, j'ai conservé les comptes instagram des éditeurs et libtraires. <br/>
![Editeurs_libraires_instagram](images/edi_lib_insta.png)

A l'aide des librairies `SELENIUM` pour automatiser le chargement des pages et `BEAUTIFULSOUP`, j'ai ensuite scrappé les données désirées - les 12 publications des comptes sur instagram - pendant un mois, du 15 oct. au 15 nov.

<a href="https://github.com/sandrineh/data-labs/blob/master/final-project/my-code/PROJET_FINAL_ETAPE_WEBSCRAPING.ipynb">Webscraping</a> et <a href="https://github.com/sandrineh/data-labs/blob/master/final-project/my-code/PROJET_FINAL_ETAPE_WEBSCRAPING_SUITE.ipynb">Webscraping suite</a>

### Data Wrangling and Cleaning

Pour enrichir le dataset, je me suis ensuite référée aux lectures relatives aux bonnes pratiques sur instagram qui mettent en avant les notions de jour, d’heure de publication, de longueur de texte, du bon usage des hashtags...j’ai créé les colonnes en conséquence. <br/>
J’ai par la suite supprimé les colonnes relatives à la localisation trop peu renseignées et enfin j’ai supprimé les doublons.
<br/>
Au final je me suis retrouvée avec un dataset de 23K publications (lignes) et 29 colonnes.

### Data Storage

**Dataset** : <a href="https://github.com/sandrineh/data-labs/tree/master/final-project/my-code/data">projet_ironhack_insta_final.csv</a>


## Data Analysis

### Overview

Overview the general steps you will go through to analyze your data in order to test your hypothesis.

### Data Exploration and Visualization

* Document each step of your data exploration and analysis.
* Print charts to demonstrate the effect of your work. Charts make your presentation look good too.
* If you use ML in your final project, also describe your feature selection process.

### Model Training and Evaluation

* Train your ML model, produce results, and evaluate.
* This is an iterative process. Try your best to improve your model performance by:
	* More data cleaning.
	* Try different models and select one that is the simplest yet produce the best result.
	* Try advanced techniques and see if they improve the result.

## Conclusion
<a href="https://sandrineh.github.io/docs/Projet_Ironhack_Final_Janvier_2020.pdf">Présentation du projet</a>
<a href="https://eleonoreh.pythonanywhere.com/">![WebApp_Prediction_instagram](images/le_test_ultime.png)</a>