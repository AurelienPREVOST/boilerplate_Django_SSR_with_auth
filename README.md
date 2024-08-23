# Django Boilerplate

Ce projet est un boilerplate Django prêt à l'emploi pour démarrer rapidement des projets web. Il inclut des fonctionnalités de base comme l'authentification des utilisateurs, une structure de templates modulaire, et une configuration de base pour le développement.

## Fonctionnalités

- Authentification des utilisateurs (connexion, déconnexion, inscription, réinitialisation du mot de passe)
- Structure de templates modulaire avec un template de base
- Séparation des configurations en fichiers partiels pour la navbar et le footer
- Configuration prête pour déployer le projet
- Attention : Aucun client mail pour l'authentification, le contenu du mail apparaitra dans le terminal

## Prérequis

- Python 3.x
- Django 5.x
- Git

## Installation

1. Clonez le dépôt :

    ```bash
    git clone https://github.com/username/django-boilerplate.git
    cd django-boilerplate
    ```

2. Créez un environnement virtuel et activez-le :

    ```bash
    python -m venv env
    source env/bin/activate  # Sur Windows : env\Scripts\activate
    ```

3. Installez les dépendances :

    ```bash
    pip install -r requirements.txt
    ```

4. Créez un fichier `.env` à la racine du projet pour stocker les variables d'environnement nécessaires :

    ```bash
    touch .env
    ```

    Exemple de contenu pour `.env` :

    ```ini
    SECRET_KEY=votre_cle_secrete
    DEBUG=True
    ALLOWED_HOSTS=localhost,127.0.0.1
    ```

5. Appliquez les migrations pour configurer la base de données :

    ```bash
    python manage.py migrate
    ```

6. Créez un super utilisateur pour accéder à l'interface d'administration de Django :

    ```bash
    python manage.py createsuperuser
    ```

7. Démarrez le serveur de développement :

    ```bash
    python manage.py runserver
    ```

    Accédez à l'application via `http://127.0.0.1:8000/`.

## Comment Contribuer

Si vous souhaitez contribuer à ce projet, veuillez suivre les étapes ci-dessous :

1. Forkez le projet
2. Créez une branche pour votre fonctionnalité (`git checkout -b feature/nom-de-la-fonctionnalité`)
3. Faites vos modifications et engagez-les (`git commit -m 'Ajouter une fonctionnalité'`)
4. Poussez vos modifications (`git push origin feature/nom-de-la-fonctionnalité`)
5. Créez une Pull Request

## Licence

Ce projet est sous licence MIT. Consultez le fichier `License` pour plus d'informations.
