# QR Studio

Générateur de QR code entièrement personnalisable, autonome et 100 % local : un seul fichier HTML, aucune installation, aucun compte, aucune donnée envoyée.

![Exemple de QR code généré avec QR Studio](demo-qr.png)

## Fonctionnalités

**Contenus pris en charge**

- Texte libre (accents, emojis, sauts de ligne)
- Lien ou site web (préfixe `https://` ajouté automatiquement)
- Wi‑Fi (SSID, sécurité WPA/WEP/aucune, réseau masqué)
- Contact — vCard 3.0 (nom, société, fonction, téléphone, e‑mail, site, adresse)
- E‑mail (`mailto:` avec objet et message)
- SMS (`SMSTO:` avec numéro et message)
- Téléphone (`tel:`)
- GPS (`geo:` avec bouton de géolocalisation)

**Apparence**

- Formes des modules : carré, arrondi, points, diamant, feuille
- Formes des yeux : carrés, arrondis, ronds, feuilles
- Remplissage uni, dégradé linéaire ou radial, angle réglable
- Couleur des yeux personnalisée et fond transparent
- 8 palettes prêtes à l'emploi + bouton « Surprise » (style aléatoire)

**Finitions**

- Correction d'erreur L / M / Q / H
- Taille de 256 à 2048 px et marge de 0 à 12 modules
- Logo central (PNG, JPG, SVG, GIF, WebP — 2 Mo max) avec taille, marge intérieure et arrondi
- Légende personnalisable (texte, couleur, taille)

**Exports**

- PNG haute résolution
- SVG vectoriel (modifiable dans Illustrator, Inkscape, Figma…)
- Copie directe dans le presse‑papiers

Les réglages sont conservés automatiquement dans le navigateur via `localStorage`.

## Utilisation

1. Téléchargez `qr-studio.html`.
2. Ouvrez-le dans un navigateur récent (Chrome, Edge, Firefox, Safari).
3. Renseignez le contenu, personnalisez le style, puis exportez.

Aucune connexion réseau n'est nécessaire : la bibliothèque QR est intégrée au fichier.

## Conseils pour un scan fiable

- Gardez des modules sombres sur un fond clair et une marge d'au moins 4 modules.
- Avec un logo, utilisez la correction d'erreur **H**.
- Testez toujours le résultat avec deux téléphones différents, en particulier avec les formes décoratives (Points, Diamant).

## Compatibilité

- Navigateur moderne requis (canvas, `Path2D`, ES2020+).
- La copie dans le presse‑papiers dépend des autorisations du navigateur.
- La géolocalisation dépend de l'autorisation de l'utilisateur.

## Contenu du dépôt

| Fichier | Rôle |
| --- | --- |
| `qr-studio.html` | L'application complète (HTML + CSS + JavaScript + bibliothèque QR) |
| `demo-qr.png` | Exemple de QR code généré |
| `THIRD-PARTY-NOTICES.md` | Licences des bibliothèques intégrées |

## Licence

Projet privé — © 2026. Tous droits réservés.

La bibliothèque intégrée `qrcode-generator` est distribuée sous licence MIT (voir `THIRD-PARTY-NOTICES.md`).
