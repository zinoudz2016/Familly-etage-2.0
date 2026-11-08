# Application Famille Étage (Avec Synchronisation Cloud Firebase)

Cette version intègre la synchronisation en temps réel via **Google Firebase Firestore** :
- **Papa** : Zineddine (`paralgan500@gmail.com`)
- **Maman** : Alaa (`dr.bouhicha@gmail.com`)
- **Enfants** : Larine (8 ans) & Taline (3 ans)

---

## Comment activer la synchronisation en temps réel entre vos 2 téléphones ?

1. Rendez-vous sur [console.firebase.google.com](https://console.firebase.google.com/) avec votre compte Google.
2. Cliquez sur **Créer un projet** (ex. `famille-etage`).
3. Dans le menu de gauche, cliquez sur **Firestore Database**, puis **Créer une base de données** (choisissez le mode test pour autoriser lecture et écriture).
4. Allez dans **Paramètres du projet** (icône d'engrenage en haut à gauche) > **Général** > section **Vos applications**, puis cliquez sur l'icône Web `</>`.
5. Donnez un nom et copiez l'objet `firebaseConfig` affiché, par exemple :
   ```json
   {
     "apiKey": "AIzaSy...",
     "authDomain": "famille-etage.firebaseapp.com",
     "projectId": "famille-etage",
     "storageBucket": "famille-etage.appspot.com",
     "messagingSenderId": "...",
     "appId": "..."
   }
   ```
6. Ouvrez l'application, allez dans l'onglet **Paramètres**, collez ce texte dans la section **Synchronisation en Direct** et cliquez sur **Enregistrer & Activer Cloud**.

Dès cet instant, chaque modification faite par Papa (tâche terminée, achat ajouté, dépense enregistrée) apparaît instantanément sur le téléphone de Maman et inversement, même après fermeture et réouverture !
