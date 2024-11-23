# message_classification
Ce projet se concentre sur la classification des messages en spam ou non-spam en utilisant le modèle Multinomial Naive Bayes (MultinomialNB).
# **Spam Message Classification with Multinomial Naive Bayes**  

## **Description**  
Ce projet vise à classifier les messages en **spam** ou **non-spam** à l'aide du modèle **Multinomial Naive Bayes (MultinomialNB)**.  
Le dataset utilisé, intitulé **MyBalancedSpamClassificationDataset.csv**, est équilibré pour garantir une évaluation juste des performances du modèle.  

---

## **Caractéristiques du Dataset**  
- **Nom du fichier :** `MyBalancedSpamClassificationDataset.csv`  
- **Format :** CSV (valeurs séparées par des virgules).  
- **Utilisation :** Identifier les messages spam en analysant les caractéristiques textuelles.  

---

## **Pipeline de Prétraitement**  
Un pipeline complet a été créé pour le prétraitement des données :  
1. **Nettoyage des données :**  
   - Suppression des caractères spéciaux et des mots inutiles.  
   - Conversion des messages en minuscules.  

2. **Tokenisation :**  
   - Découpage des messages en mots.  

3. **Suppression des mots-vides :**  
   - Suppression des mots courants sans pertinence pour la classification (ex. "le", "et", "de").  

4. **Vectorisation :**  
   - Conversion des textes en représentations numériques avec **TF-IDF** ou **Count Vectorizer**.  

---

## **Entraînement du Modèle**  
- **Algorithme utilisé :** Multinomial Naive Bayes (MultinomialNB).  
- **Étapes :**  
  1. Division des données en ensembles d’entraînement et de test.  
  2. Entraînement du modèle sur les données prétraitées.  
  3. Évaluation des performances avec des métriques comme :  
     - **Précision (Accuracy)**  
     - **Rappel (Recall)**  
     - **F1-Score**  

---

## **Exécution**  

### **1. Prérequis**  
Assurez-vous d’avoir Python installé avec les bibliothèques suivantes :  
 numpy pandas scikit-learn nltk
---
## Résultats Attendus
Une matrice de confusion montrant les prédictions du modèle.
Un rapport d’évaluation avec les scores de précision, rappel et F1. 
et un score de 98%
