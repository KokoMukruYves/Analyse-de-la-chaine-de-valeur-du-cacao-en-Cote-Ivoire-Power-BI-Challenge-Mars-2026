Challenge Power BI – Chaîne d’approvisionnement cacao (Côte d’Ivoire)
Données synthétiques (CSV) avec ~150K+ mouvements et problèmes de qualité intentionnels.

Tables : fact_Mouvements, dim_Lot, dim_Ferme, dim_Cooperative, dim_Site, dim_Transporteur, dim_Port, dim_Produit, dim_Devise, dim_Evenement.
Pas de dim_Date : les participants doivent générer leur propre calendrier et faire les relations via date_cle.
Problèmes injectés : doublons, devises ‘XO F’, poids/sacs négatifs, montants incohérents, FK manquantes, IDs hors plage, incohérences d’accents/casse, doublons producteurs, dates texte mixtes.
Idées : unifier devise→XOF, nettoyer dates, valider montants, traiter doublons, calculer pertes, humidité moyenne, coûts, export par port/campagne/grade/varieté, paiements et primes.