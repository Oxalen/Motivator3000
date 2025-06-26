# Guide d’installation de LM Studio et d’un LLM local  
**Public cible : Enseignants**

---

## Prérequis

Avant de commencer, assurez-vous de disposer des éléments suivants :

- Un ordinateur sous Windows, macOS ou Linux
- Au moins 16 Go de RAM (32 Go recommandés)
- De l’espace disque disponible (entre 10 et 20 Go selon le modèle choisi)
- Une connexion internet pour télécharger les outils et modèles

---

## 1. Installer LM Studio

### Étape 1 : Télécharger LM Studio

1. Rendez-vous sur le site officiel : [https://lmstudio.ai](https://lmstudio.ai)
2. Cliquez sur le bouton **Download**
3. Choisissez la version correspondant à votre système d’exploitation :
   - Windows (.exe)
   - macOS (.dmg)
   - Linux (.AppImage)

### Étape 2 : Installer LM Studio

- **Sous Windows** : Double-cliquez sur le fichier `.exe` et suivez les instructions d’installation.
- **Sous macOS** : Ouvrez le fichier `.dmg`, puis glissez l’icône LM Studio dans le dossier `Applications`.
- **Sous Linux** : Rendez le fichier `.AppImage` exécutable (clic droit > Propriétés > Permissions > Autoriser l’exécution), puis double-cliquez pour lancer LM Studio.

---

## 2. Télécharger et installer un LLM local

### Étape 1 : Lancer LM Studio

Ouvrez LM Studio installé sur votre machine.

### Étape 2 : Accéder à la section "Models"

Dans l’interface de LM Studio :
1. Allez dans l’onglet **"Models"**
2. Cliquez sur **"Download Models"** pour accéder à la bibliothèque de modèles

### Étape 3 : Choisir un modèle LLM local

Voici quelques modèles recommandés :

- **Mistral 7B** (léger et performant)
- **LLaMA 3** (selon disponibilité)
- **Phi-2** (plus petit, pour des machines avec peu de RAM)

**Conseils :**
- Privilégier les versions **GGUF** (optimisées pour LM Studio)
- Choisissez la version **Q4_0** ou **Q5_1** si vous avez 16 Go de RAM, **Q6 ou Q8** si vous avez plus

### Étape 4 : Télécharger le modèle

1. Cliquez sur le modèle choisi
2. Cliquez sur **Download**  
Le téléchargement peut prendre plusieurs minutes.

---

## 3. Utiliser le modèle en local

### Étape 1 : Lancer un chat

Une fois le modèle téléchargé :
1. Allez dans l’onglet **Chat**
2. Sélectionnez le modèle téléchargé dans le menu déroulant
3. Cliquez sur **Start chat** pour commencer à discuter avec l’IA localement

### Étape 2 : Paramétrage (optionnel)

Vous pouvez ajuster :
- La température (niveau de créativité)
- Le maximum de tokens (longueur de la réponse)
- Le système prompt (contexte initial)

---

## 4. Bonnes pratiques

- Fermez les autres applications pour libérer de la mémoire
- Ne téléchargez qu’un ou deux modèles à la fois
- Utilisez des prompts clairs et contextualisés

---
