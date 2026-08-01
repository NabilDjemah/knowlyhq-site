# Bébé dort enfin — Page de vente

Fichiers statiques, déployables directement sur **GitHub Pages** (aucun build requis).

---

## Avant de mettre en ligne — 5 choses à faire

### 1. PRODUCT_ID Payhip
Remplace **toutes** les occurrences de `PRODUCT_ID` dans `index.html` par ton vrai ID produit.  
Où le trouver : Payhip → ton produit → **Share & Embed** → « Buy Button ».

### 2. Date limite de l'offre
Remplace `[DATE]` dans `index.html` par une vraie date (ex. `15 juin 2025`).  
Respecte cette date : passe le prix à 27 $ à l'échéance.

### 3. Photo de Marie
- Ajoute `assets/photo-marie.jpg` (vraie photo, format carré recommandé).
- Dans `index.html`, décommente la balise `<img>` dans la section **Marie** et supprime le `.photo-circle`.

### 4. Mockup couverture
- Copie `Ebook Creation/Mockup/mockup-3d.png` → `assets/mockup-3d.png`.
- Dans `index.html`, décommente la balise `<img>` dans la section **Hero** et supprime `.img-placeholder`.

### 5. Pages légales & infos vendeur
- Remplace `[Nom légal / entreprise]`, `[Adresse postale]`, `[courriel de contact]` dans les 4 fichiers HTML.
- Remplace `[DATE]` dans `remboursement.html`, `confidentialite.html`, `conditions.html`.
- ⚠️ Fais valider ces pages par un professionnel du droit avant publication.

---

## Ligne « vérifié par un professionnel »
Elle est **commentée** dans `index.html` (3 endroits).  
Ne l'activer que si un professionnel a réellement relu le guide — obligation légale.

## Témoignages
Les blocs `[EXEMPLE À REMPLACER]` sont **fictifs** et doivent être remplacés par de vrais avis avant publication. Publier de faux avis est illégal (Loi sur la concurrence — Canada).

---

## Structure des fichiers

```
Page Vente/
├── index.html            ← page de vente principale
├── remboursement.html    ← politique de remboursement
├── confidentialite.html  ← politique de confidentialité
├── conditions.html       ← conditions de vente et licence
├── README.md             ← ce fichier
└── assets/
    ├── mockup-3d.png     ← à copier depuis Ebook Creation/Mockup/
    └── photo-marie.jpg   ← à ajouter
```

## Déploiement GitHub Pages
1. Crée un repo GitHub (ou utilise un existant).
2. Dépose tous ces fichiers à la racine (ou dans un sous-dossier `/docs`).
3. Paramètres du repo → **Pages** → Source : `main` / `root` (ou `/docs`).
4. L'URL sera `https://[username].github.io/[repo]/`.
