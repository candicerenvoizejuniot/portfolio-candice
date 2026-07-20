# Directives de Développement & Guide Agent - Portfolio Candice Renvoizé--Juniot (IRIONA)

Bienvenue. Ce fichier définit les règles de développement, les standards de conception visuelle et les procédures d'assurance qualité applicables au projet de portfolio digital de Candice Renvoizé--Juniot.

## Contexte, Identité & Parcours (CV)

- **Nom** : Candice Renvoizé--Juniot
- **Titre / Rôle** : Product Designer & Future Chef de Projet Digital (Formation 2024-2027 chez Digital Campus).
- **Vision & Profil** : Curieuse et passionnée par l'UX/UI, elle analyse et optimise les interfaces pour concevoir des expériences numériques utiles, simples et centrées sur l'humain, avec une volonté forte d'intégrer l'Intelligence Artificielle (IA) dans son processus créatif pour proposer des solutions accessibles.
- **Expériences clés à valoriser** :
  - **TOKIZ Digital** (UX/UI Designer) : Conception & réalisation de 7+ maquettes d'interfaces clients, intégration Notion, newsletters Brevo/Infomaniak.
  - **MYSOA** (Communication Marketing) : Audit Web (UI/UX, SEO, performance, scalabilité), charte graphique, logo, visuels RS.
  - **Olystia Conseil** (Communication Marketing) : Mockups d'étiquettes de vin, refonte du site Graphico, maquette Shop in Bordeaux.
  - **Galileo Global Education** (Communication Graphique) : Chemin de fer, maquette magazine, illustrations vectorielles.
- **Stack & Outils d'Expertise** : Figma, Illustrator, Photoshop, InDesign, HTML5 / CSS3.
- **Contact & Réseaux** :
  - Email : `candice.renvoizejuniot.t@gmail.com`
  - Téléphone : `07 67 10 56 92`
  - Portfolio actuel : `https://portfolio-candice-rj.vercel.app/`
  - LinkedIn : `linkedin.com/in/candice-rj/`
- **Objectif majeur du site** : Présentation interactive et captivante de 5 maquettes web clients réalisées sur Figma et Framer.

---

## 1. Principes Architecturaux

- **HTML5 Sémantique Exclusif** :
  - Structurer rigoureusement les pages avec des balises sémantiques (`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<aside>`, `<footer>`).
  - Proscrire l'usage abusif de `<div>` génériques lorsque des balises sémantiques sont adaptées.
- **Vanilla CSS3 Uniquement** :
  - Utiliser du CSS natif avec Variables CSS (Custom Properties) fondées sur le Design System de la charte IRIONA.
  - Définir une architecture modulaire et propre (`index.css` / variables / composants).
- **Interdiction Stricte des Frameworks Utilitaires** :
  - Aucun framework utilitaire CSS (Tailwind CSS, Bootstrap, Bulma, Tachyons, etc.) ne doit être installé ou importé.
  - Tout le code de style doit être sur-mesure, maîtrisé et personnalisable.

---

## 2. Directives Esthétiques (Inspiration Marathon x Couleurs IRIONA)

- **Palette de Couleurs Personnelles (Prioritaire & Exclusive)** :
  - `--color-purple-main`: `#693A8E` (Pantone 7678 C - Violet IRIONA principal)
  - `--color-lavender`: `#CFBDDE` (Pantone 263 C - Soft Lavender secondaires & fonds doux)
  - `--color-black`: `#010101` (Pantone Black 6 C - Dark Base & fonds sombres HUD)
  - `--color-white`: `#FCF8FC` (Pantone 663 C - Texte principal & éléments clairs)
  - `--color-blue-accent`: `#AEC2E6` (Pantone 658 C - Ice Blue pour les badges et états)
  - `--gradient-gold`: `linear-gradient(135deg, #8c6828 0%, #b88d40 50%, #6e4e1a 100%)` (Effet Pantone 871C Or)
- **Style Visuel & Expérience UX (Inspiration Majeure de marathonthegame.com)** :
  - **Layout & Structure Brutaliste HUD** : Grilles d'information asymétriques, sections sous forme de blocs d'interface technique, métadonnées verticales, bordures fines franches.
  - **Détails HUD Tech** : Marqueurs de coin (`+`, `[ ]`, `< >`), puces système (`RUN/`, `INIT/`, `SYS//PROJECT_01`), bandes de statut et micro-textes d'identification.
  - **Intégration SVG Sur-Mesure** : Emplacement privilégié pour les pictogrammes acérés et les illustrations vectorielles personnalisées de la cliente.
- **Typographies Google Fonts Impactantes** :
  - Titres & En-têtes : Polices à forte personnalité géométrique et ultra-wide (*Syne*, *Space Grotesk*, *Cabinet Grotesk*).
  - Étiquettes HUD & Code : Polices monospacées techniques (*Space Mono*, *JetBrains Mono*).
  - Corps de texte : Polices modernes et épurées (*Inter*, *Plus Jakarta Sans*).
- **Micro-Animations Fluides & Réactives** :
  - Survol dynamique des éléments : Inversion de contraste (passage du fond noir `#010101` au violet `#693A8E` ou lavande `#CFBDDE`), transitions fluides (`cubic-bezier(0.16, 1, 0.3, 1)`).
  - Animations d'apparition type HUD (révélation progressive des données du CV et des 5 projets maquettes).

---

## 3. Boucles de Vérification & Assurance Qualité

- **Plan d'Implémentation Systématique** :
  - L'agent doit **toujours** générer un Plan d'Implémentation détaillé sous forme d'Artéfact avant de réaliser la moindre modification de code dans le portfolio.
  - Aucune modification de code ne doit être exécutée sans l'accord formel préalable de l'utilisateur.
- **Validation d'Accessibilité (A11y) Obligatoire** :
  - Vérifier systématiquement que le HTML produit respecte les normes WAI-ARIA et WCAG 2.1 (niveau AA).
  - Assurer un rapport de contraste parfait entre les teintes IRIONA (violet, lavande, blanc, noir, bleu) pour une lisibilité irréprochable.
  - Garantir une navigation complète au clavier et la présence des attributs indispensables (`alt` informatifs pour les visuels de maquettes Figma/Framer et SVG, `aria-label` pour les composants UI/HUD).
