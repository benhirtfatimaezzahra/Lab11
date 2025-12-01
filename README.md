# Lab11 – Broadcasting et Calcul Vectoriel NumPy

Application avancée des concepts de broadcasting et de calcul vectoriel avec NumPy. Ce lab explore les opérations entre tableaux de dimensions différentes, les fonctions universelles (ufuncs) et le filtrage avec masques booléens.

Le programme démontre comment NumPy étend automatiquement les dimensions des tableaux pour permettre des opérations efficaces sans boucles explicites.

---

## Fonctionnalités

### Broadcasting
- **Scalaire + Tableau** : addition d'une valeur unique à tous les éléments
- **Vecteur ligne + Matrice** : diffusion d'un vecteur (1, n) sur une matrice (m, n)
- **Vecteur colonne + Matrice** : diffusion d'un vecteur (m, 1) sur une matrice (m, n)
- **Règles de compatibilité** : alignement automatique des dimensions
- **Optimisation mémoire** : pas de duplication physique des données

### Calcul Vectoriel
- **Opérations arithmétiques** : multiplication, addition sur tableaux entiers
- **Fonctions mathématiques** : `np.sin()`, `np.log()`, `np.mean()`
- **Compositions** : combinaison de plusieurs opérations en une expression
- **Performance** : calculs optimisés sans boucles Python

### Filtrage avec Masques
- **Masques booléens** : création avec conditions (`>`, `<`, `==`)
- **Indexation avancée** : sélection d'éléments selon critères
- **Filtrage après ufunc** : application de conditions sur résultats de fonctions
- **Extraction de sous-ensembles** : récupération des valeurs satisfaisant une condition

### Contrôle des Dimensions
- **Vérification de shapes** : inspection des dimensions après opérations
- **Compatibilité broadcasting** : validation des formes compatibles
- **Transformation de forme** : vecteur ligne vs vecteur colonne

---

## Architecture
```
Lab11.ipynb → Notebook Jupyter contenant :

1. Données initiales
   - A : tableau 1D [10, 20, 30, 40, 50]
   - M : matrice 3×3

2. Étape 5 : Broadcasting
   - Task 5.1 : Scalaire + Tableau
     * Addition de 5 à tous les éléments
     * Comparaison des shapes
   
   - Task 5.2 : Vecteur ligne + Matrice
     * Création vecteur [10, 20, 30]
     * Broadcasting sur chaque ligne de M
     * Vérification des dimensions
   
   - Task 5.3 : Vecteur colonne + Matrice
     * Création vecteur [[10], [20], [30]]
     * Broadcasting sur chaque colonne de M
     * Analyse des shapes résultantes
   
   - Task 5.4 : Rappel des règles
     * Documentation du broadcasting
     * Conditions de compatibilité

3. Étape 6 : Calcul vectoriel et filtrage
   - Task 6.1 : Calcul vectoriel global
     * Expression combinée (A * 2) + sin(A) - mean(A)
     * Opérations multiples en une ligne
   
   - Task 6.2 : Filtrage après ufunc
     * Calcul du logarithme log(A)
     * Création d'un masque booléen (> 2)
     * Extraction des valeurs filtrées
   
   - Task 6.3 : Contrôle des shapes
     * Récapitulatif de toutes les dimensions
     * Vérification de cohérence
```

---

## Installation

Cloner le projet :
```bash
git clone https://github.com/benhirtfatimaezzahra/Lab11.git
```

Installer NumPy (si nécessaire) :
```bash
pip install numpy
```

Ouvrir le notebook avec Jupyter :
```bash
cd Lab11
jupyter notebook Lab11.ipynb
```

Ou utilisez JupyterLab :
```bash
jupyter lab Lab11.ipynb
```

---



## Notes Techniques

### Concepts NumPy utilisés
- **Broadcasting** : extension automatique des dimensions
- **Ufuncs (Universal Functions)** : `np.sin()`, `np.log()`, `np.mean()`
- **Opérations vectorisées** : calculs sur tableaux entiers sans boucles
- **Masques booléens** : tableaux de True/False pour filtrage
- **Indexation avancée** : `array[masque]` pour extraction conditionnelle
- **Shape manipulation** : vecteur ligne (n,) vs vecteur colonne (n, 1)


---

## Démonstration

<img width="1599" height="726" alt="image" src="https://github.com/user-attachments/assets/078d3861-e80c-426b-a0ac-160f10f239c4" />
<img width="1558" height="725" alt="image" src="https://github.com/user-attachments/assets/43e2d7cb-23c3-493a-b3cf-24a8a58cd6ce" />
<img width="1636" height="627" alt="image" src="https://github.com/user-attachments/assets/20474124-a858-4655-aa2a-4bdb788b8679" />
<img width="1638" height="762" alt="image" src="https://github.com/user-attachments/assets/a1b57864-3660-46b7-bcb4-487ab976d3ec" />
<img width="1619" height="432" alt="image" src="https://github.com/user-attachments/assets/fe730aef-9061-45d6-949c-cd5e97e2055f" />

---

## Auteur

**Nom :** Benhirt Fatima Ezzahra  
**Cours :** Introduction à Python  
**Date :** Décembre 2025  
**Encadré par :** Pr. Mohamed LACHGAR
