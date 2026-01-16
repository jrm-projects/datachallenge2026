# Axe 2 :

Je traite le sujet de la façon suivante :

1) Je fais un document qui relie la matière et le composant du dispositif médical.
Pour ça il faut :
    - Aller sur le site [The Shift Project](https://theshiftproject.org/publications/decarbonons-industries-sante-medicaments-dm/)
    - Télécharger le fichier **Outil_de_calcul_DM_2025.xlsx** disponible sur le lien [L’outil de calcul des dispositif médicaux](https://theshiftproject.org/app/uploads/2025/11/Outil_de_calcul_DM_2025.xlsx)
    - Faire une table liant les matières (partie gauche du diagramme de flux) et les composants de dispositifs médicaux (partie droite du diagramme de flux)

2) Utiliser un modèle de NLP pour associer chaque dispositif médical de la base **DISPOSITIFS_MEDS.xlsx** à un composant de dispositifs médical (ou une combinaison pondérées par la prévision du modèle)
    - Je fait un modèle de NLP qui associe un dispositif médical de ma base **DISPOSITIFS_MEDS.xlsx** (faire des choix sur les données d'entrées) à une répartition de composants de dispositifs médical (pondérer la composition par la prévision ?)
    ATTENTION : bien ouvrir les entrelignes pour voir les bdd.
    - On calcul selon les données carbonnes (calcul déterministe)

    - Idées de modèles : TinyBERT, SLM etc.

3) Version direct avec une API chatGPT qui ajoute un détaille de la composition (+ n colonnes avec n le nb max de labels utilisés dans les compostions). Il ajoute par ligne la décomposition et après je fais le traitement

4) Evaluation et choix de l'empreinte carbone
