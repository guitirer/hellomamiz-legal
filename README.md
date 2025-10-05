# Pages légales HelloMamiz (hébergement GitHub Pages)

Ce dossier contient deux pages HTML statiques :
- `privacy.html` : politique de confidentialité alignée sur le contenu affiché dans l’application (Profil &gt; Confidentialité).
- `support.html` : page de contact/support avec renvoi vers le centre d’aide in-app.

## Déploiement via GitHub Pages

1. **Créer un dépôt GitHub** (ex. `hellomamiz-legal`).
2. Copier le dossier `AppStore/web/` dans le dépôt et pousser :
   ```bash
   git clone git@github.com:ton-compte/hellomamiz-legal.git
   cd hellomamiz-legal
   cp -R ../AppStore/web/* .
   git add .
   git commit -m "Ajout des pages légales"
   git push origin main
   ```
3. Dans GitHub, ouvrir **Settings &gt; Pages** :
   - Source : choisir branche `main` et dossier `/ (root)`.
   - Enregistrer. L’URL publique sera du type `https://ton-compte.github.io/hellomamiz-legal/`.
4. Vérifier :
   - Politique de confidentialité : `https://.../privacy.html`
   - Support : `https://.../support.html`

## Utilisation dans App Store Connect

- Champ « Privacy Policy URL » : coller l’URL publique de `privacy.html`.
- Champ « Support URL » : coller l’URL publique de `support.html`.

Pense à mettre à jour ces pages si le texte de la politique ou les contacts support changent (cohérence avec l’application et les notes App Store).
