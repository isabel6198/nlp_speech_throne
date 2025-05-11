

https://policyagendasuk.wordpress.com/datasets/  

### Discours du Trône 1911–2012 


Le Discours du Trône (Discours du Roi ou de la Reine) expose les priorités exécutives et législatives du gouvernement britannique pour la prochaine session parlementaire. Le texte intégral du discours a été codé au niveau de la « quasi-phrase » (c’est-à-dire une expression contenant une seule idée politique ou un seul sujet). Les transcriptions ont été codées à l’aveugle par deux chercheurs qui ont comparé leurs résultats pour décider si chaque quasi-phrase contenait du contenu politique, puis lui ont assigné un code de sujet principal et de sous-sujet. Cette méthode a permis d’atteindre un accord inter-codeur de 90 % pour les sujets principaux sur la plupart des années. Les désaccords restants ont été résolus par discussion, et les responsables du projet ont tranché dans les rares cas de désaccord persistant.



### Nous données sont repartis ainsi :

105 discours (chaque ligne = un discours du trône complet)
3 colonnes :

Speech_Year : année du discours
Date : date exacte
Text : texte intégral du discours



### Techniques utilisées :


Nettoyage	                Tokenisation, lemmatisation (spaCy)
Vectorisation       	    CountVectorizer, TfidfVectorizer
Thématisation	            LatentDirichletAllocation (LDA)
Sentiment (optionnel)	    VADER via NLTK


Visualisation	quelques graphiques avec matplotlib, seaborn, wordcloud


### Périodes : 

Monarque         | Règne          | Période à filtrer dans `df['Speech_Year']` |
| ---------------- | -------------- | ------------------------------------------ |
| **George V**     | 1910 – 1936    | 1911 – 1935                                |
| **Edward VIII**  | 1936 (abdiqué) | aucun discours (abdiqué avant le discours) |
| **George VI**    | 1936 – 1952    | 1937 – 1951                                |
| **Elizabeth II** | 1952 – 2022    | 1952 – 2012 *(fin de ton corpus)*          |




## comment choisir le bon nombre 

Il est possible de se fier à des indicateurs de cohérence et de perplexité afin de cibler le nombre minimal de thématiques avec la meilleure cohérence possible

https://gardeso.com/wp-content/uploads/2019/06/Berube_GARDESO2019.pdf


Qu’est-ce que la perplexité?

La perplexité est une mesure de la façon dont le modèle thématique prédit des données nouvelles ou invisibles. Il reflète la capacité de généralisation du modèle. Un faible score de perplexité signifie que le modèle est confiant et précis dans ses prédictions. Un score de perplexité élevé signifie que le modèle est incertain et inexact dans ses prédictions.

https://www.linkedin.com/advice/1/how-do-you-evaluate-coherence-perplexity?lang=fr&originalSubdomain=fr 

