<h1 align="center">🌐 InfoBroadcaster</h1>
<p align="center"><strong><em>Broadcast your Infos with ease</em></strong></p>

---

[InfoBroadcaster](https://infobroadcaster.netlify.app) est une application web développé sur une stack NodeJS dont **Express** pour le backend, et **React** pour le front qui permet de résumer automatiquement les informations d'un article en lui fournissant l'url.

Cette application permet également de partager les informations résumées dans des bulles [Rainbow](https://web-sandbox.openrainbow.com). Ainsi pour pouvoir utiliser l'application, il est nécessaire de se prémunnir d'un compte Rainbow et de les utiliser pour intéragir avec l'application.

---

## 🚀 Backend

### Organisation du projet

```
📂 /
├── 📂 API                   # Dossier contenant l'API avec les logiques de résumé et traduction
│   ├── 📂 logique           # Traitement des informations reçues par les routes et l'IA
│   ├── 📂 routes            # Route API qui vérifie le contenu, traite les requêtes
│   ├── 📂 tests             # Tests unitaires des routes et logique
│   ├── 📄 utils.js          # Script qui gère la couche de base de l'implémentation de l'IA
│   ├── 📄 index.js          # Fichier principal qui initialise l'application backend
│   ├── 📄 package.json      # Liste des dépendances Node.js
│   ├── 📄 package-lock.json # Verrouillage des dépendances pour des builds reproductibles
├── 📂 AI-Model              # Dossier contenant le modèle IA et possibilité de lancer en local
├── 📄 README.md             # Readme du repository


```

### Developpez localement

Pour lancer l'environnement backend en local, clonez le dépôt backend, naviguez dans le dossier API, et lancez la commande `npm` qui permet de lancer l'environnement backend.

```shell
git clone https://github.com/Info-Broadcaster/backend.git
```

```shell
cd backend/API/
npm start
```
Pour avoir un reload automatique du serveur NodeJS après modification des fichiers:

```shell
npm run local
```
> 💡 N.B: Cette commande est un alias du script node qui lancera nodemon.

🏁 Ainsi, en local, l'environnement sera accessible depuis l'adresse `http://localhost:3000`

### Lancez les tests unitaires

Pour lancer les tests unitaires du backend, lancez la commande suivante:

```shell
npm test
```

### Technologies utilisées
- **[Express Node.js](http://expressjs.com/)** pour le Backend
- **[Ollama](https://ollama.com/)** comme package manager du modèle IA
- **[Jest](https://jestjs.io/)** comme framework de suite de tests 

---

## 💻 Frontend

### Organisation du projet

```
📂 /
├── 📂 public                  # Fichiers multimédia accessibles directement par les utilisateurs externes
├── 📂 src                     # Code source de l'application
│   ├── 📂 assets              # Fichiers multimédia utilisés en interne par le serveur
│   ├── 📂 components          # Composants réutilisables pour l'affichage
│   ├── 📂 functions           # Fonctions pour la gestion de l'authentification et de la logique métier
│── 📄 package.json            # Liste des dépendances Node.js
│── 📄 package-lock.json       # Verrouillage des dépendances pour des builds reproductibles

```

### Développez localement

Pour lancer l'environnement front en local, clonez le repository frontend du projet puis lancez l'environnement.

```shell
git clone https://github.com/Info-Broadcaster/frontend.git
```

```shell
cd frontend/
npm run dev
```

🏁 Ainsi, en local, l'environnement sera donc accessible depuis l'adresse `http://localhost:5173`

### Technologies utilisées

- **[React](https://react.dev/)** comme framework JS pour la création des composants
- **[Vite](https://vite.dev/)** comme moteur de développement

---

## 🔗 Ressources importantes

- [Project User Stories](https://docs.google.com/spreadsheets/d/1AgSSx4N9MPHHEJpwb3tNtURM2AWaZLXGsi03HbrfYrI/edit#gid=0)
- [Maquette Figma](https://www.figma.com/file/hDj5AWrREvboq14DKgZxUi/Untitled?type=whiteboard&node-id=0%3A1&t=Jj1iuTZdETlhQiny-1)
- [Documentation API Rainbow](https://developers.openrainbow.com/)
- [Ollama docs](https://github.com/ollama/ollama/tree/main/docs)

---

## 🧑‍💻 Contributors

- [@bobylatruffe](https://github.com/bobylatruffe) alias Fatih B.  
- [@Erestona](https://github.com/Erestona) alias Tanguy P.  
- [@ShortLegsFox](https://github.com/ShortLegsFox) alias Ian B.  
- [@Nerlake](https://github.com/Nerlake) alias Léo H.  
- [@Vladimir9595](https://github.com/Vladimir9595) alias Vladimir S.  
- [@maxime-hell](https://github.com/maxime-hell) alias Maxime H.  
- [@EpitronX](https://github.com/EpitronX) alias Jérémie M.  
- [@htregnagoCNAM](https://github.com/htregnagoCNAM) alias Hugo T.  
- [@WRKT](https://github.com/WRKT) alias Winness R.  
