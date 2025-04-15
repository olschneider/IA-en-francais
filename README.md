# IA-en-francais

Cette page reprend les différentes sources d'information que je peux trouver sur la compréhension de l'IA en Francais

- Les tenseurs. Niveau:Débutant. https://www.toolify.ai/fr/ai-new-fr/les-tenseurs-pour-les-dbutants-dfinition-dun-tenseur-437491. Date: Janvier 2024
- Le Deep Learning. Niveau:Intermédiaire. https://www.geeksforgeeks.org/deep-learning-tutorial/  . Date: Décembre 2024
- Les transformers (orienté Hugging Face mais bon principes). Niveau: Débutant. https://huggingface.co/learn/nlp-course/fr/chapter0/1?fw=pt .Date: 2024
- Principe d'Attention dans l'IA. Niveau: Avancé. https://arxiv.org/abs/1706.03762 (à traduire mais indispensable pour les LLM actuels) . Date: Aout 2023 (v7)

## Les outils
- Les notebooks Jupyter. Niveau: Débutant. https://fr.wikipedia.org/wiki/Jupyter.
- Google Colab. Niveau Débutant. Bon moyen de faire des tests d'inférence sur les différents types de tache et les différents modèles LLM avec une puissance de calcul de base.  

## Machine Learning
- Apprentissage supervisé
- Apprentissage non supervisé
- Apprentissage par renforcement
- IA générative

### Composants
- Données d'entrainenment. Idéalement très diversifiées et très volumineuses.
- Modèle. Traitement, souvent mathématiques, des données en entrée pour faire une prédiction en sortie.
- Entrainement. Le modèle est entrainer avec les données d'enntrainement. Avec les données, il réalise des prédictions et les soumet à à sa propre validation pour itération pour affiner ses résuiltats.
- Inférence ou prédiction. Demande faite au modèle de prédire un résultat en fonction d'une entrée.   

### Apprentissage supervisé
Cas d'usages courants modèles de Regression et modèles de Classification.  
La regression produit une valeur nuémrique.  
La classification produit une classe (ex: chaine de caractère) correspond au mieux au type d'enregistrement en entrée.  
Dans les 2 cas, les modèles vont se servir des données d'entrainement, étiquettées vraies ou fausses, pour établir une règle qui tentera de déterminer si une entrée correspond à une sortie.  
Exemple très schématisé pour la régression, si le modèle a appris via son entrainement que toutes les maisons dans le 18e à Paris se sont vendues à 3 000 000 euros lors des 15 dernières années alors une prédira qu'une maison à vendre dans le 18e à Paris aujourd'hui aura des chances de se vendre 3 000 000 d'euros.  
De même pour la classification, si le modèle a appris que toutes les personnes pesant entre 100 et 180 kg étaient gros alors il classera une personne pesant 105 Kg comme étant gros.   
L'étiquettage des données fondamentale dans ce type d'apprentissage. L'utilisateur qui veut faire une inférence doit connaitre les étiquettes pour interprêter les données de sortie.    
(exemples de dataset d'apprentissage dispos https://www.data.gouv.fr/fr/datasets/)  

### Apprentissage non supervisé
Les modèles utilisant ce type d'apprentissage ne se basent pas sur des données classées (labélisées, étiquetées).  
Ils vont essayer de trouver des caractéristiques mathématiques, dans leur ensemble de données d'apprentissage, leur permettant de faire des prédictions sur une entrée donnée.  
Une technique couramment utilisée est le clustering qui tente de faire ressortir des groupes de données à l'intérieur d'un groupe plus vaste. L'interprétation des groupes trouvés ne fait pas forcément partie des sortie du modèle.  
Exemple donné par Google: avec l'ensemble des températures journalières sur un an, un modèle non supervisé peut créer des clusters de points (représentant les températures de jour), un cluster pour les points froids, tièdes et chauds. Les clusters représenteront normalement les saisons seront définis mais le nommage des saisons (été, automne...) peut ne pas faire partie de la sortie du modèle.

### Apprentissage par renforcement
Les modèles de ce type sont régis par le principe de récompenses. Le but du modèle est d'être recompensé pour avoir la stratégie la meilleure et la plus optimale.

### IA générative


