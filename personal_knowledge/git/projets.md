# Projets

## Agent LinkedIn : Génération des postes pour Linkedin 

Cet agent intelligent automatise la création de posts LinkedIn en utilisant l'IA pour générer du contenu pertinent et engageant. Il utilise plusieurs modèles d'IA (OpenAI, Groq, et Gemini) pour générer des posts de qualité.

## Fonctionnalités

- 🔐 Authentification sécurisée avec LinkedIn
- 🔍 Analyse des publications récentes basée sur un thème
- 🧠 Suggestions de sujets personnalisés
- ✍️ Génération de posts avec différents modèles d'IA :
  - OpenAI (GPT-4.1-mini)
  - Groq (Llama-3.3-70b-versatile)
  - Google Gemini (Gemini-2.0-flash)

## Prérequis

- Python 3.8 ou supérieur
- Compte LinkedIn
- Clés API pour :
  - OpenAI
  - Groq
  - Google Gemini

## Installation

1. Clonez ce dépôt :
```bash
git clone [URL_DU_REPO]
cd [NOM_DU_DOSSIER]
```

2. Installez les dépendances :
```bash
pip install linkedin-api
pip install openai
pip install python-dotenv
```

3. Configurez les variables d'environnement :
   - Créez un fichier `.env` à la racine du projet
   - Copiez le contenu suivant et remplissez les valeurs :
   ```
   LINKEDIN_EMAIL=your_email@example.com
   LINKEDIN_PASSWORD=your_password
   OPENAI_API_KEY=your_openai_api_key
   GROQ_API_KEY=your_groq_api_key
   GOOGLE_API_KEY=your_google_api_key
   ```

## Utilisation

1. Lancez l'agent :
```bash
python linkedin_agent.py
```

2. Suivez les instructions à l'écran pour :
   - Vous authentifier sur LinkedIn
   - Entrer un thème pour l'analyse des publications
   - Choisir parmi les suggestions de sujets générées
   - Générer des posts avec différents modèles d'IA

## Sécurité

- Ne partagez jamais votre fichier `.env`
- Ne committez pas vos identifiants dans le code
- Utilisez des mots de passe forts
- Gardez vos clés API secrètes

## Contribution

Les contributions sont les bienvenues ! N'hésitez pas à :
- Ouvrir une issue pour signaler un bug
- Proposer une pull request pour une amélioration
- Partager vos idées d'évolution

## Licence

MIT 

## Agent LinkedIn : Génération et Sauvegarde avec Google Docs

Cet agent intelligent automatise la création de posts LinkedIn en utilisant l'IA pour générer du contenu pertinent et engageant, et les sauvegarde automatiquement dans Google Docs. Il inclut également la possibilité d'une publication assistée sur LinkedIn.

## Fonctionnalités

- 🔐 Authentification sécurisée avec LinkedIn et Google
- 🔍 Analyse des publications récentes
- 🧠 Suggestions de sujets personnalisés
- ✍️ Génération de posts avec différents styles (via OpenAI, Groq, Gemini)
- 📄 Sauvegarde automatique dans Google Docs
- ✅ Publication assistée sur LinkedIn (fonctionnalité potentielle / à venir)

## Prérequis

- Python 3.8 ou supérieur
- Compte LinkedIn
- Compte Google avec accès à Google Docs
- Clés API pour OpenAI, Groq et/ou Google Gemini

## Installation

1. Clonez ce dépôt :
```bash
git clone [URL_DU_REPO]
cd [NOM_DU_DOSSIER]
```

2. Installez les dépendances :
```bash
pip install -r requirements.txt
```

3. Configurez les variables d'environnement :
   - Créez un fichier `.env` à la racine du projet
   - Copiez le contenu suivant et remplissez les valeurs :
   ```
   LINKEDIN_EMAIL=your_email@example.com
   LINKEDIN_PASSWORD=your_password
   OPENAI_API_KEY=your_openai_api_key
   GOOGLE_CLIENT_ID=your_google_client_id
   GOOGLE_CLIENT_SECRET=your_google_client_secret
   GOOGLE_API_KEY=your_google_api_key
   GROQ_API_KEY=your_groq_api_key
   ```

4. Configurez l'authentification Google :
   - Allez sur [Google Cloud Console](https://console.cloud.google.com)
   - Créez un nouveau projet
   - Activez l'API Google Docs
   - Créez des identifiants OAuth 2.0 (type "Desktop app" ou "Application de bureau")
   - Téléchargez le fichier `credentials.json` et placez-le à la racine du projet. Ce fichier contient les informations d'identification de votre application.

## Utilisation

1. Lancez l'agent :
```bash
python linkedin_agent_with_docs.py
```

2. Suivez les instructions à l'écran pour :
   - Vous authentifier
   - Choisir un sujet
   - Générer et sauvegarder les posts dans Google Docs

## Sécurité

- Ne partagez jamais votre fichier `.env`
- Ne committez pas vos identifiants dans le code
- Utilisez des mots de passe forts
- Gardez vos clés API secrètes

## Contribution

Les contributions sont les bienvenues ! N'hésitez pas à :
- Ouvrir une issue pour signaler un bug
- Proposer une pull request pour une amélioration
- Partager vos idées d'évolution

## Licence

MIT 


## Analyse économétrique des séries temporelles de rendements d’ETF : Modélisation GARCH et VAR
## Contexte et objectif du projet
Le projet s'inscrit dans un contexte financier marqué par une forte volatilité et des dynamiques complexes des marchés. Il vise à analyser les séries temporelles des rendements de trois ETF représentatifs : Amundi MSCI World UCITS ETF - EUR (CW8), Amundi MSCI India UCITS ETF - EUR (CI2) et Amundi FTSE Epra Europe Real Estate UCITS ETF - EUR (EPRE). L'objectif principal est de comprendre les caractéristiques propres à chaque ETF, d'étudier la persistance de la volatilité et les interactions entre ces actifs, et d'améliorer la capacité à anticiper les risques financiers associés. Pour cela, le projet mobilise des modèles économétriques avancés, notamment les modèles GARCH et VAR.

## Données utilisées
Les données utilisées sont les séries temporelles des rendements des trois ETF mentionnés, cotés sur Euronext Paris. Ces ETF couvrent différents marchés : actions mondiales (CW8), actions indiennes (CI2) et immobilier coté européen (EPRE). Les données incluent les valeurs historiques des prix, les rendements géométriques, ainsi que des informations sur la volatilité et la corrélation entre ces actifs. Les données proviennent de sources telles qu’Amundi.fr et Yahoo Finance.

## Méthodologie et outils
La méthodologie repose sur l’analyse économétrique des séries temporelles. Deux types de modèles sont utilisés : les modèles GARCH(1,1), GARCH multivariés (notamment le modèle BEKK) pour modéliser la volatilité conditionnelle et ses dynamiques, et les modèles Vectoriels Auto-Régressifs (VAR) pour étudier les interactions dynamiques entre les rendements des ETF. Le test de causalité de Granger est appliqué pour détecter les relations de causalité entre les séries. La sélection de l’ordre du modèle VAR est réalisée à l’aide de critères d’information (AIC, BIC, HQIC, FPE). Les outils utilisés incluent les langages Python et R.

## Principaux résultats
Les résultats montrent une forte persistance de la volatilité pour les ETF CI2 et EPRE, tandis que CW8 présente une volatilité plus stable. La corrélation conditionnelle entre les ETF est modérée et positive, avec des fluctuations dans le temps. Les tests de causalité de Granger révèlent que les valeurs passées des trois ETF ont un pouvoir prédictif significatif les unes sur les autres, justifiant l’utilisation conjointe des séries dans les modèles VAR. Les fonctions de réponse aux impulsions indiquent que les chocs ont un effet transitoire et principalement localisé sur la variable d’origine, avec une transmission limitée entre variables.

## Interprétation et implications
L’étude met en lumière la dynamique spécifique des rendements et de la volatilité des ETF, soulignant l’efficacité des modèles GARCH(1,1), GARCH et VAR pour capturer ces phénomènes. La persistance élevée de la volatilité pour certains ETF suggère un risque accru et une mémoire longue des chocs passés. La corrélation modérée entre les ETF ouvre des perspectives de diversification, bien que des phases de turbulence puissent affecter simultanément ces actifs. Ces résultats sont utiles pour optimiser les stratégies d’investissement en tenant compte des particularités de chaque ETF et des interactions entre eux.

## Compétences développées
Ce projet a permis de développer des compétences avancées en économétrie des séries temporelles, notamment dans la modélisation GARCH multivariée et les modèles VAR. Il a renforcé la maîtrise des tests statistiques comme la causalité de Granger, ainsi que l’interprétation des fonctions de réponse aux impulsions. L’utilisation pratique des langages Python et R pour l’analyse de données financières a également été approfondie, tout comme la capacité à synthétiser des résultats complexes pour des applications en finance quantitative.

 <!DOCTYPE html>
<html lang="en">
<body>
    <div class="container">
        <h1>📊 Analyse empirique des ETF (ARIMA) - Finance 2024-2025</h1>
<strong>Contexte et objectif du projet</strong>
        
Ce projet s’inscrit dans le domaine de la finance empirique et vise à analyser les propriétés statistiques et économétriques des fonds négociés en bourse (ETF). L’objectif principal est de comprendre la dynamique des rendements de plusieurs ETF, d’évaluer leurs caractéristiques statistiques, et d’appliquer des modèles économétriques pour mieux appréhender leur comportement temporel.

<strong>Données utilisées</strong>

Les données utilisées sont des séries temporelles quotidiennes des prix de trois ETF : Amundi Index MSCI Emerging Markets UCITS ETF DR (AEME.PA), Amundi MSCI Europe Growth UCITS ETF Acc (CG9.PA), et Amundi MSCI Europe Value Factor UCITS ETF-C (CV9.PA). Ces données couvrent une période allant de 2017 à fin 2024.

<strong>Méthodologie et outils</strong>

L’analyse débute par des statistiques descriptives des rendements géométriques, accompagnées de tests de normalité (Jarque-Bera) et d’analyse des corrélations. Des tests de stationnarité (ADF, KPSS) sont ensuite appliqués pour vérifier les propriétés des séries temporelles. La modélisation économétrique est réalisée via des modèles ARIMA pour capturer les dynamiques des rendements. Enfin, un test de cointégration d’Engle et Granger est effectué pour étudier les relations de long terme entre les ETF. Les analyses ont été conduites à l’aide de Gretl.

<strong>Principaux résultats</strong>

Les rendements des ETF présentent une distribution non normale, avec une forte asymétrie et un excès de kurtosis, indiquant des événements extrêmes fréquents. Les séries de prix ne sont pas stationnaires, mais leurs premières différences le sont, validant l’utilisation des modèles ARIMA. Le test de cointégration révèle l’absence de relation de long terme stable entre les ETF étudiés.

<strong>Interprétation et implications</strong>

Ces résultats soulignent la complexité des dynamiques des actifs financiers et la nécessité d’utiliser des modèles adaptés pour la gestion de portefeuille et l’analyse des risques. La non-normalité des rendements et l’absence de cointégration montrent que les stratégies d’investissement doivent prendre en compte ces caractéristiques pour optimiser la prise de décision.

<strong>Compétences développées</strong>

Ce travail a permis de renforcer les compétences en analyse statistique, tests économétriques, modélisation de séries temporelles (modèle ARIMA), ainsi qu’en interprétation des résultats financiers.
</body>
</html>

## Data Visualisation: US-Demography and Italy's 2022 Heatwave
Working as a team of three data scientists, we delivered a two‑part analytics project that takes raw public data all the way to interactive insights:

1️⃣ U.S. County Demography Explorer
Data : NHGIS population series (2000 & 2010) for 3,100 counties.

What we built : automated R pipeline (tidyverse + sf) that cleans, joins shapefiles, and feeds a Shiny + Leaflet dashboard. Users click any county to see real‑time race break‑downs—and instantly verify census numbers such as Los Angeles County’s 9.8 M residents.

2️⃣ Climate‑Health Impact for Italy, Summer 2022
Data : ERA5 land temperatures (2015‑2023) + World Mortality Dataset.

Method : Python pipeline (pandas, xarray, statsmodels) to model expected deaths with week fixed effects, then quantify excess mortality.

Insight : ≈ 26,800 excess deaths linked to the 2022 heatwave; bin‑scatter visuals highlight a sharp mortality jump beyond the 95th‑percentile temperature.


🔧 Tech & Skills
R (tidyverse, Shiny, Leaflet) • Python (pandas, xarray, statsmodels, cartopy) • CDS & NHGIS APIs.
Spatial data wrangling │ time‑series modelling │ interactive dashboards │ agile teamwork.

Result : a compact showcase of how we transform gigabytes of climate and demographic data into actionable, recruiter‑ready insights. Let’s talk if you’re looking for data talent that bridges engineering, analytics and compelling storytelling. 📩

#DataScience #SpatialAnalytics #ClimateRisk #ShinyApps #Python #RStats

## Machine Learning – Analyse de sentiment de tweets financiers

Projet universitaire conduit par une équipe de 5 étudiants.

🔎 Pipeline NLP : nettoyage, tokenisation BERT & vectorisation TF‑IDF.

⚙️ 6 modèles comparés ; BERT en tête avec F1‑score 0,93 (binaire) et 0,75 en multi‑classe (validation croisée 5‑fold) ; BiLSTM 0,88, Random Forest / Régression logistique 0,86. ​

📈 Insights : courbe ROC, importance des tokens (SHAP) et analyse des limites (longueur 512 tokens, coût calcul). ​

🚀 Compétences acquises : fine‑tuning Transformers, optimisation hyper‑paramètres, validation croisée stratifiée, visualisation avancée & travail agile.

Présentation finale le 10 avril 2025 avec rapport 2 pages et démo live. #NLP #Transformers #SentimentAnalysis #MachineLearning

## Analyse des relations entre deux variables via des données Eurostat un projet en R

Ce projet académique consiste à analyser la relation entre deux variables (autres que le PIB et la satisfaction de vie) issues des données Eurostat. Il est structuré en quatre étapes principales : téléchargement et importation des données en R, nettoyage et fusion des ensembles de données, création de statistiques descriptives illustrées par des graphiques et tableaux, et enfin modélisation statistique (régression linéaire et non linéaire) pour examiner la relation entre les deux variables. Le travail finalisé doit être présenté dans un document PDF avec des visualisations pertinentes et des résultats d'analyse, sans inclure le code R ni les données brutes.

## Predicting high site traffic

This project aims to predict high website traffic for a recipe site by analyzing various data attributes (such as recipe IDs, nutritional values, categories, and serving sizes) to identify recipes likely to attract a large number of visitors. The approach involves data preparation, exploratory analysis, and the development of predictive models—including a linear probability model, logistic regression, and random forest—implemented in R. Model performance is assessed using confusion matrices, ROC curves, and AUC, while marginal effects and variable importance guide the site's editorial strategy.

## Data Sampling and Data Communication
This project aims to analyze electoral polls and their results to evaluate their accuracy and understand the challenges they present, particularly in the context of far-right candidates. It consists of three main parts: a theoretical analysis of polls and their methodologies, a data analysis with visualizations to assess poll accuracy, and an interpretation of the results with recommendations to improve their precision. The expected deliverable includes a concise written report and up to three graphs illustrating the key findings.

## Consommation de carburants en France, l'année 2023

Ce projet vise à analyser les prix des carburants en France pour l'année 2023 en utilisant Python. Il comprend plusieurs étapes clés : la collecte de données depuis une source prédéfinie, leur préparation via des transformations spécifiques comme l'extraction des dates ou la création d'indices de prix, ainsi que la visualisation des tendances hebdomadaires à l'aide de bibliothèques comme Matplotlib ou Seaborn. En bonus, il propose de cartographier les prix moyens par département. Enfin, le projet inclut la modélisation pour prévoir les prix futurs des carburants, en se concentrant davantage sur la méthodologie que sur l'optimisation du modèle. Le livrable attendu est un notebook Python bien documenté intégrant toutes ces étapes.

## Web Scraping and Interactive Dashboard

The project involves analyzing election polling data in groups of three by collecting information from assigned Wikipedia pages, cleaning and processing the data using Python (especially Pandas), and creating an interactive interface for users to explore the data. The interface should include visualizations, summary statistics, and manual data entry options, with libraries like Streamlit, Dash, or Tkinter recommended for a user-friendly design.

## Coffee Shop Analysis project
This project focuses on leveraging Python to analyze and visualize data for optimizing the performance of a coffee shop. Using the libraries **Matplotlib** and **Seaborn**, it involves exploring sales patterns through line plots, bar charts, scatter plots, box plots, and violin plots. The project also includes the creation of an advanced dashboard showcasing key insights, such as sales trends, product profitability, and the relationship between temperature and coffee sales. By combining these visualizations, the project provides actionable strategies to improve decision-making and business outcomes for the coffee shop.





