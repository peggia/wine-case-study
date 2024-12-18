# wine-case-study
Le marché du vin aux USA

## Contexte
Etude de cas effectué lors du passage de la certification Data Analyste du 14 au 16 Octobre 2024.

![image](https://github.com/user-attachments/assets/5f0543da-4117-43f3-9159-a36140ce443f)

## Contenu de repository
* Jeu de données apres prétraitement (df_wine)
* Jupyter notebook pour le prétraitement et l'analyse exploratoire du jeu de données
* Ficher power BI contenant le Dashboard final, après analyse et sélection des indicateurs pertinents

Note: Pour utiliser le fichier PowerBI, après ouverture dans l'application Power BI, menu Accueil, choisir l'option "Transformer les données" puis "paramètres de la source des données" puis "changer la source", et selectionner le fichier df_wine prélablement copié en local dans votre ordinateur.

![image](https://github.com/user-attachments/assets/fd74b950-f7a4-4fc7-93da-1f3baa2e3459)

## Analyse exploratoire et préparation des données
### Pré-traitements
* Suppression des doublons
* Suppression des vins dont le pays et/ou le prix n’étaient pas renseignés (~6%)
* Ajout de la colonne millésime
### Méthodologie
Analyse descendante du marché aux Etats-Unis: 
* Tous les vins 
* Les vins français
* Les vins de Bourgogne 
* Comparaisons du vin Domaine des Croix (Pinot Noir, millésime 2016, 94/100)

### Faits marquants
1. Les prix des vins français aux USA restent plus élevés que les vins locaux
2. Les vins français sont bien représentés (2è position après les USA)
3. Les vins français sont dans le TOP 5 des pays avec des vins notés 100/100
4. Avec une note moyenne de 88/100, les vins français sont en 8ème position sur un total de 43 pays producteurs
5. Les prix des vins français aux USA restent plus élevés que les vins locaux américains
6. Les vins français sont bien représentés (2è position après les USA en nombre total de vins présents sur le marché)
7. Les vins français sont dans le TOP 5 des pays avec des vins notés 100/100
8. Avec une note moyenne de 88/100, les vins français sont en 8ème position sur un total de 43 pays producteurs.

## Dashboard Power BI
1. Tous les vins aux USA
![image](https://github.com/user-attachments/assets/b8025fa6-4383-40bd-b4a9-02706b2bfc7b)

2. Les Vins Français vendus aux USA
![image](https://github.com/user-attachments/assets/07f0f7b4-4a39-44a9-a95e-fd32f77a05d4)

* Notez que toutes les régions ne sont pas affichées. Il manque le Beajoulais, Bordeaux et le Sud-ouest (voir section Difficultés rencontrées).
  
3. Les Vins de Bourgogne vendus aux USA
![image](https://github.com/user-attachments/assets/ff3f8f46-7e9d-44d6-bdb6-63867d205ff7)

4. Les Pinots Noirs vendus aux USA
![image](https://github.com/user-attachments/assets/65594c0d-416a-4790-ba40-a0c85b8623b1)

## Discussions
![image](https://github.com/user-attachments/assets/6caeb550-dd51-42b9-b4c0-ead51f72eb3d)

## Conclusions et Recommandations
![image](https://github.com/user-attachments/assets/6ba5cab2-561a-4ae2-93d8-a33f7650d5e7)

## Difficultés rencontrées
1. Extraction du millésime à partir de la dénomination du vin. Il a fallu plusieurs aller-retours entre le notebook et le Power BI, pour trouver une expression regex qui semble marcher !
2. Problème avec l'utilisation des emplacements géographiques dans Power BI. En effet, la région "Southwest France" était placée au Cameroun et non pas en France ! Aussi les vins de Bordeaux et du Beajoulais ne sont pas nonplus affichés sur la carte de France (Les noms ne sont pas considérés comme de "provinces" par Power BI peut etre ?). Pour résoudre ce problème il faudrait peut-etre se baser sur des cordonnées (latitude, longitude), en ajoutant une colonne supplémentaire ?

## Merci!
:wine_glass:
:purple_heart:
:heart:
![image](https://github.com/user-attachments/assets/9960eda5-a7ed-4a92-9bd7-2e9bccef6a12)

source de l'image: https://www.carnetdevins.fr/guide-des-regions/





  
