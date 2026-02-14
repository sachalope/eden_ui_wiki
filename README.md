# EDEN UI EDITOR - Documentation

Site web de documentation pour l'éditeur EDEN UI.

## 📂 Structure du site

```
eden_ui_docs/
├── index.html           # Page d'accueil
├── animations.html      # Documentation des animations
├── composants.html      # Types d'éléments (Frame, Sprite, Button, Text)
├── proprietes.html      # Propriétés des éléments
├── editeur.html         # Guide de l'éditeur
├── actions.html         # Actions et événements
├── styles.css           # Styles globaux
└── README.md           # Ce fichier
```

## 🚀 Utilisation

### Ouvrir localement

1. Ouvrez simplement `index.html` dans votre navigateur
2. La navigation entre les pages se fait via le menu latéral gauche
3. Aucun serveur web requis, tout fonctionne en local

### Déployer en ligne

Pour héberger sur un serveur web :

1. Uploadez tous les fichiers dans un dossier
2. Configurez votre serveur pour servir des fichiers HTML statiques
3. L'URL d'accès sera : `http://votre-domaine.com/index.html`

### Intégration dans un projet

Vous pouvez intégrer cette documentation directement dans votre addon :

1. Créez un dossier `html/` dans votre addon
2. Copiez tous les fichiers dedans
3. Utilisez un panel HTML pour afficher la documentation en jeu

## 📚 Contenu de la documentation

### 🎬 Animations
- **Presets d'animation** : Fade In/Out, Scale Pop, Slide Up, Hover Pulse, Color Pulse, Rotate
- **Types d'animation** : Fade, Move, Scale, Rotate, Color Pulse
- **Triggers** : OnShow, OnHover, OnClick, Loop
- **Easing** : Linear, InQuad, OutQuad, InOutQuad
- **Composition d'animations** : Animations additives et overwrite
- **Propagation parent-enfant**

### 🧩 Composants
- **Frame** : Conteneur principal
- **Sprite** : Images et matériaux
- **Button** : Boutons interactifs avec états (normal, hover, pressed, disabled)
- **Text** : Texte stylisé avec polices Google Fonts
- **Hiérarchie** : Système parent-enfant
- **Z-Order** : Gestion de la profondeur d'affichage

### ⚙️ Propriétés
- **Position et Taille** : X, Y, W, H
- **Ancrage** : 9 points d'ancrage (TopLeft, Center, etc.)
- **Z-Order** : Ordre d'affichage
- **Couleur et Transparence** : RGB + Alpha
- **Transformations** : Rotation, Scale
- **Matériaux** : Gestion des chemins et Material Picker
- **Visibilité** : Hidden et Clipping

### ✏️ Éditeur
- **Interface** : Outliner, Canvas, Propriétés
- **Sélection** : Simple et multi-sélection
- **Raccourcis clavier** : Ctrl+Z, Ctrl+D, Delete, Flèches, etc.
- **Gizmos** : Déplacement et redimensionnement
- **Zoom et Pan** : Navigation dans le canvas
- **Système de pages** : Multi-pages avec navigation
- **Save et Export** : JSON (projet) et Lua (code)

### ⚡ Actions
- **Types d'actions** : Aucune, Fermer le menu, Naviguer vers page, Code custom
- **Événements** : États des boutons et callbacks OnClick
- **Combinaisons** : Actions + Animations
- **Inherit Hover** : Texte réactif sur boutons
- **Export** : Structure du code et variable 'u'

## 🎨 Design

Le wiki utilise un design sobre et professionnel :
- **Palette de couleurs** : Bleu (#3498db) et gris (#2c3e50)
- **Navigation** : Sidebar fixe à gauche
- **Responsive** : S'adapte aux écrans mobiles, tablettes et desktop
- **Typography** : Police Segoe UI pour une lisibilité optimale
- **Cards** : Organisation en cartes pour structurer l'information

## 🔧 Personnalisation

### Modifier les couleurs

Éditez le fichier `styles.css` et changez les variables CSS dans `:root` :

```css
:root {
    --primary-color: #2c3e50;      /* Couleur principale */
    --accent-color: #3498db;       /* Couleur d'accent */
    --bg-color: #ecf0f1;          /* Fond de page */
    --card-bg: #ffffff;           /* Fond des cartes */
    /* ... autres variables ... */
}
```

### Ajouter une nouvelle page

1. Créez un fichier HTML (ex: `nouvelle-page.html`)
2. Copiez la structure d'une page existante
3. Modifiez le contenu
4. Ajoutez le lien dans la sidebar de toutes les pages :

```html
<li><a href="nouvelle-page.html">Nouvelle Page</a></li>
```

## 📝 Notes

- Tous les fichiers sont des pages HTML statiques (pas de backend requis)
- Les styles sont centralisés dans `styles.css`
- La navigation est manuelle (pas de JavaScript de routing)
- Les exemples de code utilisent la syntaxe Lua pour Garry's Mod

## 📄 License

Documentation créée pour EDEN UI EDITOR © 2026

---

**Auteur** : Documentation générée pour le système EDEN UI Editor V2  
**Date** : Février 2026  
**Version** : 1.0
