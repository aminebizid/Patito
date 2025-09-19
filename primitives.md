# Cours sur les Primitives et Intégrales

## 1. Introduction aux Primitives

### Définition
Une primitive (ou antidérivée) d'une fonction f(x) est une fonction F(x) telle que F'(x) = f(x).

**Notation :**
- Si F'(x) = f(x), alors F(x) est une primitive de f(x)
- L'ensemble des primitives s'écrit : ∫ f(x) dx = F(x) + C

### Propriété fondamentale
Si F(x) est une primitive de f(x), alors F(x) + C (où C est une constante) est aussi une primitive de f(x).

### Lien avec les dérivées
Les primitives sont l'opération inverse de la dérivation :
- Dérivation : F(x) → F'(x) = f(x)
- Primitivation : f(x) → F(x) + C où F'(x) = f(x)

## 2. Primitives de Base

### Table des primitives usuelles
| Fonction f(x) | Primitive F(x) |
|---------------|----------------|
| k (constante) | kx + C |
| x | x²/2 + C |
| xⁿ (n ≠ -1) | xⁿ⁺¹/(n+1) + C |
| 1/x | ln|x| + C |
| eˣ | eˣ + C |
| aˣ | aˣ/ln(a) + C |
| cos(x) | sin(x) + C |
| sin(x) | -cos(x) + C |
| 1/cos²(x) = sec²(x) | tan(x) + C |
| 1/√(1-x²) | arcsin(x) + C |
| 1/(1+x²) | arctan(x) + C |

### Propriétés des primitives

#### 1. Linéarité
```
∫ [af(x) + bg(x)] dx = a∫ f(x) dx + b∫ g(x) dx
```

#### 2. Primitive d'une somme
```
∫ [f(x) + g(x)] dx = ∫ f(x) dx + ∫ g(x) dx
```

## 3. Exercices Simples

### Exercice 1 : Primitives de base
Calculez les primitives suivantes :

a) ∫ 3x² dx

b) ∫ (2x + 5) dx

c) ∫ 1/x dx

d) ∫ √x dx

**Solutions :**

a) ∫ 3x² dx = 3 · x³/3 + C = x³ + C

b) ∫ (2x + 5) dx = x² + 5x + C

c) ∫ 1/x dx = ln|x| + C

d) ∫ √x dx = ∫ x^(1/2) dx = x^(3/2)/(3/2) + C = (2/3)x^(3/2) + C

### Exercice 2 : Polynômes

Calculez la primitive de :

f(x) = 4x³ - 6x² + 2x - 1

**Solution :**

∫ (4x³ - 6x² + 2x - 1) dx = x⁴ - 2x³ + x² - x + C

### Exercice 3 : Fonctions trigonométriques

Calculez les primitives de :

a) f(x) = sin(x) + cos(x)

b) g(x) = 3sin(x) - 2cos(x)

**Solutions :**

a) ∫ [sin(x) + cos(x)] dx = -cos(x) + sin(x) + C

b) ∫ [3sin(x) - 2cos(x)] dx = -3cos(x) - 2sin(x) + C

## 4. Méthodes d'Intégration

### 4.1 Intégration par substitution

**Principe :** 

Si ∫ f(g(x)) · g'(x) dx, on pose u = g(x), donc du = g'(x) dx

**Exemple :** 

∫ 2x cos(x²) dx

- Posons u = x², donc du = 2x dx
- L'intégrale devient : ∫ cos(u) du = sin(u) + C = sin(x²) + C

### 4.2 Intégration par parties

**Formule :** 

∫ u dv = uv - ∫ v du

**Exemple :** ∫ x eˣ dx
- Posons u = x et dv = eˣ dx
- Donc du = dx et v = eˣ
- ∫ x eˣ dx = x eˣ - ∫ eˣ dx = x eˣ - eˣ + C = eˣ(x - 1) + C

## 5. Exercices Intermédiaires

### Exercice 4 : Substitution simple

Calculez ∫ (3x + 1)⁵ dx

**Solution :**
Posons u = 3x + 1, donc du = 3 dx, d'où dx = du/3

∫ (3x + 1)⁵ dx = ∫ u⁵ · (du/3) = (1/3) ∫ u⁵ du = (1/3) · u⁶/6 + C = u⁶/18 + C = (3x + 1)⁶/18 + C

### Exercice 5 : Fonctions composées
Calculez ∫ x/√(x² + 1) dx

**Solution :**
Posons u = x² + 1, donc du = 2x dx, d'où x dx = du/2
∫ x/√(x² + 1) dx = ∫ (1/√u) · (du/2) = (1/2) ∫ u^(-1/2) du = (1/2) · 2u^(1/2) + C = √(x² + 1) + C

### Exercice 6 : Intégration par parties
Calculez ∫ x sin(x) dx

**Solution :**
Posons u = x et dv = sin(x) dx
Donc du = dx et v = -cos(x)
∫ x sin(x) dx = -x cos(x) - ∫ (-cos(x)) dx = -x cos(x) + sin(x) + C

## 6. Intégrales Définies

### Théorème fondamental du calcul
Si F(x) est une primitive de f(x), alors :
```
∫[a à b] f(x) dx = F(b) - F(a) = [F(x)]ᵃᵇ
```

### Propriétés des intégrales définies
1. ∫[a à a] f(x) dx = 0
2. ∫[a à b] f(x) dx = -∫[b à a] f(x) dx
3. ∫[a à b] f(x) dx + ∫[b à c] f(x) dx = ∫[a à c] f(x) dx
4. ∫[a à b] [f(x) + g(x)] dx = ∫[a à b] f(x) dx + ∫[a à b] g(x) dx

### Exercice 7 : Intégrale définie simple
Calculez ∫[0 à 2] x² dx

**Solution :**
∫[0 à 2] x² dx = [x³/3]₀² = 8/3 - 0 = 8/3

## 7. Exercices Compliqués

### Exercice 8 : Substitution complexe
Calculez ∫ sin³(x) cos(x) dx

**Solution :**
Posons u = sin(x), donc du = cos(x) dx
∫ sin³(x) cos(x) dx = ∫ u³ du = u⁴/4 + C = sin⁴(x)/4 + C

### Exercice 9 : Intégration par parties répétée
Calculez ∫ x² eˣ dx

**Solution :**
Première intégration par parties : u = x², dv = eˣ dx
du = 2x dx, v = eˣ
∫ x² eˣ dx = x² eˣ - ∫ 2x eˣ dx

Deuxième intégration par parties : u = 2x, dv = eˣ dx
du = 2 dx, v = eˣ
∫ 2x eˣ dx = 2x eˣ - ∫ 2 eˣ dx = 2x eˣ - 2eˣ

Donc : ∫ x² eˣ dx = x² eˣ - (2x eˣ - 2eˣ) + C = eˣ(x² - 2x + 2) + C

### Exercice 10 : Fractions rationnelles
Calculez ∫ 1/(x² - 1) dx

**Solution :**
Décomposition en éléments simples : 1/(x² - 1) = 1/((x-1)(x+1)) = A/(x-1) + B/(x+1)
1 = A(x+1) + B(x-1)
Pour x = 1 : 1 = 2A, donc A = 1/2
Pour x = -1 : 1 = -2B, donc B = -1/2

∫ 1/(x² - 1) dx = ∫ [1/2 · 1/(x-1) - 1/2 · 1/(x+1)] dx = (1/2)ln|x-1| - (1/2)ln|x+1| + C = (1/2)ln|x-1|/|x+1| + C

### Exercice 11 : Intégrale avec racine
Calculez ∫ √(1 - x²) dx

**Solution :**
Substitution trigonométrique : x = sin(θ), dx = cos(θ) dθ
√(1 - x²) = √(1 - sin²(θ)) = cos(θ)
∫ √(1 - x²) dx = ∫ cos²(θ) dθ = ∫ (1 + cos(2θ))/2 dθ = θ/2 + sin(2θ)/4 + C
= θ/2 + (sin(θ)cos(θ))/2 + C = arcsin(x)/2 + (x√(1-x²))/2 + C

## 8. Applications des Intégrales

### Calcul d'aires
L'aire sous la courbe y = f(x) entre x = a et x = b est :
```
Aire = ∫[a à b] f(x) dx
```

### Exercice 12 : Aire sous une parabole
Calculez l'aire sous la courbe y = x² entre x = 0 et x = 3.

**Solution :**
Aire = ∫[0 à 3] x² dx = [x³/3]₀³ = 27/3 - 0 = 9 unités²

### Volume de solides de révolution
Volume obtenu en faisant tourner y = f(x) autour de l'axe des x :
```
V = π ∫[a à b] [f(x)]² dx
```

### Exercice 13 : Volume d'un cône
Calculez le volume du cône obtenu en faisant tourner y = x autour de l'axe des x, de x = 0 à x = h.

**Solution :**
V = π ∫[0 à h] x² dx = π [x³/3]₀ʰ = π h³/3

## 9. Exercices d'Entraînement Supplémentaires

### Niveau Avancé

**Exercice 14 :** ∫ eˣ sin(x) dx (par parties répétées)

**Exercice 15 :** ∫ 1/√(x² + 1) dx (substitution trigonométrique)

**Exercice 16 :** ∫[0 à π/2] sin⁴(x) dx (réduction)

**Exercice 17 :** ∫ ln(x) dx (par parties)

**Exercice 18 :** Calculez l'aire entre y = x² et y = x³ de x = 0 à x = 1

## 10. Conseils pour Maîtriser les Primitives

1. **Mémorisez les primitives de base**
2. **Identifiez la méthode appropriée :**
   - Substitution pour les fonctions composées
   - Parties pour les produits de fonctions différentes
   - Décomposition pour les fractions rationnelles
3. **Vérifiez en dérivant votre résultat**
4. **N'oubliez jamais la constante C**
5. **Pratiquez les techniques de calcul régulièrement**

## 11. Exemple Concret : Les Primitives dans la Vie Réelle

### Exemple : Distance parcourue par une voiture

**Situation :** Vous connaissez la vitesse de votre voiture à chaque instant et vous voulez calculer la distance totale parcourue.

**La fonction :** Si votre vitesse est donnée par v(t) = 3t² + 2t + 5 (en m/s, où t est en secondes)

**La primitive :** Pour trouver la distance, on calcule ∫ v(t) dt = t³ + t² + 5t + C

**Calcul pratique :**
Distance parcourue entre t = 0 et t = 10 secondes :
∫[0 à 10] (3t² + 2t + 5) dt = [t³ + t² + 5t]₀¹⁰ = (1000 + 100 + 50) - 0 = 1150 mètres

**Ce que cela nous dit :**
- La primitive de la vitesse donne la position (ou distance)
- L'intégrale définie donne le déplacement total sur un intervalle de temps

### Autres Exemples Quotidiens

- **Physique :** Calcul du travail d'une force variable : W = ∫ F(x) dx
- **Économie :** Coût total à partir du coût marginal : C(x) = ∫ Cm(x) dx
- **Médecine :** Dose totale de médicament administrée : D = ∫ débit(t) dt
- **Ingénierie :** Volume d'eau dans un réservoir à partir du débit : V = ∫ débit(t) dt
- **Statistiques :** Probabilité à partir de la densité : P(a < X < b) = ∫[a à b] f(x) dx

**Les primitives permettent de reconstituer une grandeur totale à partir de son taux de variation !**

---

*Ce cours couvre les aspects essentiels des primitives et intégrales. La maîtrise des techniques d'intégration demande de la pratique régulière !*