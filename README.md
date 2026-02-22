# Pti-plaisir 🧵

Application web de gestion de boutique pour commerçants de tissu et mode.
Conçue pour être légère, rapide et utilisable depuis n'importe quel appareil.

## Aperçu

Pti-plaisir est une PWA mono-fichier qui centralise les opérations quotidiennes d'une boutique :
ventes, clients, stock tissu et reçus PDF — le tout synchronisé en temps réel via Supabase.

## Fonctionnalités

- **Authentification** — Login multi-vendeurs sécurisé (Supabase Auth)
- **Tableau de bord** — Chiffre d'affaires jour / semaine / mois / année
- **Ventes & reçus** — Génération de reçus PDF détaillés ou simplifiés (jsPDF)
- **Crédits clients** — Suivi des dettes avec barre de progression de remboursement
- **Stock tissu** — Gestion par article avec alertes de rupture (rouge / orange / vert)
- **PWA** — Installable sur mobile et desktop, fonctionne hors ligne grâce au service worker

## Stack technique

| Couche | Technologie |
|--------|------------|
| Frontend | HTML · CSS · JavaScript (vanilla) |
| Backend / Auth | [Supabase](https://supabase.com) (PostgreSQL + Auth) |
| PDF | [jsPDF](https://github.com/parallax/jsPDF) |
| Polices | Cormorant Garamond · Outfit (Google Fonts) |
| Déploiement | GitHub Pages |

## Structure du projet

```
pti-plaisir/
├── index.html      # Application complète (UI + logique)
├── manifest.json   # Configuration PWA
├── sw.js           # Service worker (cache hors-ligne)
└── README.md
```

## Installation locale

```bash
git clone https://github.com/MariamDouamba/pti-plaisir.git
cd pti-plaisir
```

Ouvrez ensuite `index.html` avec un serveur local (ex. Live Server dans VS Code).

> **Note** : l'application nécessite une connexion Supabase configurée pour que l'auth et la base de données fonctionnent.

## Déploiement

Le projet est hébergé sur **GitHub Pages** à l'adresse :
`https://mariamDouamba.github.io/pti-plaisir/`

## Auteur

Mariam Douamba

## Licence

MIT
