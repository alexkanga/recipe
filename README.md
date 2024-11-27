
# Application de Recettes React-Node 🍲

Bienvenue dans l'application de recettes React-Node ! Cette application permet aux utilisateurs de consulter, ajouter et gérer leurs recettes préférées. Elle est construite avec React pour le frontend et Node.js avec l'ORM Prisma pour le backend. Elle utilise également la base de données PostgreSQL de render.com

## Commencer 🚀

### Prérequis :

- Node.js et npm installés sur votre machine.
- Un compte sur [Render Postgresql](https://render.com/docs/postgresql-creating-connecting) pour la base de données (utilisez un lien externe pour le développement).
- Une [clé API Spoonacular](https://spoonacular.com/food-api) pour l'API de recettes.

### Configuration :

1. **Cloner le dépôt** :
   ```bash
   git clone https://github.com/alexkanga/recipe.git
   cd recipe
   ```

2. **Configuration du Backend** :

   - Accédez au répertoire backend :
     ```bash
     cd backend
     ```

   - Installez les packages nécessaires :
     ```bash
     npm install
     ```

   - **API Spoonacular** :
     - Ajoutez la clé API à la variable `API_KEY` dans le fichier `.env`.

   - **Configuration de postgresqL sur render externe** :
     - Créez une nouvelle instance de base de données sur PostgreSQL render.
     - Copiez la chaîne de connexion PostgreSQL fournie .

   - **Configuration de Prisma** :
     - Remplacez la valeur de `DATABASE_URL` dans le fichier `.env` par la chaîne de connexion PostgreSQL.
     - Initialisez Prisma et générez le client Prisma :
       ```bash
       npx prisma init
       npx prisma generate
       ```

   - Démarrez le serveur backend :
     ```bash
     npm start
     ```

3. **Configuration du Frontend** :

   - Accédez au répertoire frontend :
     ```bash
     cd frontend
     ```

   - Installez les packages nécessaires :
     ```bash
     npm install
     ```

   - Démarrez le serveur de développement frontend :
     ```bash
     npm run dev
     ```
4. **Version demo** :
https://recipe-1-5flp.onrender.com/