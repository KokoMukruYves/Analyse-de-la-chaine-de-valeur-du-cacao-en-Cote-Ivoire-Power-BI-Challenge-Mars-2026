# Analyse-de-la-chaine-de-valeur-du-cacao-en-Cote-d'Ivoire-Power-BI-Challenge-Mars-2026

![ezgif com-speed(4)](https://github.com/user-attachments/assets/ed609465-28da-46e1-9227-b6d983806701)

---
## 📌 I.  Vu général du Projet 

Ce dashboard offre une lecture complète de la chaîne de valeur du cacao en Côte d’Ivoire, depuis la production jusqu’à l’exportation, en mettant en évidence les leviers de performance, les inefficacités et les opportunités de création de valeur.

Le challenge place les participants dans le rôle d'analyste de données relatives à la chaine de valeur du Cacao en Côte d’Ivoire.


Le développement de ce projet était animé par le souci d' (d):

    o	Analyser la production de cacao par produit, ferme et coopérative ;
    
    o   Suivre les indicateurs de qualité (humidité, pertes) ;
    
    o	Évaluer la performance logistique (transport et stockage) ;
    
    o	Mesurer la performance financière (prix, valeur nette, marges) ;
    
    o	Visualiser les flux d’exportation via les ports; 

    o   Evaluer la tendance de certains indicateurs clés dans le temps et en faire une projections futures.


Les données d'analyse sont organisées en 10 tables dont 9 dimensions et une de faits (Fact_Mouvements). Il s'agit entre autres des dimensions: Produits, Lot, Coopérative, Ferme, Evenements, Sites, Transporteurs, Ports et Devises. 

Pour développer des fonctions temporelles intelligentes, la Table Date a été également créée ainsi que 3 autres tables permettant de capter l'impact de la variation de certains paramètres sur les indicateurs de performance de la chaine de valeur du Cacao. Tel est le cas de table sur la variation du prix, du taux de change et de la surface cultivée.


## 🧹II. Processus ETL

Le processus ETL a consisté principalement au Nettoyage, transformation et importation des données.

Le nettoyage en soit, a été l'étape cruciale où nous avions effectué les activités suivantes :


    o	Identification les doublons et leur suppression ;
    
    o   Identification des devises incohérentes et leur standardisation ;
    
    o	Identifications les valeurs négatives (poids/sacs) et harmonisation ;
    
    o	Correction des montants incohérents (remplacement de certains séparteurs comme "." par "," ;

    o	Identification /ajout de clés étrangères manquantes non existantes afin de faciliter la liason entre tables
        (Ex: Création de la Produit ID dans Dim_Lot);
    
    o	Suppression des clés étrangères hors plage (Ex: port ID de 11,6 alors que les identifications sont 1 et 2);

    o	Standardisation du format de dates en évitant de formats mixtes (2002/01/20 ; 20-01-2002, etc. au sein
        d'une même colonne);

    o	Normalisation de valeurs textuelles pour palier au problème d'incohérences d’accents/casse (Ex: Noms de région 
        au départ non standardisés) ; 
        
    o	Renommer certaines colonnes pour plus de lisibilité et clarté ;

    o	Suppression des duplicats dans la dimension producteurs pour assurer l'uniquité des données ;

    o	Conversion de format de variable vers leur forme canonique (du format textuel vers le numérique et vis-versa au 
        cas échéant).

    o	Fusion de certaines dimensions en une dimension unique: tel est le cas de la dimension Lot, Produit, Ferme &
        Coopération tout en supprimant les colonnes rédondantes ;

    o	Suppression des espaces blancs unitules.

Après s'etre rassuré que les données sont déjà  de qualité et donc préparées suffisament pour l'analyse, la modelisation a été un pond crucial afin d'établir des relations et rendre l'extraction de l'information pertinente possible.

##### 🏗 Modelisation en Etoile

<img width="699" height="498" alt="image" src="https://github.com/user-attachments/assets/b4682f96-eaf3-4873-85ef-5f43812bf9aa" />


##  🧮 III. Mesures clés
Pour performer les analyses, plusieurs mesures ont été calculées, il s'agit entre autres:
   
    o  Volume Total de Production ;
    
    o  Marge Bénéficiaire totale ;
    
    o  Cout Logistique (Transport et Stockage) ;
    
    o  Age Moyen de la ferme et de la Coopérative ;
    
    o  Volume Export ;   
    
    o  Humidité Moyenne ;
    
    o  Taux de Perte ;
    
    o  Target Humidité, Rendement ;
    
    o  Total Mouvements ;
    
    o  Total Sac ; 
    
    o  YOY ;
    
    o  Etc.


## 📅📊 IV.  Tableau de Bord Interactif développé 


![ezgif com-speed](https://github.com/user-attachments/assets/d0d233d8-c9d1-42b1-b3c9-9f4bfff472e6)


## 🔎 V. Synthèse analytiques de la chaîne de valeur du Cocoa en Côte d'Ivoire

| Section | KPI / Thème | Constat / Insight | Recommandation stratégique |
|---------|-------------|-------------------|---------------------------|
| **📈 Performance commerciale** | Chiffre d'affaires | Évolution positive mais marquée par une saisonnalité forte (campagnes 2023/24 → 2025/26 : 10,2M → 14,0M tonnes export) | Renforcer la planification des stocks pour lisser les pics de campagne et maximiser les opportunités de prix |
| | Marge bénéficiaire nette | 4,9% (faible) malgré un CA élevé, avec une marge en légère hausse pour les produits premium | Poursuivre la montée en gamme et la certification pour améliorer la rentabilité |
| **🚛🚚 Logistique & coûts** | Coût logistique/tonne | 3,2K FCFA, avec des pics à 13K FCFA pour l'export | Optimiser les trajets et réduire la dépendance aux sous-traitants peu performants |
| | Flux dominant | Coop → Centre collecte → Transport → Port (camion + rail prédominant) | Fluidifier les interfaces entre étapes pour réduire les pertes et délais |
| **💧 Qualité & pertes** | Taux de perte moyen | 1,77%, concentré sur transport et stockage | Cibler les goulots critiques avec des audits et formations |
| | Humidité moyenne | 7,5%, avec zones > 8% entraînant des risques de rejet à l'import | Renforcer le séchage post-récolte et former les producteurs |
| **🏭 Certification & valeur** | Impact certification | Lots certifiés → valeur nette supérieure (primes) ; export certifié : 21,82M vs non certifié 19,39M tonnes | Accélérer la certification des coopératives pour augmenter la valeur ajoutée |
| **🌱 Concentration production** | Volume production | 290,7K tonnes, fortement concentrée (ex : Lacs, coopératives #88, #16, #102) | Diversifier la base producteurs pour réduire la vulnérabilité |
| | Top fermes | Abdou Assé (8105, 11218, 11439) domine en volume | Éviter la dépendance excessive à quelques producteurs clés |
| **⚖️ Rentabilité & prix** | Prix moyen | Varie selon qualité, humidité, certification, grade ; premium génère plus de revenus (ex : produit ID 2 : +4,79% marge) | Favoriser les segments premium et valoriser la traçabilité qualité/prix |
| **📦 Export & 🚢ports** | Volume export | Port de San-Pédro : 41,2M tonnes ; Port d'Abidjan : 20,29M tonnes | Équilibrer les flux entre ports pour réduire les congestions et optimiser les coûts |
| | Valeur nette export | San-Pédro : 15,32T FCFA ; Abidjan : 14,76T FCFA | San-Pédro plus performant en valeur → analyser et reproduire les bonnes pratiques |
| **📅 Dynamique temporelle** | Saisonnalité | Forte concentration des volumes sur les campagnes, avec fluctuations importantes | Mettre en place un stockage tampon et une gestion prévisionnelle des ressources |
| | Évolution du nombre de fermes | Croissance régulière (~4400 fermes sur la période) | Accompagner cette croissance par des programmes de formation et de certification |
| **📊 Projections & sensibilité** | Impact variation prix | Variation prix → impact direct sur CA | Mettre en place des outils de couverture ou de contrat long terme pour stabiliser les revenus |
| | Impact taux de change | Fluctuation impacte la valeur nette export | Intégrer une gestion active du risque de change |
| | Surface cultivée vs production | Corrélation positive : +0,29 variation surface → hausse production | Encourager l'expansion contrôlée avec des pratiques durables |

## 🛠 VI. Outils et Compétences demontrées

    o	Power BI ; 	
    
    o	Power Query ;
      
    o	Transformation de données brutes en données exploitable ;
    
    o   Modalisation de données ;
    
    o	Création de la Table Date (Time Intelligence) ainsi que les tables captant la variation de certains paramètres macroéconomiques ;
    
    o	Design du Dashboard clair et attrayant ;
    
    o	Visualisations interactives avec ZoomCharts
    
    o	Analyse Géographique et de la Chaine Logistique.
    
## 🎯 VII. Conclusion

Ce projet démontre comment un nettoyage, une transformation et une modélisation structurés des données permettent de convertir des jeux de données bruts en insights analytiques pertinents.

Le tableau de bord offre une vue claire et structurée de la chaîne d’approvisionnement du cacao ainsi que de son évolution selon les événements, les modes de transport, les périodes et les régions géographiques en Côte d’Ivoire.


## 🏆 VIII. Details par rapport au Challenge


    o	Organisateur : Trésor ADOSSI

    o	Thème: Challenge Power-BI Chaine d'Approvisionnement Cacao (Côte d’Ivoire)

    o	Durée:   du 01 mars au 05 Avril 2026 

---

[![Power BI Dashboard](https://img.shields.io/badge/Cliquez_ici_pour_acceder_au_tableau_de_bord_interactif-F2C811?style=for-the-badge&logo=microsoftpowerbi&logoColor=black)](https://app.powerbi.com/view?r=eyJrIjoiYjYxOWFiMTAtMzdiNS00YTA2LTlkODUtYmZkNmIzZGRiYjRjIiwidCI6Ijk0MWJiZjVmLWYyYzAtNDg3NS1hMjRjLTY5MDc4NjVkMjUxYSIsImMiOjh9)


## 🔗 Pour tout contact de collaboration ou parténariat

N'hésitez pas de me contacter sur :

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/koko-mukuru-yves-98621a14a) 
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:kokomukuruy@gmail.com)

---
<p align="center">
  <i>"Transformation des données brutes en informations pertitentes, pour la meuilleure prise des décisions stratégiques éclairées."</i>

</p>

**© 2026 Koko Mukuru Yves**. Tout droit reservés
