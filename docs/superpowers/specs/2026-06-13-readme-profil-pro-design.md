# Refonte du profil GitHub — design « simple & pro »

## Objectif

Transformer le README du profil GitHub (`README.md`) en une carte de visite
sobre et professionnelle qui donne envie de contacter Alexandre, en mettant en
avant sa disponibilité **freelance**.

## Contexte

- Le README actuel utilise un thème « Dark Sasuke » (violet/rouge), un ton très
  geek (typing SVG « GPU go brrrrr », « I eat V-Bucks for breakfast »), des
  trophées et un compteur de vues. Direction abandonnée.
- Audience : visibilité générale (carte de visite tous publics).
- Langue : **anglais**.
- Ton : **simple et professionnel**, sans private jokes ni gaming.

## Décisions validées

- Structure retenue : variante « **Polished pro** » — texte structuré + badges
  discrets + carte de stats GitHub.
- Statut **freelance** mis en avant comme déclencheur de contact principal.
- Lien **Malt** ajouté en tête de la section contact.
- Style de badges : `flat-square` (pas `for-the-badge`), accent bleu GitHub
  (`#58a6ff`) sobre.

## Structure du README (de haut en bas)

Tout est centré au minimum nécessaire ; le corps reste aligné à gauche pour la
lisibilité.

1. **En-tête**
   - Nom : `Alexandre Petitjean`
   - Rôle : `Freelance Full Stack Developer · Lyon, France · Python / Django`
   - Badge vert `Available for freelance work` (couleur `#2ea043`).
   - Phrase d'intro :
     « Currently building LLM-powered tools and telecom engineering software
     @ITSolutionsFactory. Open to new freelance missions. »
     (lien `@ITSolutionsFactory` → https://github.com/itsolutionsfactory)

2. **Currently** (liste à puces)
   - 🔭 LLM-powered tooling for telecom engineering
   - 🌱 [react-allauth](https://github.com/alexandre-petitjean/react-allauth) —
     Django AllAuth SDK for React
   - ✍️ Writing at [alexandre-petitjean.fr](https://alexandre-petitjean.fr/)

3. **Tech stack** (badges `flat-square`, sur 2 lignes logiques)
   - Langages / frameworks : Python, Django, TypeScript, React, Flutter
   - Données / infra : PostgreSQL, MariaDB, Docker, Kubernetes

4. **GitHub** (cartes côte à côte, thème `github_dark`, fond `#0d1117`)
   - `github-readme-stats` (stats, `hide=contribs`)
   - `github-readme-stats/top-langs` (layout compact)

5. **Reach me** (badges `flat-square`, dans cet ordre)
   - **Malt** `Hire me` (couleur `#FC5757`, `logo=malt`) →
     https://www.malt.fr/profile/alexandrepetitjean1
   - Website → https://alexandre-petitjean.fr/
   - LinkedIn → https://linkedin.com/in/petitjeana
   - Email → mailto:petitjean.alexandre.pro@gmail.com
   - Stack Overflow → https://stackoverflow.com/users/9580005

## Contraintes techniques

- Conserver le bloc `<div align="center">` pour l'en-tête et le contact, corps
  en markdown standard.
- Badges via `img.shields.io` en `style=flat-square`.
- Cartes de stats via `github-readme-stats.vercel.app`, thème `github_dark`.
- Liens cliquables en markdown (les liens des badges via `[![..](badge)](url)`).
- Pas de section Windows dans d'éventuelles notes ; ici sans objet.

## Éléments supprimés du README actuel

- Banner `capsule-render` Dark Sasuke + footer wave.
- Typing SVG (« GPU go brrrrr », « V-Bucks »…).
- Compteur de vues `komarev`, follow Twitter, trophées `github-profile-trophy`.
- Bloc `class Developer` en Python et image manga `image-readme.jpeg`
  (non réutilisée dans cette direction).
- Animation snake (présente uniquement sur l'ancienne branche).

## Critères de réussite

- Le profil se lit en quelques secondes et paraît crédible / professionnel.
- La disponibilité freelance et le lien Malt sont immédiatement visibles.
- Aucune dépendance cassée ; rendu correct en dark et light mode GitHub.
- Tous les liens (Malt, site, LinkedIn, email, Stack Overflow, react-allauth)
  pointent vers les bonnes destinations.
