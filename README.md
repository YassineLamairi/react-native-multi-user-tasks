# react-native-multi-user-tasks
Application mobile de gestion de tâches multi-listes développée avec React Native (Expo). Gestion d'authentification, navigation par pile et consommation d'API REST.
# 📱 Gestionnaire de Tâches Mobile - React Native

Ce projet est une application mobile complète de gestion de tâches (Todo List) développée avec **React Native** et l'écosystème **Expo**.

L'application permet aux utilisateurs de créer plusieurs listes de tâches, de gérer les éléments à faire, et intègre un système d'authentification complet communiquant avec une API distante.

## 🚀 Fonctionnalités Clés

* **Authentification :** Inscription (Sign Up) et Connexion (Sign In) via API (Tokens).
* **Multi-Listes :** Création, modification et suppression de listes de tâches (ex: "Travail", "Courses").
* **Gestion des Tâches :** Ajout d'items dans une liste, marquage comme "fait", suppression.
* **Navigation Fluide :** Navigation par pile (Stack Navigation) entre l'accueil, les listes et les détails.
* **Interface Réactive :** Utilisation de composants natifs et gestion des inputs clavier.

## 🏗️ Architecture Technique

Le projet suit les bonnes pratiques du développement mobile moderne :

### 1. State Management (Gestion d'État)
Utilisation de **React Context API** (`TokenContext`) pour gérer l'état global de l'application (session utilisateur, token d'authentification) sans "prop drilling".

### 2. Navigation
Implémentation de **React Navigation** avec un `NavigationContainer` et un `Stack.Navigator` pour gérer le flux :
* `SignIn` -> `Home` -> `TodoLists` -> `TodoItems`.

### 3. Architecture Modulaire
Le code est organisé proprement pour la maintenabilité :
* `screen/` : Les vues principales (écrans).
* `components/` : Composants réutilisables (UI).
* `navigation/` : Configuration du routeur.
* `context/` : Logique de l'état global.
* `js/` : Logique métier et appels API (`fetch`, gestion des tokens).

## 🛠️ Stack Technique
* **Framework :** React Native (Expo SDK).
* **Langage :** JavaScript (ES6+).
* **Navigation :** @react-navigation/native-stack.
* **API :** Fetch API pour la communication backend (GraphQL/REST).
* **Assets :** Gestion des icônes et images adaptatives.

## 📦 Installation et Lancement

### Pré-requis
* Node.js installé.
* Application **Expo Go** sur votre téléphone (ou un émulateur Android/iOS).

### Étapes
1.  **Installation des dépendances :**
    ```bash
    npm install
    ```

2.  **Lancement du serveur de développement :**
    ```bash
    npx expo start
    ```

3.  **Tester :**
    * Scannez le QR Code avec l'application Expo Go (Android) ou l'appareil photo (iOS).
    * Ou appuyez sur `a` pour lancer sur un émulateur Android.

## 👤 Auteur
* **Mohamed Yassine Lamairi**
