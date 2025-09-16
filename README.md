<div align="center">
  
# Analyser l'efficacité des campagnes d'emailing

</div>

Ce projet propose une analyse des performances de campagnes d’emailing (taux d’ouverture, clics, conversions) en utilisant **Python** et **Power BI**, afin d’identifier les meilleures fenêtres temporelles pour maximiser l’impact marketing.  

---

## Données
- **Source** : [Kaggle - Email Marketing Campaign Dashboard](https://www.kaggle.com/datasets/mariusnikiforovas/email-marketing-campaign-dashboard?select=filtered_dataset.csv)  
- **Champs principaux** :
  - Informations clients (nom, numéro de compte)
  - Campagnes distinctes
  - Dates d’envoi, rebond, ouverture, clic, achat, etc.
  - Montants des achats réalisés  

---

## Préparation des données
- **Filtrage des emails non délivrés** : suppression des cas de rebond.  
- **Normalisation des campagnes** : renommage pour une meilleure lisibilité analytique.  
- **Colonnes indicatrices (booléennes)** : génération automatique pour les actions clés (ouverture, clic, achat).  
- **Segmentation horaire** : découpage en plages stratégiques pour l’identification des heures les plus performantes :
  - 6h-9h : Petit matin  
  - 9h-12h : Matin  
  - 12h-14h : Midi  
  - 14h-18h : Après-midi  
  - 18h-21h : Soir  
  - 21h-00h : Fin de soirée  
  - 00h-6h : Nuit  

---

## Visualisations
- Nombre et pourcentage d'ouvertures par campagne  
![](https://github.com/FabienHaury/Analyser-l-efficacite-des-campagnes-d-emailing/blob/main/Python/Screenshot/Graphiques/graph_campagne_open.png)

- Tableau récapitulatif des KPI par campagne et par mois  
![](https://github.com/FabienHaury/Analyser-l-efficacite-des-campagnes-d-emailing/blob/main/Python/Screenshot/Tableaux/tab_summary_annee_mois.png)

- Heatmap des ouvertures par jour de la semaine et campagne  
![](https://github.com/FabienHaury/Analyser-l-efficacite-des-campagnes-d-emailing/blob/main/Python/Screenshot/Graphiques/graph_nombre_ouvertures_par_campagne_et_jour.png)

- Répartition des ouvertures par plage horaire (exemple campagne 4, mai 2021/2022)  
![](https://github.com/FabienHaury/Analyser-l-efficacite-des-campagnes-d-emailing/blob/main/Python/Screenshot/Tableaux/tab_ann%C3%A9e_mois_jour_seg.png)

---

## Résultats
- Taux de rebond très faible : **1,5% en moyenne**, signe d’une excellente qualité de la base emails.  
- Taux d’ouverture élevé : entre **76,9% et 87,7%** selon les campagnes.  
- Taux de clics hétérogène : de **8,4%** (campagne 3) jusqu’à **28,3%** (campagne 2).  
- Taux de transaction proportionnel aux clics : meilleure performance pour la campagne 2 (**3,8%**), plus faible pour la campagne 4 (**0,7%**).  
- La campagne 2 génère le plus de revenus (**531 259 $**, soit près de **60% du total**).  
- Aucun jour de la semaine ne montre systématiquement un meilleur taux d’ouverture.  
- Les heures de **nuit (00h-6h)** concentrent la majorité des ouvertures.  

---

## Suggestions
- Collecter plus d’informations sur les causes réelles des rebonds (adresses invalides, serveurs inaccessibles…).  
- Étudier le **contenu des emails** (non disponible ici) pour comprendre le succès de la campagne 2.  
- Optimiser les envois autour des plages **00h-6h**, qui montrent les meilleures performances d’ouverture.  

---

## Outils
- **Python** : Pandas, Numpy, Seaborn (préparation, nettoyage, segmentation, premières analyses visuelles).  
- **Power BI** : dashboards interactifs, analyses temporelles détaillées, KPIs dynamiques.  

---

## Contact
- 📧 [Email](mailto:67912775+FabienHaury@users.noreply.github.com)  
- 💼 [LinkedIn](https://www.linkedin.com/in/fabienhaury/)
