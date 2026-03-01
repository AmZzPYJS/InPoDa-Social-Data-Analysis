📌 Contexte du projet

Ce projet a été réalisé dans le cadre du TD 11–12 (LSIN304) à l’Université de Versailles Saint-Quentin-en-Yvelines.

L’objectif était de concevoir une plateforme fictive nommée InPoDa, dédiée à la collecte, au traitement et à l’analyse de données issues des réseaux sociaux (tweets au format JSON).

Le projet simule une architecture simplifiée de pipeline data :
    1.    Collecte des publications
    2.    Nettoyage et validation des données
    3.    Traitement et enrichissement
    4.    Analyse statistique
    5.    Visualisation des résultats

⸻

🏗 Architecture générale

Le système fonctionne selon les étapes suivantes :
    •    Lecture d’un fichier JSON contenant des publications
    •    Validation et nettoyage des données (expressions régulières)
    •    Modélisation des tweets sous forme de dictionnaires Python
    •    Encapsulation des traitements via la programmation orientée objet
    •    Stockage intermédiaire dans une “zone d’atterrissage”
    •    Enrichissement des données (sentiment, topics, hashtags…)
    •    Chargement dans une structure type DataFrame pour analyse

⸻

🧱 Modélisation des données

Chaque tweet est représenté sous forme de dictionnaire structuré :

```
{
    "auteur": "...",
    "contenu": "...",
    "hashtags": [...],
    "mentions": [...],
    "sentiment": "...",
    "topics": [...]
}
```

La modélisation a été adaptée pour faciliter les opérations analytiques demandées.

⸻

⚙️ Fonctionnalités implémentées

🔍 Traitement des données
    •    Identification de l’auteur
    •    Extraction des hashtags
    •    Extraction des utilisateurs mentionnés
    •    Analyse de sentiment (TextBlob)
    •    Identification des topics

📈 Analyse des données
    •    Top K hashtags
    •    Top K utilisateurs
    •    Top K utilisateurs mentionnés
    •    Top K topics
    •    Nombre de publications par utilisateur
    •    Nombre de publications par hashtag
    •    Nombre de publications par topic
    •    Tweets d’un utilisateur spécifique
    •    Tweets mentionnant un utilisateur spécifique

⸻

🧪 Technologies utilisées
    •    Python
    •    Programmation Orientée Objet (POO)
    •    Expressions régulières (re)
    •    TextBlob (analyse de sentiment)
    •    Matplotlib (visualisation)
    •    Pandas (analyse tabulaire si utilisé)
    •    Jupyter Notebook

⸻

📊 Visualisation

Les résultats analytiques sont représentés graphiquement à l’aide de matplotlib, permettant :
    •    Visualisation des Top K
    •    Histogrammes de fréquence
    •    Répartition des sentiments

⸻

🎓 Objectifs pédagogiques
    •    Compréhension d’un pipeline de traitement de données
    •    Manipulation de données JSON
    •    Structuration via POO
    •    Nettoyage via regex
    •    Analyse statistique
    •    Visualisation de données

⸻

🚀 Perspectives d’amélioration
    •    Intégration d’un stockage base de données
    •    API REST pour déclencher les traitements
    •    Automatisation du pipeline
    •    Déploiement cloud
    •    Analyse NLP plus avancée
