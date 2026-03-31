# Analyse-de-la-chaine-de-valeur-du-cacao-en-Cote-d'Ivoire-Power-BI-Challenge-Mars-2026

![ezgif com-speed(4)](https://github.com/user-attachments/assets/ed609465-28da-46e1-9227-b6d983806701)

---

<details>
<summary id="introduction"> Introduction</summary>

🎯 Objectifs
* Analyser la production de cacao par produit, ferme et coopérative ;
* Suivre les indicateurs de qualité (humidité, pertes)
* Évaluer la performance logistique (transport et stockage)
* Mesurer la performance financière (prix, valeur nette, marges)
* Visualiser les flux d’exportation via les ports

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

[![Power BI Dashboard](https://img.shields.io/badge/Cliquez_ici_pour_acceder_au_tableau_de_bord_interactif-F2C811?style=for-the-badge&logo=microsoftpowerbi&logoColor=black)](<iframe title="Koko_Mukuru_Yves_Challenge_Chaine_Logistique_cacao_CI_Mars 2026" width="600" height="373.5" src="https://app.powerbi.com/view?r=eyJrIjoiYjYxOWFiMTAtMzdiNS00YTA2LTlkODUtYmZkNmIzZGRiYjRjIiwidCI6Ijk0MWJiZjVmLWYyYzAtNDg3NS1hMjRjLTY5MDc4NjVkMjUxYSIsImMiOjh9" frameborder="0" allowFullScreen="true"></iframe>)


## 🔗 Connect with me

For questions or collaborations, feel free to reach out!

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/koko-mukuru-yves-98621a14a) 
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:kokomukuruy@gmail.com)

---
<p align="center">
  <i>"Turning data into actionable insights, one project at a time."</i>
</p>

**© 2026 Koko Mukuru Yves**. All rights reserved
