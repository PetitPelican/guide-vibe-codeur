# Décisions d'architecture — Guide du Vibe Codeur
_Dernière mise à jour : 2026-06-20_

> Ce fichier répond au **pourquoi**. Pour le quoi (stack actuelle, couches, flux), voir `architecture.md`.

## Décisions clés

### Migration vers Astro
**Pourquoi :** Meilleure maintenabilité qu'un HTML monolithique — composants réutilisables, build optimisé, intégration native avec Tailwind et Vercel.

### Site 100% statique (SSG)
**Pourquoi :** Pas de backend nécessaire — contenu éditorial pur, performance maximale, hébergement gratuit sur Vercel.

### Stack — choix initiaux
| Outil | Décision |
|---|---|
| Astro | Framework SSG — composants + zero JS par défaut |
| Tailwind CSS | Styling utilitaire — déjà utilisé dans le HTML source |
| Vercel | Déploiement — intégration git automatique, CDN global |
