# Analyse-de-la-chaine-de-valeur-du-cacao-en-Cote-d'Ivoire-Power-BI-Challenge-Mars-2026

![ezgif com-speed(4)](https://github.com/user-attachments/assets/ed609465-28da-46e1-9227-b6d983806701)

---
## 📌 Vu général du Projet 

Ce dashboard offre une lecture complète de la chaîne de valeur du cacao en Côte d’Ivoire, depuis la production jusqu’à l’exportation, en mettant en évidence les leviers de performance, les inefficacités et les opportunités de création de valeur.

Le challenge place les participants dans le rôle d'analyste de données relatives à la chaine de valeur du Cacao en Côte d’Ivoire.


Le développement de ce projet était animé par le souci d' (d):

    o	Analyser la production de cacao par produit, ferme et coopérative ;
    
    o   Suivre les indicateurs de qualité (humidité, pertes) ;
    
    o	Évaluer la performance logistique (transport et stockage) ;
    
    o	Mesurer la performance financière (prix, valeur nette, marges) ;
    
    o	Visualiser les flux d’exportation via les ports; 


Les données d'analyse sont organisées en 10 tables dont 9 dimensions et une de faits (Fact_Mouvements). Il s'agit entre autres des dimensions: Produits, Lot, Coopérative, Ferme, Evenements, Sites, Transporteurs, Ports et Devises. 

Pour développer des fonctions temporelles intelligences, la table date a été également créée ainsi que 3 autres tables permettant de capter l'impact de la variation de certains paramétres sur les indicateurs de performance de la chaine de valeur du Cacao. Tel est le cas de table sur la variation du prix, du taux de change et de la surface cultivée.


## 🧹Processus ETL

Le processus ETL a consisté principalement au Nettoyage, transformation et importation des données (OLAP).

Le nettoyage en soit, a était l'étape crucial où nous avions effectuer les activités suivantes :


    o	Identification les doublons et leur suppression ;
    
    o   Identification des devises incohérentes et leur standardisation ;
    
    o	Identifications les valeurs négatives (poids/sacs) et harmonisation ;
    
    o	Correction des montants incohérents (remplacement de certains séparteurs comme "." par "," ;

    o	Identification /ajout de clés étrangères manquantes non existantes afin de faciliter la liason entre tables
        (Ex: Création de la Produit ID dans Dim_Lot);
    
    o	Suppression des clés étrangères hors plage (Ex: port ID de 11,6 alors que les identifications sont 1 et 2);

    o	Standardisation du format de dates en évitant de formats était mixtes (2002/01/20 ; 20-01-2002, etc. au sein
        d'une mm colonne);

    o	Normalisation de valeurs textuelles pour palier au problème d'incohérences d’accents/casse (Ex: Nom de région 
        au départ non standardisés) ;

    o	Suppression des duplicats dans la dimension producteurs pour assurer l'uniquité des données ;

    o	Conversion de format de variable vers leur forme canonique (du format textuel vers le numérique et vis-versa au 
        cas échéant).

    o	Fusion de certaines dimensions en une dimension unique: tel est le cas de la dimension Lot, Produit, Ferme &
        Coopération tout en supprimant les colonnes rédondantes ;

    o	Suppression des espaces blancs unitules.

Après s'etre rassuré que les données sont déjà  de qualité et donc préparées suffisament pour l'analyse, la modelisation a été un pond crucial afin d'établir des relations et rendre l'extraction de l'information pertinente possible.

##### 🏗 Modelisation en Etoile

<img width="699" height="498" alt="image" src="https://github.com/user-attachments/assets/b4682f96-eaf3-4873-85ef-5f43812bf9aa" />

---

## 📅📊 Tableau de Bord Interactif développé 


![ezgif com-speed](https://github.com/user-attachments/assets/d0d233d8-c9d1-42b1-b3c9-9f4bfff472e6)

---

## 🔎 Résultats des analyses 


Production totale : 290.7K tonnes
Forte contribution de certaines zones (ex : Lacs)
Chiffre d’affaires : 41.06T FCFA
Marge bénéficiaire : 4.9% #Faible
Coût logistique/tonne : 3.2K FCFA #Trop eleve
Activité la plus coûteuse : Export (~13K)
Taux de perte : 1.77%
Humidité moyenne : 7.5%
Produits premium génèrent le plus de revenus
Certification = impact positif sur CA
Flux dominants :
Coop → Centre collecte → Transport → Port
Transport dominant : Camion + Rail
---

## Recommendations

---
# 🛠 Outils et Compétences demontrées

    o	Power BI ; 	
    
    o	Power Query ;
    
    o	Nettoyage et Standardisation de données brutes ;
    
    o	Transformation de données brutes en données exploitable ;
    
    o   Modalisation de données ;
    
    o	Création de la Table Date ainsi que les tables captant la variation de certains paramètres macroéconomiques ;
    
    o	Intelligence Temporelle ;
    
    o	Design du Dashboard clair et attrayant ;
    
    o	Analyse Géographique et de la Chaine Logistique.
    
---

## 🏆 Details par rapport au Challenge


    o	Organisateur : Tresor ADOSSI

    o	Thème: Challenge Power-BI Chaine d'Approvisionnement Cacao (Côte d’Ivoire)

    o	Durée:   du 01 mars au 05 Avril 2026 

---

[![Power BI Dashboard](https://img.shields.io/badge/Cliquez_ici_pour_acceder_au_tableau_de_bord_interactif-F2C811?style=for-the-badge&logo=microsoftpowerbi&logoColor=black)](https://app.powerbi.com/view?r=eyJrIjoiYjYxOWFiMTAtMzdiNS00YTA2LTlkODUtYmZkNmIzZGRiYjRjIiwidCI6Ijk0MWJiZjVmLWYyYzAtNDg3NS1hMjRjLTY5MDc4NjVkMjUxYSIsImMiOjh9)


## 🔗 Pour tout contact de collaboration ou parténariat

N'hésitez pas à me contacter sur :

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/koko-mukuru-yves-98621a14a) 
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:kokomukuruy@gmail.com)

---
<p align="center">
  <i>"Transformation des données brutes en informations pertitentes, pour la meuilleure prise des décisions stratégiques éclairées."</i>

</p>

**© 2026 Koko Mukuru Yves**. Tout droit reservés
