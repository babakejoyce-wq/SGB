#  SGB — Système de Gestion de Bibliothèque
### Université Excellence · v1.0 · 2025

> Application web fullstack de gestion documentaire universitaire — emprunts, retours, pénalités, catalogue, membres, statistiques.

---

##  Aperçu

**SGB** est une application de gestion de bibliothèque conçue pour l'Université Excellence (Lomé, Togo). Elle remplace les fiches papier par une interface moderne, rapide et 100% traçable.

Elle couvre l'intégralité du cycle documentaire :
de l'inscription d'un membre jusqu'au calcul automatique des pénalités de retard, en passant par la gestion des réservations et la génération de rapports.

---

##  Fonctionnalités

| Module | Description |
|---|---|
| 🔐 **Authentification** | Login par profil (Bibliothécaire / Administrateur / Étudiant) |
| 📖 **Emprunts** | Enregistrement rapide, auto-remplissage par N° étudiant et ISBN |
| 🔄 **Retours** | Validation du retour, détection automatique des retards |
| 📚 **Catalogue** | Recherche plein texte, filtres multi-critères, statut en temps réel |
| 👥 **Membres** | Gestion complète des profils, rôles, quotas et statuts |
| 🔖 **Réservations** | File d'attente numérotée avec attribution en un clic |
| 💰 **Pénalités** | Calculateur interactif, barème configurable par tranche, encaissement |
| 📊 **Statistiques** | Graphiques d'activité, top livres, analyse par filière |
| 🔔 **Alertes** | Retards critiques, rappels automatiques J−2, notifications en temps réel |
| ⚙️ **Paramètres** | Configuration système, durées d'emprunt, sauvegarde, toggles |

---

##  Structure du projet

```
sgb/
├── index.html          # Page d'accueil publique (landing page animée)
├── app.html            # Application principale (SPA fullstack)
└── README.md
```

> Le projet est entièrement **frontend** (HTML / CSS / JavaScript vanilla).  
> Aucune dépendance npm. Aucun framework. Aucune installation requise.

---

##  Lancer le projet

### Option 1 — Ouvrir directement

```bash
# Cloner le dépôt
git clone https://github.com/babakejoyce-wq/sgb.git
cd sgb

# Ouvrir index.html dans votre navigateur
open index.html        # macOS
start index.html       # Windows
xdg-open index.html    # Linux
```

### Option 2 — Serveur local (recommandé)

```bash
# Avec Python
python -m http.server 8000

# Avec Node.js / npx
npx serve .

# Puis ouvrir
http://localhost:8000
```

### Option 3 — Déploiement Vercel (recommandé pour la mise en ligne)

```bash
npm i -g vercel
vercel
```

---

##  Stack technique

| Technologie | Usage |
|---|---|
| **HTML5** | Structure sémantique, accessibilité |
| **CSS3** | Variables custom, animations, Grid, Flexbox, responsive |
| **JavaScript ES6+** | Logique métier, DOM, interactions, données |
| **Font Awesome 6** | Iconographie (CDN) |
| **Google Fonts** | Inter + Syne (CDN) |

Aucun framework JavaScript. Aucune dépendance externe installée localement.

---

##  Profils utilisateurs

| Profil | Identifiant démo | Accès |
|---|---|---|
| **Bibliothécaire** | `marie.dupont` | Emprunts, retours, pénalités, catalogue, membres |
| **Administrateur** | `admin` | Tout + paramètres système, rapports globaux |
| **Étudiant** | `koffi.amouzou` | Catalogue, historique personnel, réservations |

> En mode démo, tous les identifiants acceptent n'importe quel mot de passe.

---

##  Design system

```
Palette :
  --ink      #0B0F1A   Fond principal
  --bg2      #111828   Fond secondaire (sidebar, cards)
  --blue     #1A6BF5   Couleur principale (actions, focus)
  --cyan     #00C9A7   Succès / disponibilité
  --amber    #F5A623   Avertissements / pénalités
  --red      #E8453C   Erreurs / retards critiques

Typographie :
  Syne 700–800         Titres, chiffres, logo
  Inter 400–700        Corps, labels, navigation
```

---

## 📸 Captures d'écran

| Page d'accueil | Tableau de bord | Pénalités |
|---|---|---|
| *(landing animée, particules canvas, prévisualisation browser)* | *(stats, emprunts récents, mini-graphique)* | *(calculateur + barème configurable)* |

---

## Roadmap

- [ ] Connexion base de données MySQL (PHP / Laravel)
- [ ] API REST complète (CRUD livres, membres, emprunts)
- [ ] Scan QR code natif (caméra)
- [ ] Export PDF des rapports (jsPDF)
- [ ] Notifications email (SMTP)
- [ ] Mode PWA (Progressive Web App)
- [ ] Multilangue FR / EN

---

##  Auteure

**Joyce Babake** (Sky)
Étudiante en Licence Professionnelle Développement Web — Lomé, Togo
Freelance · Star's Sky — *Oser l'infini*

- 🌐 Portfolio : [portfolio-amber-delta-2oudxboyr8.vercel.app](https://portfolio-amber-delta-2oudxboyr8.vercel.app)
- 🐙 GitHub : [@babakejoyce-wq](https://github.com/babakejoyce-wq)

---

## 📄 Licence

Ce projet a été développé dans le cadre d'un cahier des charges académique pour l'Université Excellence.
Usage éducatif et portfolio.

---

<div align="center">
  Made with ❤️ in Lomé, Togo 🇹🇬
</div>
