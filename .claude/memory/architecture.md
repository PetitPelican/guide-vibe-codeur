# Architecture — Guide du Vibe Codeur
_Dernière mise à jour : 2026-06-20_

## Vue d'ensemble

Site statique Astro — landing page éducative sur le vibe coding, déployée sur Vercel.

## Couches

### Frontend
- Astro (SSG) — pages et composants
- Tailwind CSS — styling
- Google Fonts (Inter, JetBrains Mono) — typographie

### Déploiement
- Vercel — CDN global, déploiement auto sur push git

## Flux

```
src/ (Astro) → build statique → Vercel CDN → utilisateur
```

## Structure cible (après migration)

```
src/
  pages/
    index.astro        # page principale
  components/
    Hero.astro
    Section.astro
    NavSidebar.astro
    CodeBox.astro
    ...
  styles/
    global.css
public/
  fonts/
  images/
```

## Environnements

| Env | URL | Notes |
|---|---|---|
| Dev | localhost:4321 | `astro dev` |
| Prod | À configurer sur Vercel | Deploy auto sur push main |
