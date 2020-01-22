<img src="logo.png" alt="Logo_tableau" style="width: 30px;"/>

# Projet Tableau
[Voir le projet Tableau](https://public.tableau.com/profile/sandrine.henry#!/vizhome/marchspublics/Histoire1?publish=yes)

## Objectif : 
Mettre en pratique les compétences acquises en Business Intelligence à l'aide du logiciel Tableau avec le dataset de notre choix.

## Choix du dataset : 

> "Le jeu de données représente la liste des marchés supérieurs à 20 000 € passés par la collectivité parisienne. Cette liste précise l’objet du marché, le nom du titulaire, le montant du marché sur sa durée complète, sa durée, le budget de rattachement, l’article du Code des marchés publics relatif au mode de mise en concurrence, la nature de l’achat concerné.[https://www.data.gouv.fr/fr/datasets/liste-des-marches-de-la-collectivite-parisienne/]


## Résultats : 

#### NOMBRE D'ENREGISTREMENTS PAR ANNEE : 

**Slide 1** : je regarde dans un premier temps le nombre de contrats par an. Il y a une petite quantité de contrats qui n'ont pas d'année. Je les exclus avec l'option filtre.
<br/>**Analyse** : après une baisse du nombre de contrat en 2014, on observe depuis une hausse constante année par année, avec en 2017 un nombre de contrats plus important qu'en 2013.
  
#### NATURE DE MARCHE PAR ANNEE : 

**Slide 2** : Je cherche à voir la nature des contrats par année. Dans un tableau, je croise les années de notifications (toujours en excluant "NULL") avec le champ "Nature du marché".
<br/>**Analyse** : les contrats de Services, comptent pour plus de 50% des contrats notifiés. En 2017, la part était de 55%. Les contrats "Travaux" comptent pour 1/3 de contrats et les 15% restant concernent les contrats de "Fournitures". Nous verrons plus tard à quoi cela correspond.

**Slide 3** : Pour que cela soit plus parlant, je crée une visualisation. J'ai choisi un stacked chart.

**Slide 4** _Evolution par Nature de marché par Année_: le tableau et le graphique permettent d'observer les évolutions du nombre de contrat par nature de ces derniers mais je décide de faire une dernière slide pour calculer l'évolution du nb de contrats par année. 
J'ai utilisé le tuto suivant pour le faire : https://www.theinformationlab.fr/2018/02/02/evolutions-annee-tableau/
<br/>**Analyse** : ce tableau nous permet de confirmer la hausse du nb de contrat en 2017 vs 2016 et ce pour les 3 types. L'évolution la plus forte est pour les contrats "Travaux" (+29%), puis "Fourniture" (+15%) et enfin "Services" (+10%).

**Slide 5** : Je crée un dashboard qui affiche toutes les visualisations créées afin avoir une vue d'ensemble. 

#### SITUATION GEOGRAPHIQUE :

Je regarde ici comment se répartissent les attributions de contrats sur un plan géographique. 

**Slide 6** _Situation géographique des fournisseurs_: Je crée une visulaisation qui permet de voir la position géographique des entreprises avec lesquelles paris a signé un contrat. 
<br/>**Analyse** : suivant toute logique, la majorité des contrats ont été signés avec des entreprises d'Ile de France. Mais on voit que les entreprises se trouvent dans toute la France. 
    
**Slide 7** _Répartition des contrats entre IDF et Hors IDF_: le graphique montre la répartition des contrats entre IDF et Hors IDF. 
<br/>**Analyse** : on voit que plus des 3/4 des contrats sont signés en IDF. Ce qui confirme ce qui a été présenté dans les slides précédentes. 
 
**Slide 8** _Situation géographique des fournisseurs (zoom IDF)_ : Il s'agit de faire un zoom sur l'IDF. Je crée une variable qui consiste à regrouper tous les codes postaux d'IDF et de renommer cet ensemble "IDF".
<br/>**Analyse** : Avec ce zoom, on voit que le plus grand nombre de contrats sont à Paris puis dans ce que l'on appelle la "Petite couronne" (villes limitrophes de Paris).
    
**Slide 9** _Situation géographique des fournisseurs par Nature de contrat_ : Je regarde ici la Répartition des contrats entre IDF et Hors IDF par Nature de contrat.
<br/>**Analyse** : on voit que les contarts de type "Service" et "Travaux" sont le plus souvent signés avec des entreprises d'IDF. Pour ce qui est des contrats de type "Fourniture", il n'y a pas de grandes différences. 
    
#### ANALYSE DES PRIX :

**Slide 10 /** _Moyenne des Montants max et min par année et zone géographique)_ : pour cet partie, je crée un line chart. 
<br/>**Analyse** : on voit qu'au fil des années, bien que le montant (min ou max) soit plus bas pour les entreprises Hors IDF, ce dernier a tendance à se rapprocher de celui des entreprises en IDF.


