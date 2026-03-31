# Analyse-de-la-chaine-de-valeur-du-cacao-en-Cote-d'Ivoire-Power-BI-Challenge-Mars-2026
<img width="213" height="206" alt="image" src="https://github.com/user-attachments/assets/c867626e-319e-4c38-ba34-2e7c127a4ec6" />
<img width="213" height="206" alt="image" src="https://github.com/user-attachments/assets/37ab856c-75d7-4fe6-b9c6-03c937c62a47" />
<img width="213" height="206" alt="image" src="https://github.com/user-attachments/assets/72cde0c0-ae08-4423-8e28-d11637c3f806" />
<img width="213" height="206" alt="image" src="https://github.com/user-attachments/assets/79d41534-7d69-4768-a2ab-e67e23bb38ac" />
<img width="213" height="206" alt="image" src="https://github.com/user-attachments/assets/8a5df154-880c-4fb8-bed5-f4a0e9a4d121" />
<img width="213" height="206" alt="image" src="https://github.com/user-attachments/assets/e35c3c07-c3a0-4816-ab14-04b3303920a0" />
<img width="213" height="204" alt="image" src="https://github.com/user-attachments/assets/bc42999c-bd8b-446f-b9a1-de79b5b50224" />


<img width="206" height="262" alt="image" src="https://github.com/user-attachments/assets/070595a0-d454-4082-88ae-496284c1d495" />
<img width="209" height="267" alt="image" src="https://github.com/user-attachments/assets/06529dfa-1907-4035-9fba-f5ca6ba41546" />

<img width="215" height="209" alt="image" src="https://github.com/user-attachments/assets/c6201dcf-0c90-487f-8886-77ee3f8a0647" />



Projet réalisé dans le cadre d’un challenge en data analytics, portant sur la chaîne de valeur du cacao en Côte d’Ivoire. Il consiste à développer un dashboard Power BI interactif pour analyser la supply chain, de la production à l’export, et générer des insights sur la performance, la qualité et la logistique.



<details>
<summary id="introduction"> Introduction</summary>

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


## Vue d'ensemble
<img width="881" height="497" alt="Screenshot 2026-03-30 164614" src="https://github.com/user-attachments/assets/7e4f840a-2bf1-4c67-8f41-f1d1804d49a5" />

## Analyse du Flux du Cacao
<img width="879" height="495" alt="Screenshot 2026-03-30 164801" src="https://github.com/user-attachments/assets/919d5d69-4857-48a5-90af-4389b59e4858" />

## Analyse de la Performance
<img width="871" height="486" alt="Screenshot 2026-03-30 175536" src="https://github.com/user-attachments/assets/c07283bf-0ff1-4f3a-ac07-9a55499acae9" />

## Analyse de la tendance dans le temps

<img width="879" height="497" alt="Screenshot 2026-03-30 164854" src="https://github.com/user-attachments/assets/8ff52535-6723-4f8e-84ed-13d9f0d5fe59" />

## Analyse Geographique
<img width="880" height="496" alt="Screenshot 2026-03-30 165026" src="https://github.com/user-attachments/assets/f6966fab-ffb3-46e7-b44c-167afd128dd9" />

## Ports et Exports

<img width="874" height="492" alt="image" src="https://github.com/user-attachments/assets/86e7f8de-0463-45e9-b3e8-32a2bb0c9b97" />

## Impact de la Variation de certains parametres

<img width="875" height="495" alt="Screenshot 2026-03-30 165200" src="https://github.com/user-attachments/assets/858e33b2-c829-4842-8862-312f73e7a9d1" />


</details>

---
<details>

<summary id="results--insights"> Results / Insights</summary>





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

[![Power BI Dashboard](https://img.shields.io/badge/Click_here_to_access_the_interactive_dashboard-F2C811?style=for-the-badge&logo=microsoftpowerbi&logoColor=black)](https://app.powerbi.com/view?r=eyJrIjoiZDU0YTIwNTEtN2VjMi00NjA5LWJkOTgtOTI2MGQwMDIyY2RmIiwidCI6Ijk0MWJiZjVmLWYyYzAtNDg3NS1hMjRjLTY5MDc4NjVkMjUxYSIsImMiOjh9)




## 🔗 Connect with me

For questions or collaborations, feel free to reach out!

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/koko-mukuru-yves-98621a14a) 
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:kokomukuruy@gmail.com)

---
<p align="center">
  <i>"Turning data into actionable insights, one project at a time."</i>
</p>

**© 2026 Koko Mukuru Yves**. All rights reserved
