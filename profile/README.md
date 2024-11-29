# INFOBROADCASTER :globe_with_meridians:

[InfoBroadcaster](https://infobroadcaster.netlify.app) est une application web développé sur une stack NodeJS dont **Express** pour le backend, et **React** pour le front qui permet de résumer automatiquement les informations d'un article en lui fournissant l'url.

Cette application permet également de partager les informations résumées dans des bulles [Rainbow](https://web-sandbox.openrainbow.com). 

Ainsi pour pouvoir utiliser l'application, il est nécessaire de se connecter avec ses identifiants Rainbow.

---

## Backend

### Organisation du projet

```
/
├── API                   # Dossier contenant l'API avec les logiques de resumé et traduction
  └── logique             # Traitement des informations reçues par les routes et l"IA
  └── routes              # Route API qui vérifie le contenu, traite les requêtes
  └── tests               # Tests unitaires des routes et logique
  └── utils.js            # Script qui gère la couche de base de l'implémentation de l'IA
  └── index.js            # Fichier principal qui initialise l'application backend
  └── package.json        # Liste des dépendances Node.js
  └── package-lock.json
├── AI-Model              # Dossier contenant le modèle IA et possibilité de lancer en local
├── postman-api           # Fichier  à importer dans Postman pour tester les requêtes
├── README.md             # Readme du repository

```

### Developpez localement

Pour lancer l'environnement backend en local, naviguez dans le dossier API, et lancez les commandes suivantes:

```shell
npm start
```

Pour avoir un reload automatique du serveur NodeJS après modification des fichiers:

```shell
npm run local
```
> N.B: Cette commande est un alias du script node qui lancera nodemon.

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

## Frontend

### Organisation du projet
```
/
├── public                  # Fichiers multimédia accessible aux utilisateur externe
├── src                     # Code source
  └── assets                # Fichier multimédia propre au serveur
  └── components            # Composants d'affichage
  └── functions             # Gestion de l'authentification
```

### Déveloper localement

```shell
npm run dev
```

### Technologies utilisées
- **[React](https://react.dev/)** comme framework JS pour la création des composants
- **[Vite](https://vite.dev/)** comme moteur de développement

---

## Ressources importantes
- [Lien Excel des User Stories](https://docs.google.com/spreadsheets/d/1AgSSx4N9MPHHEJpwb3tNtURM2AWaZLXGsi03HbrfYrI/edit#gid=0)
- [Lien Maquette Figma](https://www.figma.com/file/hDj5AWrREvboq14DKgZxUi/Untitled?type=whiteboard&node-id=0%3A1&t=Jj1iuTZdETlhQiny-1)
- [Liens Utiles - TensorFlow.NET](https://github.com/SciSharp/TensorFlow.NET?tab=readme-ov-file)
- [Documentation API Rainbow](https://developers.openrainbow.com/)

---

## Contributors
- @bobylatruffe alias Fatih B.
- @Erestona alias Tanguy P.
- @ShortLegsFox alias Ian B.
- @Nerlake alias Léo H.
- @Vladimir9595 alias Vladimir S.
- @maxime-hell alias Maxime H.
- @EpitronX alias Jérémie M.
- @htregnagoCNAM alias Hugo T.
- @WRKT alias Winness R.
