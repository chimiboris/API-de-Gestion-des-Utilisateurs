# API de Gestion des utilisateurs

## 📌 Fonctionnalités
- 📄 Créer un utilisateur avec nom, email et mot de passe (crypté avec
	BCrypt).
- 📋 Consulter la liste des utilisateurs. (Authentification exigée)
- 📝 Mettre à jour un utilisateur. (Authentification exigée)
- 🗑️ Supprimer un utilisateur. (Authentification exigée)
- 🗑️ Authentification : Un utilisateur peut se connecter via son email et son
	mot de passe.

## 🚀 Commande pour le lancement de l'application
```bash
mvn spring-boot:run

## 🚀 url pour tester l'application sur swagger
👉 http://localhost:8082/swagger-ui.html
ou
👉 http://localhost:8082/swagger-ui/index.html
ou
👉 http://localhost:8082/swagger-ui/index.html#/


Instruction pour les test sur swagger:

Après avoir démarrer le projet, bien vouloir utiliser ces liens http://localhost:8082/swagger-ui/index.html#/   ou ceci http://localhost:8082/swagger-ui/index.html pour avoir accès à l’interface graphique de swagger puis créer un utilisateur (avec pour rôle ADMIN) sur l’API POST /api/auth/register Ajouter un nouveau utilisateur avec par exemple les données suivantes :
{
  "username": "username",
  "email": "email@gmail.com",
  "password": "password",
  "role": "ADMIN"
}
Ensuite utilisez exactement ces mêmes données ci-dessus que vous avez renseignés pour vous authentifier à travers l’API POST/api/auth/login, une fois connecté utilisez le token qui ous sera genéré sur Authorize(un symbole de cadenas) puis coller uniquement le token du genre(HYjjsbdk5rzfgbjfe6...) dans le champ value qui vous sera proposé ensuite cliquez sur close tout en restant connecté car c’est une fois authentifié que vous pouvez tester toutes les autres API car elles exigent d’être d’abord authentifiées avant de faire toutes opérations sur les autres API.




