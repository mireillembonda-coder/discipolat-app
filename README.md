# Discipolat

Suivi des disciples : inscription, présences aux programmes, suivi hebdomadaire, statuts, espace superviseur.

## Comment c'est construit

| Partie | Fichiers | Où elle tourne |
|---|---|---|
| **Coquille installable** (icône sur le téléphone, ouverture hors ligne) | `index.html`, `classique.html`, `sw.js`, `manifest.webmanifest`, `icons/` | GitHub Pages : https://mireillembonda-coder.github.io/discipolat-app/ |
| **Application** (écrans et logique) | `discipolat/*.gs`, `discipolat/Index.html` | Google Apps Script, données dans un Google Sheet |

L'ancienne version (dépôt `discipolat`) renvoyait vers Vercel ; celle-ci reste sur GitHub Pages.

**Attention :** `github.io` est bloqué chez certains opérateurs mobiles. Si un disciple n'arrive pas à ouvrir l'application, c'est la première chose à vérifier (essayer en Wi-Fi ou avec un autre opérateur).

## Mettre à jour

- **Coquille** : chaque modification de `main` est publiée sur GitHub Pages par `.github/workflows/pages.yml`.
- **Application Apps Script** : `ADRESSE_PAGE` (dans `Connexion.gs`) pointe vers l'adresse GitHub Pages ci-dessus. Copier les fichiers de `discipolat/` dans le projet Apps Script, puis **Déployer → Gérer les déploiements → crayon → Nouvelle version** (ne pas créer un nouveau déploiement : l'adresse changerait).

## Historique

Ce dépôt reprend, avec leur historique, les fichiers de Discipolat du dépôt `mireillembonda-coder/discipolat` (branche `gh-pages`), sans les autres applications qui y étaient rangées.
