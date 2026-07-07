# ODK-Retail-Audit
Questionnaire de collecte de données terrain (XLSForm/ODK) pour un audit retail en Côte d'Ivoire : disponibilité produit, prix, merchandising et perception vs concurrence.

# Retail Audit Nivea CIV — Formulaire de collecte ODK (XLSForm)

## Contexte
Formulaire de collecte de données terrain conçu pour un audit retail de la marque
Nivea en Côte d'Ivoire, dans le cadre d'un projet de suivi de la présence en points
de vente face à la concurrence (Mixa, Dove, Vaseline, Rexona, Axe, Narta, OE).

## Objectif
Mesurer, point de vente par point de vente : la disponibilité produit, le
positionnement prix, la visibilité merchandising et la perception de la marque,
pour alimenter les décisions commerciales et marketing.

## Structure du questionnaire (XLSForm)
- **Section 1 — Identification du point de vente** : agent recenseur, nom du PDV,
  marché, géolocalisation GPS, type et taille du point de vente, contact,
  source d'approvisionnement Nivea
- **Section 2 — Disponibilité produits (Nivea & concurrence)**, par catégorie :
  - Body Lotion (Nivea, Mixa, Dove, Vaseline)
  - Roll-ons (Nivea, Rexona, Dove, Axe, Narta, OE)
  - Sprays (Nivea, Rexona, Dove, Axe, Narta, OE)
  - Pour chaque marque : présence (oui/non), prix minimum, prix maximum
- **Section 3 — Merchandising / Visibilité** : exposition en avant, présence de PLV,
  animations/promotions
- **Section 4 — Perception & demande** : produit le plus demandé, marque concurrente
  la plus vendue, perception Nivea vs concurrents
- **Section 5 — Commentaires libres** : observations terrain

## Stack technique
`XLSForm` · `ODK Collect` — formulaire structuré (survey / choices / settings),
compatible collecte mobile hors-ligne avec géolocalisation.

## Cas d'usage
Alimente un pipeline de collecte terrain → nettoyage/traitement (R/Python) →
dashboard décisionnel (couverture réseau, part de linéaire, écarts de prix par zone).
