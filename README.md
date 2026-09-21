# 🇫🇷 Analyseur Municipales 2026 — Résultats Officiels du 1er Tour

![Version](https://img.shields.io/badge/version-2.0.0-0055A4?style=for-the-badge)
![Statut](https://img.shields.io/badge/statut-actif-EF4135?style=for-the-badge)
![Licence](https://img.shields.io/badge/licence-MIT-white?style=for-the-badge)
![Langue](https://img.shields.io/badge/langue-français-0055A4?style=for-the-badge)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Chart.js](https://img.shields.io/badge/Chart.js-FF6384?style=for-the-badge&logo=chart.js&logoColor=white)
![Open Source](https://img.shields.io/badge/Open%20Source-%E2%9D%A4-EF4135?style=for-the-badge)

> **Outil d'analyse tactique et open-source** pour explorer les résultats officiels du **1er tour des élections municipales 2026** en France. Visualisation par commune, taux de participation, tendances politiques et analyse des reports de voix.

---

## 📊 Aperçu

**Analyseur Municipales 2026** est une application web **100 % client-side** (aucune donnée envoyée à un serveur) permettant d'agréger et de visualiser les résultats électoraux à partir des fichiers CSV officiels publiés sur [data.gouv.fr](https://www.data.gouv.fr).

Idéal pour :
- 🗺️ Les analystes politiques et journalistes
- 📈 Les chercheurs en sciences sociales
- 🏛️ Les collectivités territoriales
- 👥 Les citoyens curieux

---

## ✨ Fonctionnalités

| Fonctionnalité | Description |
|---|---|
| 📥 **Import CSV** | Glisser-déposer ou sélection de fichier (format "Résultats par bureaux de vote") |
| 🔄 **Agrégation automatique** | Consolidation des bureaux de vote par commune (format Wide) |
| 📊 **Visualisation graphique** | Diagrammes en barres interactifs via Chart.js |
| 🔍 **Recherche & tri** | Filtrage par nom, code commune ou département |
| 🏆 **Analyse des résultats** | Vainqueur, score, écart avec le 2ᵉ, nuance politique |
| 📱 **Responsive** | Interface adaptée mobile, tablette et desktop |
| 🎨 **Thème tricolore** | Identité visuelle bleu-blanc-rouge |
| 🔒 **Confidentialité totale** | Traitement 100 % local — aucune donnée transmise |

---

## 🚀 Démo en ligne

👉 **Accéder à l'application** : [https://gunout.github.io/Municipales_France_Analyseur_1er_Tour/](https://github.com/gunout/municipales-analyser)

---

## 🛠️ Installation

### Prérequis

Aucun ! L'application fonctionne directement dans un navigateur moderne.

### Utilisation locale

```bash
# Cloner le dépôt
git clone https://github.com/gunout/municipales-analyser.git

# Accéder au dossier
cd municipales-analyser

# Ouvrir le fichier dans un navigateur
open index.html
# ou double-cliquer sur index.html
```

### Déploiement GitHub Pages

1. Poussez le code sur votre dépôt GitHub
2. Rendez-vous dans `Settings` → `Pages`
3. Sélectionnez la branche `main` et le dossier `/root`
4. L'application est en ligne en quelques minutes

---

## 📂 Format des données

L'application accepte les fichiers CSV officiels du **Ministère de l'Intérieur** :

🔗 [Télécharger les données officielles](https://www.data.gouv.fr/datasets/elections-municipales-2026-resultats-du-premier-tour?resource_id=1428132c-ad5e-437e-a928-7c2a254e40eb)

**Colonnes attendues (détection automatique) :**

| Champ | Colonnes reconnues |
|---|---|
| Code commune | `code commune`, `codcom` |
| Nom commune | `libelle commune`, `nom commune` |
| Code département | `code departement`, `coddep` |
| Inscrits | `inscrits` |
| Votants | `votants` |
| Exprimés | `exprimes` |
| Blancs | `blancs` |
| Nuls | `nuls` |
| Listes (1 à 20) | `libelle de liste N`, `voix N`, `nuance liste N` |

> ✅ Séparateurs supportés : `;`, `,`, `\t` (tabulation)

---

## 🧱 Stack technique

- **HTML5 / CSS3** — Interface responsive et thème tricolore
- **JavaScript Vanilla** — Aucun framework, aucune dépendance lourde
- **Chart.js 3.9.1** — Visualisation des données
- **Google Fonts** — Orbitron & Share Tech Mono

---

## 📁 Structure du projet

```
Municipales_France_Analyseur_1er_Tour/
│
├── index.html          # Application complète (HTML + CSS + JS)
├── preview.png         # Image d'aperçu pour les réseaux sociaux
├── README.md           # Documentation
└── LICENSE             # Licence MIT
```

---

## 🤝 Contribution

Les contributions sont les bienvenues ! Pour proposer une amélioration :

1. **Fork** le projet
2. Créez une branche (`git checkout -b feature/amelioration`)
3. **Commit** vos changements (`git commit -m 'Ajout fonctionnalité X'`)
4. **Push** (`git push origin feature/amelioration`)
5. Ouvrez une **Pull Request**

---

## 📜 Licence

Ce projet est distribué sous licence **MIT** — voir le fichier [LICENSE](LICENSE) pour plus d'informations.

---

## ⚠️ Avertissement

Cette application est un **outil d'analyse à but informatif**. Les données affichées proviennent des sources officielles du **Ministère de l'Intérieur** via [data.gouv.fr](https://www.data.gouv.fr). En cas de divergence, seuls les résultats publiés par les autorités compétentes font foi.

---

## 🙏 Remerciements

- **Ministère de l'Intérieur** — Données officielles
- **data.gouv.fr** — Plateforme open data
- **Chart.js** — Bibliothèque de visualisation
- **La communauté open source** ❤️

---

<div align="center">

**🇫🇷 Fait en France avec ❤️**

![Bleu](https://img.shields.io/badge/-0055A4?style=flat-square)
![Blanc](https://img.shields.io/badge/-FFFFFF?style=flat-square)
![Rouge](https://img.shields.io/badge/-EF4135?style=flat-square)

*République Française — Liberté · Égalité · Fraternité*

</div>

---

<div align="center">

### 🇫🇷 Gunout · 2026

![Made in France](https://img.shields.io/badge/Made_in-France-002395?style=flat-square&labelColor=FFFFFF&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCA5MDAgNjAwIj48cmVjdCB3aWR0aD0iOTAwIiBoZWlnaHQ9IjYwMCIgZmlsbD0iIzAwMjM5NSIvPjxyZWN0IHdpZHRoPSI5MDAiIGhlaWdodD0iNDAwIiB5PSIxMDAiIGZpbGw9IiNmZmYiLz48cmVjdCB3aWR0aD0iOTAwIiBoZWlnaHQ9IjIwMCIgeT0iNDAwIiBmaWxsPSIjZWQyOTM5Ii8+PC9zdmc+)
![GitHub](https://img.shields.io/badge/GitHub-gunout-181717?style=flat-square&logo=github&logoColor=white)
![Year](https://img.shields.io/badge/2026-ED2939?style=flat-square&labelColor=FFFFFF)

<sub>© 2026 <strong>Gunout</strong> — Tous droits réservés.</sub>

</div>
