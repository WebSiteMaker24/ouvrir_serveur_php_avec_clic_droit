# 📁 Menu contextuel Windows - Outils développeur

Ce script de registre Windows ajoute plusieurs **actions personnalisées au clic droit** dans l’Explorateur de fichiers.  
Il est destiné à améliorer la productivité, notamment pour le développement PHP et le travail sur des dossiers de projet.

L’importation du fichier `.reg` crée de nouvelles entrées dans le menu contextuel, sans modifier le comportement standard de Windows.

---

## ⚙️ Fonctionnalités ajoutées

### 1️⃣ Ouvrir un fichier PHP avec le serveur PHP intégré

**Cible :** fichiers `.php`

**Action :**
- Lance le serveur PHP intégré (`php -S`)
- Démarre sur `localhost:555`
- Le fichier cliqué est utilisé comme point d’entrée

**Utilité :**
- Tester rapidement un script PHP sans configuration Apache/Nginx
- Idéal pour du debug ou des tests rapides

---

### 2️⃣ Ouvrir un serveur PHP depuis un dossier

**Cible :** fichiers `.php` (menu dédié)

**Action :**
- Lance le serveur PHP intégré sur `localhost:555`
- Le serveur s’exécute dans le dossier courant

**Utilité :**
- Servir un projet PHP complet
- Tester un site localement en quelques secondes

---

### 3️⃣ Ouvrir un dossier dans Visual Studio Code

**Cible :** dossiers

**Action :**
- Ouvre le dossier sélectionné directement dans VS Code

**Utilité :**
- Accès rapide à un projet
- Évite la navigation manuelle depuis l’éditeur

---

### 4️⃣ Ouvrir Visual Studio Code depuis l’intérieur d’un dossier

**Cible :** clic droit dans le vide d’un dossier

**Action :**
- Ouvre VS Code dans le dossier courant

**Utilité :**
- Lancer l’éditeur depuis n’importe quel répertoire
- Pratique pour créer ou explorer rapidement un projet

---

### 5️⃣ Afficher l’arborescence complète d’un dossier

**Cible :** dossiers

**Action :**
- Ouvre un terminal
- Affiche l’arborescence complète avec `tree /a /f`

**Utilité :**
- Visualiser la structure d’un projet
- Utile pour l’analyse, la documentation ou le debug

---

### 6️⃣ Copier le chemin complet d’un fichier

**Cible :** tous les fichiers

**Action :**
- Copie le chemin absolu du fichier dans le presse-papiers
- Aucune fenêtre ne reste ouverte

**Utilité :**
- Coller rapidement un chemin dans un terminal, un script ou un éditeur
- Gain de temps, zéro manipulation manuelle

---

## 🛠️ Prérequis

- Windows
- PHP installé et accessible via la variable `PATH`
- Visual Studio Code installé (`code` accessible en ligne de commande)
- Droits administrateur pour importer le registre

---

## 📥 Installation

1. Copier le contenu du script dans un fichier `menu_contextuel.reg`
2. Double-cliquer sur le fichier
3. Confirmer l’ajout au registre Windows
4. Redémarrer l’Explorateur de fichiers si nécessaire

---

## ⚠️ Remarques

- Le script n’écrase aucune clé système existante
- Toutes les actions sont locales
- Aucune dépendance externe n’est ajoutée

---

## 🎯 Objectif

Centraliser des actions simples, explicites et immédiatement utiles directement dans le menu contextuel Windows, avec une logique minimaliste et efficace, pour travailler plus vite sans alourdir l’environnement.
