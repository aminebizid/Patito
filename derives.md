# Cours sur les Dérivées Mathématiques

## 1. Introduction aux Dérivées

### Définition
La dérivée d'une fonction f(x) en un point x₀ représente le taux de variation instantané de la fonction en ce point. Elle correspond à la pente de la tangente à la courbe au point considéré.

**Définition formelle :**
```
f'(x₀) = lim[h→0] [f(x₀ + h) - f(x₀)] / h
```

### Interprétation géométrique
- La dérivée f'(x₀) est la pente de la tangente à la courbe y = f(x) au point (x₀, f(x₀))
- Si f'(x₀) > 0 : la fonction est croissante en x₀
- Si f'(x₀) < 0 : la fonction est décroissante en x₀
- Si f'(x₀) = 0 : point critique (maximum, minimum ou point d'inflexion)

## 2. Règles de Dérivation

### Dérivées de base
| Fonction | Dérivée |
|----------|---------|
| f(x) = c (constante) | f'(x) = 0 |
| f(x) = x | f'(x) = 1 |
| f(x) = xⁿ | f'(x) = n·xⁿ⁻¹ |
| f(x) = eˣ | f'(x) = eˣ |
| f(x) = ln(x) | f'(x) = 1/x |
| f(x) = sin(x) | f'(x) = cos(x) |
| f(x) = cos(x) | f'(x) = -sin(x) |
| f(x) = tan(x) | f'(x) = 1 + tan²(x) = sec²(x) |

### Règles de calcul

#### 1. Règle de la somme
```
(f + g)' = f' + g'
```

#### 2. Règle du produit
```
(f · g)' = f' · g + f · g'
```

#### 3. Règle du quotient
```
(f/g)' = (f' · g - f · g') / g²
```

#### 4. Règle de la chaîne
```
(f ∘ g)'(x) = f'(g(x)) · g'(x)
```

## 3. Exercices Simples

### Exercice 1 : Dérivées de base
Calculez les dérivées des fonctions suivantes :

a) f(x) = 5x³

b) g(x) = 2x² + 3x - 1

c) h(x) = √x

d) k(x) = 1/x


**Solutions :**
a) f'(x) = 15x²
b) g'(x) = 4x + 3
c) h(x) = x^(1/2), donc h'(x) = (1/2)x^(-1/2) = 1/(2√x)
d) k(x) = x⁻¹, donc k'(x) = -x⁻² = -1/x²

### Exercice 2 : Règle de la somme
Calculez la dérivée de :
f(x) = 3x⁴ - 2x³ + 5x² - 7x + 2

**Solution :**
f'(x) = 12x³ - 6x² + 10x - 7

### Exercice 3 : Règle du produit
Calculez la dérivée de :
f(x) = (2x + 1)(x² - 3)

**Solution :**
f'(x) = 2(x² - 3) + (2x + 1)(2x) = 2x² - 6 + 4x² + 2x = 6x² + 2x - 6

## 4. Exercices Intermédiaires

### Exercice 4 : Règle du quotient
Calculez la dérivée de :
f(x) = (x² + 1)/(x - 2)

**Solution :**
f'(x) = [2x(x - 2) - (x² + 1)(1)] / (x - 2)²
f'(x) = [2x² - 4x - x² - 1] / (x - 2)²
f'(x) = (x² - 4x - 1) / (x - 2)²

### Exercice 5 : Fonctions trigonométriques
Calculez les dérivées de :
a) f(x) = x sin(x)
b) g(x) = cos(x)/x

**Solutions :**
a) f'(x) = sin(x) + x cos(x)
b) g'(x) = [-sin(x) · x - cos(x) · 1] / x² = (-x sin(x) - cos(x)) / x²

### Exercice 6 : Règle de la chaîne (simple)
Calculez la dérivée de :
f(x) = (2x + 3)⁵

**Solution :**
f'(x) = 5(2x + 3)⁴ · 2 = 10(2x + 3)⁴

## 5. Exercices Compliqués

### Exercice 7 : Composition complexe
Calculez la dérivée de :
f(x) = sin(x² + 3x)

**Solution :**
f'(x) = cos(x² + 3x) · (2x + 3)

### Exercice 8 : Produit avec composition
Calculez la dérivée de :
f(x) = x³ · e^(2x+1)

**Solution :**
f'(x) = 3x² · e^(2x+1) + x³ · e^(2x+1) · 2
f'(x) = e^(2x+1)(3x² + 2x³)
f'(x) = x²e^(2x+1)(3 + 2x)

### Exercice 9 : Quotient avec composition
Calculez la dérivée de :
f(x) = ln(x)/(x² + 1)

**Solution :**
f'(x) = [(1/x)(x² + 1) - ln(x) · 2x] / (x² + 1)²
f'(x) = [x + 1/x - 2x ln(x)] / (x² + 1)²
f'(x) = [x² + 1 - 2x² ln(x)] / [x(x² + 1)²]

### Exercice 10 : Fonction implicite
Trouvez dy/dx si : x² + y² = 25

**Solution :**
En dérivant implicitement :
2x + 2y(dy/dx) = 0
dy/dx = -x/y

### Exercice 11 : Dérivée logarithmique
Calculez la dérivée de :
f(x) = x^x (pour x > 0)

**Solution :**
On utilise ln(f(x)) = x ln(x)
En dérivant : f'(x)/f(x) = ln(x) + 1
Donc : f'(x) = x^x(ln(x) + 1)

### Exercice 12 : Composition très complexe
Calculez la dérivée de :
f(x) = e^(sin(√(x² + 1)))

**Solution :**
f'(x) = e^(sin(√(x² + 1))) · cos(√(x² + 1)) · (1/2)(x² + 1)^(-1/2) · 2x
f'(x) = e^(sin(√(x² + 1))) · cos(√(x² + 1)) · x/√(x² + 1)

## 6. Applications des Dérivées

### Étude de fonctions
- **Points critiques :** f'(x) = 0
- **Croissance :** f'(x) > 0 ⟹ fonction croissante
- **Décroissance :** f'(x) < 0 ⟹ fonction décroissante

### Optimisation
Pour trouver les extrema d'une fonction :
1. Calculer f'(x)
2. Résoudre f'(x) = 0
3. Étudier le signe de f'(x) autour des points critiques

### Problème d'optimisation (Exercice 13)
Un rectangle est inscrit dans un demi-cercle de rayon R. Quelles sont les dimensions qui maximisent l'aire du rectangle ?

**Solution :**
- Soit x la demi-largeur du rectangle
- Hauteur : y = √(R² - x²)
- Aire : A(x) = 2x√(R² - x²)
- A'(x) = 2√(R² - x²) + 2x · (-x)/√(R² - x²) = 2(R² - 2x²)/√(R² - x²)
- A'(x) = 0 ⟹ R² - 2x² = 0 ⟹ x = R/√2
- Dimensions optimales : largeur = R√2, hauteur = R/√2

## 7. Exercices d'Entraînement Supplémentaires

### Niveau Avancé

**Exercice 14 :** Calculez la dérivée de f(x) = (sin(x))^(cos(x))

**Exercice 15 :** Trouvez la dérivée de g(x) = ∫[0 à x²] sin(t²) dt

**Exercice 16 :** Calculez lim[x→0] [sin(3x) - 3sin(x)] / x³ en utilisant les dérivées

**Exercice 17 :** Étudiez la fonction f(x) = xe^(-x) : domaine, limites, variations, extrema

## Conseils pour Maîtriser les Dérivées

1. **Mémorisez les dérivées de base**
2. **Pratiquez les règles de calcul régulièrement**
3. **Identifiez le type de fonction avant de dériver**
4. **Vérifiez vos calculs en dérivant le résultat**
5. **Utilisez la règle de la chaîne systématiquement pour les compositions**

## 8. Exemple Concret : Les Dérivées dans la Vie Réelle

### Exemple : La Vitesse d'une Voiture

**Situation :** Vous conduisez une voiture et votre position sur l'autoroute change au fil du temps.

**La fonction :** Si votre position est donnée par s(t) = 2t² + 10t (en mètres, où t est en secondes)

**La dérivée :** s'(t) = 4t + 10

**Signification pratique :**
- **s(t)** = votre position sur la route à l'instant t
- **s'(t)** = votre vitesse instantanée à l'instant t

**Calculs concrets :**
- À t = 0 secondes : vitesse = 4(0) + 10 = 10 m/s
- À t = 5 secondes : vitesse = 4(5) + 10 = 30 m/s
- À t = 10 secondes : vitesse = 4(10) + 10 = 50 m/s

**Ce que cela nous dit :**
1. Vous accélérez constamment (la vitesse augmente de 4 m/s chaque seconde)
2. Votre accélération est constante : s''(t) = 4 m/s²

### Autres Exemples Quotidiens

- **Économie :** Le coût marginal (dérivée du coût total) pour produire une unité supplémentaire
- **Médecine :** La vitesse de croissance d'une tumeur ou la vitesse d'élimination d'un médicament
- **Météo :** La vitesse de changement de la température ou de la pression atmosphérique
- **Finance :** La sensibilité du prix d'une action aux variations du marché

**La dérivée nous donne toujours le taux de changement instantané - c'est son pouvoir dans la vie réelle !**

---

*Ce cours couvre les aspects essentiels des dérivées. La pratique régulière est la clé pour maîtriser ces concepts !*