# Analyse-de-la-chaine-de-valeur-du-cacao-en-Cote-d'Ivoire-Power-BI-Challenge-Mars-2026

![ezgif com-speed(4)](https://github.com/user-attachments/assets/ed609465-28da-46e1-9227-b6d983806701)

---
## Vu général du Projet 

Ce dashboard offre une lecture complète de la chaîne de valeur du cacao en Côte d’Ivoire, depuis la production jusqu’à l’exportation, en mettant en évidence les leviers de performance, les inefficacités et les opportunités de création de valeur.

Le challenge place les participants dans le rôle d'analyste de données relatives à la chaine de valeur du Cacao en Côte d’Ivoire.

Les données sont organisées en 10 tables dont 9 dimensions et une de faits (Fact_Mouvements). Il s'agit entre autres des dimensions: Produits, Lot, Coopérative, Ferme, Evenements, Sites, Transporteurs, Ports et Devises. 

Pour développer des fonctions temporelles intelligences, la table date a été également créée ainsi que 3 autres tables permettant de capter l'impact de la variation de certains paramétres sur les indicateurs de performance de la chaine de valeur du Cacao. Tel est le cas de table sur la variation du prix, du taux de change et de la surface cultivée.

Le développement de ce projet était animé par le souci d' (d):

-  Analyser la production de cacao par produit, ferme et coopérative ;
- Suivre les indicateurs de qualité (humidité, pertes) ;
- Évaluer la performance logistique (transport et stockage) ;
- Mesurer la performance financière (prix, valeur nette, marges) ;
- Visualiser les flux d’exportation via les ports; 


## Processus ETL

Le processus ETL a consisté principalement au Nettoyage, transformation et importation des données (OLAP).

Le nettoyage en soit, a était l'étape crucial où nous avions effectuer les activités suivantes :

- Identifier les doublons et leur suppression.
- Identifier des devises incohérentes et leur standardisation ;
- Identifier les valeurs négatives (poids/sacs) et les adresser ;
- Corriger les montants incohérents (supprimer le "." et le remplacer par la ",";
- Identifier/ajouter de clés étrangères manquantes non existante afin de faciliter la liason entre tables (Ex: Création de la Produit ID dans 
   Dim_Lot;
- Supprimer les clés étrangères hors plage ;
- Standardiser le format de dates car au départ le format était mixtes (2002/01/20 ; 20-01-2002, etc.).
- Normalisation de valeurs textuelles pour palier au problè d'incohérences d’accents/casse (Ex: Nom de région au départ non standardisés) ;
- Supprimer les duplicats dans la dimension producteurs pour assurer l'uniquité des données.
- Convertir le format de variable vers leur forme canonique (du format textuel vers le numérique et vis-versa au cas échéant).
- Fusionner certaines dimensions en une dimension unique: tel est le cas de la dimension Lot, Produit, Ferme & Coopération tout en supprimant les colonnes rédondantes ;
- Suppression des espaces blancs unitules.

#Modelisation en Etoile

<img width="699" height="498" alt="image" src="https://github.com/user-attachments/assets/b4682f96-eaf3-4873-85ef-5f43812bf9aa" />


</details>

---

<details>
<summary id="etl-process"> ETL Process</summary>


The analysis followed a structured **ETL pipeline**:


### 1. Data Extraction


  

### 2. Data Cleaning

* Handled missing values 
* Filled non-critical missing values (`Payment_Type` & 'Location') with default values (e.g. 'Unknown').
* Corrected inconsistent values (e.g., negative ages, impossible timestamps in `Time_In`/`Time_Out`).
* Standardized categorical values (`Gender`: Male/Female, `Payment_Type`: Private/Insurance/Other).


### 3. Data Transformation

* Created additional calculated columns: Age_Group, Cohort_Month, First_Visit_Date, Hospital_Rush.

* Create measures and KPIs: Average Age, Average Days Between Visits, Average Visits per Day, New Patient Acquisition Rate, Total Patients, Retention Rate & Peak Hours/Hospital Rush.

* Built supporting tables for temporal and demographic analysis (Daily Visits, Monthly Cohorts, Payment Trends).


</details>

---
<details>

<summary id="dashboard-overview">Dashboard Overview</summary>

![ezgif com-added-text](https://github.com/user-attachments/assets/79333dc0-a9fd-40d6-b65d-81856ae2abf5)


</details>

---
<details>

<summary id="results--insights"> Results / Insights</summary>



![ezgif com-speed](https://github.com/user-attachments/assets/d0d233d8-c9d1-42b1-b3c9-9f4bfff472e6)


### **The Story of Our Hospital’s Patient Flow and Performance**


</details>
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
<details>



<summary id="recommendations"> Recommendations</summary>



</details>

---

## 🏆 Details par rapport au Challenge

Organisateur : Tresor ADOSSI

Theme: Challenge Power-BI Chaine d'Approvisionnement Cacao (Cote d'Ivoire)

Mini Challenge du 01 mars au 05 Avril 2026 

---

[![Power BI Dashboard](https://img.shields.io/badge/Cliquez_ici_pour_acceder_au_tableau_de_bord_interactif-F2C811?style=for-the-badge&logo=microsoftpowerbi&logoColor=black)](https://app.powerbi.com/view?r=eyJrIjoiYjYxOWFiMTAtMzdiNS00YTA2LTlkODUtYmZkNmIzZGRiYjRjIiwidCI6Ijk0MWJiZjVmLWYyYzAtNDg3NS1hMjRjLTY5MDc4NjVkMjUxYSIsImMiOjh9)


## 🔗 Connect with me

For questions or collaborations, feel free to reach out!

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/koko-mukuru-yves-98621a14a) 
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:kokomukuruy@gmail.com)

---
<p align="center">
  <i>"Turning data into actionable insights, one project at a time."</i>
</p>

**© 2026 Koko Mukuru Yves**. All rights reserved
