# Analyse NLP des discours du trône au Royaume-Uni (1911–2012)

## Contexte académique

- **Filière :** Master 2 ECAP  
- **Matière :** Traitement Automatique du Langage Naturel (NLP)  
- **Encadrant :** M. Bennani  
- **Période :** Mai 2025  
- **Étudiantes :** Cassandre Orhan, Isabel Palacio Barco, Lauriane Belane Tanga & Marie Kerhoas

---

## Sujet

**Titre :** *Étude des discours du trône au Royaume-Uni par NLP (1911–2012)*  
**Sous-titre :** *Une analyse sur les thématiques, les partis politiques et les sentiments des discours*

Ce projet vise à explorer, via les techniques de traitement automatique du langage naturel, les discours prononcés lors des ouvertures officielles du Parlement britannique. L’étude porte sur :
- les thématiques évoquées dans les discours
- l’évolution du contenu selon le parti politique au pouvoir
- les sentiments exprimés à travers le temps

---

##  Contenu du notebook `01_speech_throne.ipynb`

Le notebook inclut les étapes suivantes :
1. Prétraitement des données textuelles (lemmatisation, stop words, etc)
2. Analyse thématique par LDA 
3. Analyse des sentiments avec VADER 
4. Modélisation

---

## Bibliothèques utilisées (requirements.txt)

Ce projet s’appuie sur les packages suivants :

- **Traitement NLP**
  - `spacy` : Tokenisation, POS, entités nommées
  - `nltk` : Analyse de sentiments (VADER)
- **Vectorisation & ML**
  - `scikit-learn` : TF-IDF, LDA, métriques
- **Manipulation de données**
  - `pandas`, `numpy`
- **Visualisation**
  - `matplotlib`, `seaborn`
  - `wordcloud` : Nuages de mots
  - `pyLDAvis` : Visualisation interactive des topics
- **Fichiers Excel**
  - `openpyxl`

---
