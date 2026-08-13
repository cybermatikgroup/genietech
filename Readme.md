# GenieTech — Buzzer & Quiz 2026

Système de buzzer et de gestion de quiz pour la compétition GenieTech.

## Structure

- `index.html` — page d'accueil, liens vers les 3 interfaces
- `equipe.html` — interface équipe (buzzer)
- `ecran.html` — grand écran (projecteur/TV)
- `jury.html` — interface jury (pilotage du jeu)
- `Code.gs` — moteur du jeu (Google Apps Script), branché sur un Google Sheet à 4 onglets : `Equipes`, `Questions`, `EtatJeu`, `Configuration`

## Installation

1. Ouvrir le Google Sheet du projet, coller `Code.gs` dans Extensions > Apps Script.
2. Exécuter `initEtatJeu()` une fois depuis l'éditeur.
3. Déployer comme application web (exécuter en tant que moi, accès à tout le monde), copier l'URL `/exec`.
4. Remplacer `SCRIPT_URL` dans `equipe.html`, `ecran.html` et `jury.html` par cette URL.
5. Servir les fichiers HTML statiquement :

```bash
npm start
```

## Licence

ISC
