# Prestige Immobilier — Abidjan

Site vitrine pour une agence immobilière de luxe basée à Cocody, Abidjan (Côte d'Ivoire).

## Structure du projet

```
immo-demo.html          # Fichier unique — tout le site (HTML + CSS + JS)
virtuelle-360.jpg/      # Dossier contenant les images panoramiques 360°
  salon-360.jpg
  chambre-360.jpg
  cuisine-360.jpg
  piscine-360.jpg
  terasse-360.jpg
Gemini_Generated_Image_*.png   # Images générées (visuels biens)
1776278040368-*.mp4            # Vidéo de présentation
```

## Technologies

- HTML/CSS/JS pur — pas de framework, pas de build tool
- **Pannellum** (`cdn.jsdelivr.net/npm/pannellum@2.5.6`) pour la visite virtuelle 360°
- **Google Fonts** : Cormorant Garamond (serif) + Outfit (sans-serif)

## Fonctionnalités clés

- Navigation fixe avec effet scroll
- Hero plein écran avec stats animées
- Barre de recherche (achat/location/investissement)
- Grille de biens immobiliers avec filtres
- Visite virtuelle 360° en modal (5 scènes : salon, chambre, cuisine, piscine, terrasse)
- Section équipe, financement, formulaire de contact
- Footer complet

## Visite 360° (Pannellum)

Les scènes sont configurées dans l'objet `config360` (fin du fichier JS).
Chaque scène référence une image dans `./virtuelle-360.jpg/<nom>-360.jpg`.
Les hotspots permettent la navigation entre scènes.

## Conventions

- CSS en variables `:root` (couleurs `--gold`, `--cream`, `--dark`, etc.)
- Classes utilitaires : `.fade-up`, `.eyebrow`, `.sec-title`, `.btn-gold`, `.btn-ghost`
- Responsive géré par media queries (breakpoints à 900px et 600px)
- Tout est dans un seul fichier `immo-demo.html` — ne pas fragmenter sans raison
