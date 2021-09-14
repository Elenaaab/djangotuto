# Procédure de démarrage

1. Se placer dans le dossier où on souhaite créer le projet et créer un projet django : django-admin startproject nomprojetàcréer
2. Se placer dans le répertoire racine du projet (où se trouve le fichier manage.py)
3. Démarrer le virtualenv : workon nomVirtualEnv
4. Démarrer le serveur de développement : python manage.py runserver

5. ## Guide en trois étapes pour effectuer des modifications aux modèles

- Modifier les modèles (dans models.py).
- Exécuter python manage.py makemigrations pour créer des migrations correspondant à ces changements.
- Exécuter python manage.py migrate pour appliquer ces modifications à la base de données.

6. Lancer un shell interactif pour interagir avec l'API : python manage.py shell

7. ## Créer un site d'administration (back office)

- Créer un superuser : python manage.py createsuperuser
- Lancer le serveur : python manage.py runserver
- Aller sur l'URL d'administration (ouvrir le navigateur web et ajouter /admin/) : http://127.0.0.1:8000/admin/.