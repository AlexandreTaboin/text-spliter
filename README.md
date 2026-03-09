# ✂️ Séparateur de Texte

Un outil web **100% côté client** (aucun serveur requis) permettant de découper du texte long ou des fichiers texte en plusieurs parties, selon une limite de caractères définie.

---

## 📋 Table des matières

- [Aperçu](#aperçu)
- [Fonctionnalités](#fonctionnalités)
- [Installation](#installation)
- [Utilisation](#utilisation)
- [Options](#options)
- [Formats supportés](#formats-supportés)
- [Technologies](#technologies)

---

## 🖼️ Aperçu

Cet outil est idéal pour découper de longs textes afin de les envoyer dans des outils limités en caractères (ChatGPT, SMS, API, formulaires, etc.).  
Il fonctionne entièrement dans le navigateur : **aucune donnée n'est envoyée sur un serveur**.

---

## ✅ Fonctionnalités

- 📝 **Mode texte** : collez directement votre texte dans une zone de saisie avec compteur de caractères en temps réel
- 📁 **Mode fichiers** : glissez-déposez ou sélectionnez plusieurs fichiers simultanément
- ✂️ **Deux modes de découpe** :
  - **Intelligente** : coupe au niveau des espaces ou sauts de ligne pour ne jamais couper un mot en plein milieu
  - **Brute** : coupe exactement à la limite de caractères définie
- 📋 **Copier** chaque partie en un clic dans le presse-papier
- 💾 **Télécharger** chaque partie individuellement en fichier `.txt`
- 🔢 **Compteur de caractères** en temps réel dans le mode texte
- ✅ **Résumé automatique** du nombre de sources traitées et de parties générées
- ⚠️ **Gestion des erreurs** : fichier vide, fichier illisible, aucun contenu
- 🚫 **Dédoublonnage automatique** des fichiers ajoutés (par nom + taille)
- 🗑️ **Suppression individuelle** des fichiers depuis la liste
- 📱 **Interface responsive** adaptée aux mobiles et tablettes
- 🔔 **Toast de notification** lors d'une copie ou d'un téléchargement

---

## 🚀 Installation

Aucune installation requise. C'est un fichier HTML unique, autonome.

1. Téléchargez ou clonez ce dépôt :
   ```bash
   git clone https://github.com/votre-utilisateur/separateur-texte.git
   ```
2. Ouvrez le fichier `index.html` dans votre navigateur :
   ```bash
   cd separateur-texte
   start index.html       # Windows
   open index.html        # macOS
   xdg-open index.html    # Linux
   ```

> ✅ Aucune dépendance, aucun serveur, aucune connexion internet requise.

---

## 📖 Utilisation

### Mode Texte

1. Cliquez sur l'onglet **📝 Texte**
2. Collez votre texte dans la zone de saisie
3. Le compteur de caractères se met à jour automatiquement
4. Configurez vos options (limite et mode de découpe)
5. Cliquez sur **✂️ Découper le texte**
6. Pour chaque partie générée :
   - Cliquez sur **📋 Copier** pour copier le contenu
   - Cliquez sur **💾 .txt** pour télécharger la partie en fichier texte

### Mode Fichiers

1. Cliquez sur l'onglet **📁 Fichiers**
2. Glissez-déposez vos fichiers dans la zone prévue, ou cliquez pour parcourir
3. Les fichiers ajoutés apparaissent dans une liste avec leur nom et taille
4. Supprimez un fichier de la liste en cliquant sur le bouton ✖
5. Configurez vos options (limite et mode de découpe)
6. Cliquez sur **✂️ Découper le texte**
7. Les résultats s'affichent par fichier, avec le nombre de parties et le nombre de caractères par partie

---

## ⚙️ Options

| Option | Description | Valeur par défaut |
|---|---|---|
| **Limite par partie** | Nombre maximum de caractères par partie | `10 000` |
| **Mode Intelligente** | Coupe au dernier espace ou saut de ligne avant la limite | Activé par défaut |
| **Mode Brute** | Coupe exactement à la limite, sans tenir compte des mots | - |

---

## 📂 Formats supportés

| Catégorie | Extensions |
|---|---|
| Texte brut | `.txt`, `.log`, `.md`, `.rtf`, `.csv` |
| Web | `.html`, `.htm`, `.css`, `.js`, `.ts`, `.jsx`, `.tsx`, `.vue`, `.svelte` |
| Données | `.json`, `.xml`, `.yml`, `.yaml`, `.ini`, `.cfg`, `.conf` |
| Programmation | `.py`, `.java`, `.c`, `.cpp`, `.h`, `.php`, `.rb`, `.go`, `.rs`, `.sh`, `.bat`, `.sql` |
| Sous-titres | `.srt`, `.sub`, `.vtt` |
| Autres | `.tex` |

---

## 🗂️ Structure du projet

```
separateur-texte/
│
├── index.html      # Fichier principal (HTML + CSS + JavaScript)
└── README.md       # Documentation du projet
```

> Tout le code (HTML, CSS, JavaScript) est contenu dans un seul fichier `index.html`.

---

## 🛠️ Technologies

- **HTML5** — Structure de la page
- **CSS3** — Mise en forme, animations, responsive design
- **JavaScript (Vanilla ES6+)** — Logique de découpe, gestion des fichiers, interactions
- **FileReader API** — Lecture des fichiers locaux dans le navigateur
- **Clipboard API** — Copie dans le presse-papier
- **Blob + URL API** — Téléchargement des parties en fichier `.txt`

---

## 📄 Licence

Ce projet est sous licence **MIT**. Vous êtes libre de l'utiliser, le modifier et le distribuer.

---

*Fait avec ❤️ — 100% local, 100% privé.*
