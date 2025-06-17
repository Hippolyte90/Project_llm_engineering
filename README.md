# Projet d'Ingénierie LLM

Ce projet est une collection d'applications et d'outils avancés basés sur l'Intelligence Artificielle et les Large Language Models (LLMs). Il comprend plusieurs notebooks Jupyter qui démontrent différentes applications pratiques de l'IA.

## 📚 Composants du Projet

### Applications Principales

1. **Solution Commerciale & Brochure d'Entreprise**
   - `solution_commerciale_brochure_entreprise.ipynb` : Générateur de brochures d'entreprise
   - `company_brochure_generator.ipynb` : Outil de création de brochures

2. **Assistant IA Multimodal**
   - `multi-modal_Airline_AI_assistant.ipynb` : Assistant IA pour le secteur aérien

3. **Générateur de Code C++**
   - `high_performance_cpp_code_generator.ipynb` : Outil de génération de code C++ optimisé

4. **Travailleur du Savoir Personnel**
   - `personal_knowledge_worker.ipynb` : Système de gestion des connaissances personnelles
   - `personal_knowledge/` : Répertoire contenant les données de connaissances

5. **Outils de Communication**
   - `conversation_3P_LLMs.ipynb` : Système de conversation multi-LLMs
   - `minute_meeting.ipynb` : Générateur de comptes-rendus de réunion

## 🛠️ Installation (Windows)

### Prérequis
1. Installer [Anaconda](https://www.anaconda.com/download)
2. Installer [Git](https://git-scm.com/download/win)

### Étapes d'Installation

1. **Cloner le Répertoire**
   ```powershell
   mkdir dossier_projet
   cd dossier_projet
   git clone [URL_DE_VOTRE_REPO]
   ```
2. **Configuration de l'Environnement**
   - Créer un fichier `.env` à la racine du projet
   - Utiliser le Bloc-notes Windows pour créer le fichier
   - Enregistrer sous le nom `.env` (selectionnez "Tous les fichiers")
   - Ajouter vos clés API pour :
     - OpenAI
     - Anthropic
     - Google AI
     - Autres services selon vos besoins
    
3. **Créer l'Environnement avec Anaconda**
   - Ouvrir "Anaconda PowerShell Prompt"
   - Naviguer vers votre dossier cloné
   - Exécuter les commandes suivantes :
   ```bash
   conda env create -f environment.yml  # Prend 1-10 minutes
   conda activate llms
   python --version  # Vérifier la version de Python
   ```

4. **Configuration avec pip (Alternative)**
   - Dans Windows PowerShell :
   ```powershell
   cd [votre_dossier]
   venv\Scripts\activate
   python -m pip install --upgrade pip
   pip install -r requirements.txt
   ```


## 🤖 Guide des LLMs

### Critères de Comparaison des LLMs

#### LLMs Propriétaires vs Open Source
- GPT-4
- Gemini 2.5 Pro
- Claude
- Autres modèles open source (disponible sur HuggingFace)

#### Métriques d'Évaluation
1. **ARC (AI2 Reasoning Challenge)**
   - Évalue la capacité de raisonnement scientifique
   - Questions à choix multiples

2. **MMLU (Massive Multitask Language Understanding)**
   - Évalue la compréhension sur 57+ sujets complexes
   - Test de connaissances générales

3. **TruthfulQA**
   - Mesure l'exactitude et la véracité des réponses
   - Évaluation de la fiabilité

4. **GSM8K**
   - Test de résolution de problèmes mathématiques
   - Niveau élémentaire à moyen

#### Critères de Base
- Date de sortie
- Coût d'utilisation
- Nombre de paramètres
- Nombre de tokens d'entraînement
- Longueur du contexte

#### Loi Chinchilla
- Principe important : le nombre de paramètres doit être proportionnel au nombre de tokens d'entraînement
- Impact sur les performances du modèle

## 🚀 Utilisation
Ouvrir "Anaconda PowerShell Prompt"
Accéder au dossier
1. Activer l'environnement :
   ```bash
   conda activate llms
   ```

2. Lancer Jupyter Lab :
   ```bash
   jupyter lab
   ```

3. Ouvrir et exécuter les notebooks souhaités

## 📦 Dépendances Principales

- LangChain et ses extensions
- Transformers
- PyTorch
- OpenAI
- Anthropic
- Google Generative AI
- Gradio
- FAISS
- ChromaDB
- Et autres bibliothèques d'IA et de traitement de données

## 🤝 Contribution

Les contributions sont les bienvenues ! N'hésitez pas à :
1. Fork le projet
2. Créer une branche pour votre fonctionnalité
3. Commiter vos changements
4. Pousser vers la branche
5. Ouvrir une Pull Request

## 📝 Licence

Ce projet est sous licence MIT. Voir le fichier LICENSE pour plus de détails.

## ⚠️ Notes Importantes

1. Assurez-vous d'avoir les clés API nécessaires
2. Respectez les conditions d'utilisation des services d'IA
3. Vérifiez la compatibilité des versions de Python et des dépendances
4. Considérez les coûts d'utilisation des différents LLMs
5. Tenez compte des limitations de contexte et de performance selon vos besoins 