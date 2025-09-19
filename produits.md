# Cours sur les Produits Scalaires et Vectoriels

## 1. Introduction aux Vecteurs

### Définition
Un vecteur est un objet mathématique caractérisé par :
- **Une direction** (droite support)
- **Un sens** (orientation sur cette droite)
- **Une norme** (longueur ou intensité)

### Notation
- Vecteur : **u**, **AB**, ou u⃗ (avec flèche)
- Norme : ||**u**|| ou |**u**|
- Coordonnées en 2D : **u** = (x, y)
- Coordonnées en 3D : **u** = (x, y, z)

### Opérations de base
- **Addition :** **u** + **v** = (u₁ + v₁, u₂ + v₂, u₃ + v₃)
- **Multiplication par un scalaire :** k**u** = (ku₁, ku₂, ku₃)
- **Norme :** ||**u**|| = √(u₁² + u₂² + u₃²)

## 2. Produit Scalaire

### Définition géométrique
Le produit scalaire de deux vecteurs **u** et **v** est :
```
u · v = ||u|| × ||v|| × cos(θ)
```
où θ est l'angle entre les deux vecteurs.

### Définition algébrique
En coordonnées :
- **2D :** **u** · **v** = u₁v₁ + u₂v₂
- **3D :** **u** · **v** = u₁v₁ + u₂v₂ + u₃v₃

### Propriétés du produit scalaire
1. **Commutativité :** **u** · **v** = **v** · **u**
2. **Distributivité :** **u** · (**v** + **w**) = **u** · **v** + **u** · **w**
3. **Associativité mixte :** k(**u** · **v**) = (k**u**) · **v** = **u** · (k**v**)
4. **Positivité :** **u** · **u** = ||**u**||² ≥ 0

### Interprétations géométriques
- **u** · **v** > 0 : angle aigu (θ < 90°)
- **u** · **v** = 0 : vecteurs orthogonaux (θ = 90°)
- **u** · **v** < 0 : angle obtus (θ > 90°)

### Applications du produit scalaire
1. **Calcul d'angle :** cos(θ) = (**u** · **v**) / (||**u**|| × ||**v**||)
2. **Test d'orthogonalité :** **u** ⊥ **v** ⟺ **u** · **v** = 0
3. **Projection :** proj_v(**u**) = (**u** · **v** / ||**v**||²) × **v**

## 3. Exercices sur le Produit Scalaire

### Exercice 1 : Calcul de produit scalaire
Soit **u** = (3, -2, 1) et **v** = (1, 4, -2). Calculez **u** · **v**.

**Solution :**
**u** · **v** = 3×1 + (-2)×4 + 1×(-2) = 3 - 8 - 2 = -7

### Exercice 2 : Calcul d'angle
Calculez l'angle entre **u** = (1, 1) et **v** = (1, 0).

**Solution :**
- **u** · **v** = 1×1 + 1×0 = 1
- ||**u**|| = √(1² + 1²) = √2
- ||**v**|| = √(1² + 0²) = 1
- cos(θ) = 1 / (√2 × 1) = 1/√2 = √2/2
- θ = 45°

### Exercice 3 : Test d'orthogonalité
Les vecteurs **u** = (2, 3) et **v** = (3, -2) sont-ils orthogonaux ?

**Solution :**
**u** · **v** = 2×3 + 3×(-2) = 6 - 6 = 0
Oui, ils sont orthogonaux car leur produit scalaire est nul.

## 4. Produit Vectoriel

### Définition géométrique
Le produit vectoriel **u** ∧ **v** (ou **u** × **v**) est un vecteur tel que :
- **Direction :** perpendiculaire au plan formé par **u** et **v**
- **Sens :** donné par la règle de la main droite
- **Norme :** ||**u** ∧ **v**|| = ||**u**|| × ||**v**|| × sin(θ)

### Définition algébrique (3D uniquement)
Pour **u** = (u₁, u₂, u₃) et **v** = (v₁, v₂, v₃) :
```
u ∧ v = (u₂v₃ - u₃v₂, u₃v₁ - u₁v₃, u₁v₂ - u₂v₁)
```

### Calcul avec les déterminants
```
u ∧ v = |i  j  k|
        |u₁ u₂ u₃|
        |v₁ v₂ v₃|
```

### Propriétés du produit vectoriel
1. **Anti-commutativité :** **u** ∧ **v** = -(**v** ∧ **u**)
2. **Distributivité :** **u** ∧ (**v** + **w**) = **u** ∧ **v** + **u** ∧ **w**
3. **Associativité mixte :** k(**u** ∧ **v**) = (k**u**) ∧ **v** = **u** ∧ (k**v**)
4. **Vecteur nul :** **u** ∧ **u** = **0**

### Cas particuliers
- **u** ∧ **v** = **0** ⟺ **u** et **v** sont colinéaires
- ||**u** ∧ **v**|| = aire du parallélogramme formé par **u** et **v**

### Applications du produit vectoriel
1. **Calcul d'aire :** Aire = ||**u** ∧ **v**|| / 2 (pour un triangle)
2. **Vecteur normal :** **n** = **u** ∧ **v** (perpendiculaire au plan)
3. **Test de colinéarité :** **u** et **v** colinéaires ⟺ **u** ∧ **v** = **0**

## 5. Exercices sur le Produit Vectoriel

### Exercice 4 : Calcul de produit vectoriel
Calculez **u⃗** ∧ **v⃗** avec **u⃗** = (1, 2, 3) et **v⃗** = (2, -1, 4).

**Solution :**
**u⃗** ∧ **v⃗** = (2×4 - 3×(-1), 3×2 - 1×4, 1×(-1) - 2×2)
= (8 + 3, 6 - 4, -1 - 4)
= (11, 2, -5)

### Exercice 5 : Calcul d'aire
Calculez l'aire du triangle ABC avec A(1, 0, 0), B(0, 1, 0), C(0, 0, 1).

**Solution :**
- **AB⃗** = (-1, 1, 0)
- **AC⃗** = (-1, 0, 1)
- **AB⃗** ∧ **AC⃗** = (1×1 - 0×0, 0×(-1) - (-1)×1, (-1)×0 - 1×(-1)) = (1, 1, 1)
- ||**AB⃗** ∧ **AC⃗**|| = √(1² + 1² + 1²) = √3
- Aire = √3 / 2

### Exercice 6 : Vecteur normal à un plan
Trouvez un vecteur normal au plan passant par les points A(1, 1, 1), B(2, 3, 1), C(3, 1, 2).

**Solution :**
- **AB⃗** = (1, 2, 0)
- **AC⃗** = (2, 0, 1)
- **n⃗** = **AB⃗** ∧ **AC⃗** = (2×1 - 0×0, 0×2 - 1×1, 1×0 - 2×2) = (2, -1, -4)

## 6. Exercices Combinés

### Exercice 7 : Relations entre produits
Soit **u⃗** = (1, -1, 2), **v⃗** = (3, 0, 1), **w⃗** = (2, 1, -1).
Calculez :
a) (**u⃗** · **v⃗**) **w⃗**
b) **u⃗** · (**v⃗** ∧ **w⃗**)

**Solutions :**
a) **u⃗** · **v⃗** = 1×3 + (-1)×0 + 2×1 = 5
   (**u⃗** · **v⃗**) **w⃗** = 5(2, 1, -1) = (10, 5, -5)

b) **v⃗** ∧ **w⃗** = (0×(-1) - 1×1, 1×2 - 3×(-1), 3×1 - 0×2) = (-1, 5, 3)
   **u⃗** · (**v⃗** ∧ **w⃗**) = 1×(-1) + (-1)×5 + 2×3 = -1 - 5 + 6 = 0

### Exercice 8 : Problème géométrique
Dans un repère orthonormé, on considère les points A(2, 1, 3), B(4, 0, 1), C(1, 2, 5).
a) Calculez l'aire du triangle ABC
b) Trouvez la hauteur issue de A dans le triangle ABC

**Solutions :**
a) **AB⃗** = (2, -1, -2), **AC⃗** = (-1, 1, 2)
   **AB⃗** ∧ **AC⃗** = ((-1)×2 - (-2)×1, (-2)×(-1) - 2×2, 2×1 - (-1)×(-1)) = (0, -2, 1)
   ||**AB⃗** ∧ **AC⃗**|| = √(0² + (-2)² + 1²) = √5
   Aire = √5 / 2

b) ||**AC⃗**|| = √((-1)² + 1² + 2²) = √6
   Hauteur = (2 × Aire) / ||**AC⃗**|| = √5 / √6 = √30 / 6

## 7. Applications Avancées

### 7.1 Produit mixte
Le produit mixte de trois vecteurs **u⃗**, **v⃗**, **w⃗** est :
```
[u⃗, v⃗, w⃗] = u⃗ · (v⃗ ∧ w⃗)
```

**Propriétés :**
- Volume du parallélépipède = |**u⃗** · (**v⃗** ∧ **w⃗**)|
- Les trois vecteurs sont coplanaires ⟺ **u⃗** · (**v⃗** ∧ **w⃗**) = 0

### 7.2 Double produit vectoriel
```
u⃗ ∧ (v⃗ ∧ w⃗) = (u⃗ · w⃗)v⃗ - (u⃗ · v⃗)w⃗
```

### Exercice 9 : Volume d'un tétraèdre
Calculez le volume du tétraèdre OABC avec O(0,0,0), A(1,0,0), B(0,1,0), C(0,0,1).

**Solution :**
**OA⃗** = (1, 0, 0), **OB⃗** = (0, 1, 0), **OC⃗** = (0, 0, 1)
Volume = |**OA⃗** · (**OB⃗** ∧ **OC⃗**)| / 6
**OB⃗** ∧ **OC⃗** = (1, 0, 0)
**OA⃗** · (**OB⃗** ∧ **OC⃗**) = 1
Volume = 1/6

## 8. Exercices d'Entraînement

### Niveau Intermédiaire

**Exercice 10 :** Soit **u⃗** = (2, 1, -3) et **v⃗** = (1, -2, 4). Calculez l'angle entre **u⃗** et **v⃗**.

**Exercice 11 :** Trouvez tous les vecteurs **w⃗** = (x, y, 0) orthogonaux à **u⃗** = (1, 2, 3).

**Exercice 12 :** Calculez l'aire du parallélogramme formé par **u⃗** = (3, 4, 0) et **v⃗** = (1, 1, 2).

### Niveau Avancé

**Exercice 13 :** Démontrez que (**u⃗** ∧ **v⃗**) · **w⃗** = **u⃗** · (**v⃗** ∧ **w⃗**).

**Exercice 14 :** Trouvez l'équation du plan passant par A(1,2,3) et perpendiculaire aux vecteurs **u⃗** = (1,1,0) et **v⃗** = (0,1,1).

**Exercice 15 :** Calculez la distance entre les droites D₁: (x,y,z) = (1,0,2) + t(1,1,1) et D₂: (x,y,z) = (0,1,0) + s(2,1,0).

## 9. Applications Pratiques

### Physique
- **Force et moment :** **M⃗** = **r⃗** ∧ **F⃗**
- **Vitesse angulaire :** **v⃗** = **ω⃗** ∧ **r⃗**
- **Champ magnétique :** **F⃗** = q(**v⃗** ∧ **B⃗**)

### Géométrie
- **Équation de plan :** **n⃗** · (**r⃗** - **r₀⃗**) = 0
- **Distance point-plan :** d = |**n⃗** · (**P⃗** - **A⃗**)| / ||**n⃗**||

### Informatique graphique
- **Éclairage :** I = I₀ cos(θ) = I₀ (**n⃗** · **l⃗**)
- **Détection de collision**
- **Calcul de normales pour le rendu 3D**

## 10. Exemple Concret : Navigation Maritime

### Situation
Un bateau navigue avec une vitesse **v⃗ₛ** = (15, 10) km/h par rapport à l'eau. Un courant marin a une vitesse **v⃗ᶜ** = (5, -3) km/h.

### Calculs pratiques

**Vitesse réelle du bateau :**
**v⃗ᵣ** = **v⃗ₛ** + **v⃗ᶜ** = (15+5, 10-3) = (20, 7) km/h

**Vitesse réelle :**
||**v⃗ᵣ**|| = √(20² + 7²) = √449 ≈ 21,2 km/h

**Direction :**
tan(θ) = 7/20 = 0,35 ⟹ θ ≈ 19,3°

**Produit scalaire pour l'efficacité :**
**v⃗ₛ** · **v⃗ᶜ** = 15×5 + 10×(-3) = 75 - 30 = 45 > 0
Le courant aide partiellement le bateau.

### Autres applications maritimes
- **Calcul de cap** pour compenser la dérive
- **Optimisation de route** en utilisant les courants
- **Calcul de forces** sur les voiles (produit vectoriel vent × surface)

**Les produits scalaire et vectoriel sont essentiels pour modéliser les phénomènes physiques en 3D !**

---

*Ce cours couvre les aspects fondamentaux des produits scalaire et vectoriel. La maîtrise de ces outils est cruciale pour la géométrie, la physique et l'ingénierie !*