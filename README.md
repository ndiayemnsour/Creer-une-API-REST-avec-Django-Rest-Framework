# Creer-une-API-REST-avec-Django-Rest-Framework
Créer une API REST avec Django Rest Framework pour communiquer avec le serveur et Front-End

## Initialisation du projet
1. créer un environnement virtuel venv
```
python3 -m venv .venv
```
2. Avtiver venv
sous windows
```
.venv\Scripts\activate
```
sous mac os
```
source .venv/bin/activate 
```
3. Installer django rest framework, si django n'est pas installer il sera
```
pip install djangorestframework
```
4. Créer le projet gestion_library avec
```
django-admin startproject gestion_library
```
5. Créer l'app library dans le repertoire du projet : gestion_library
```
python manage.py startapp library
```
python manage.py startapp library
```

## Creation, migration du model
1. creation des Models dans le fichier models : Author(name), Book(title), Loan(borrow_date, return_date)

2. Enrigistrer les models dans admin.py
admin.site.register(Author)
admin.site.register(Book)
admin.site.register(Loan)

3. Ajouter notre app Library dans sittings.py
4. Executer les migrations
```
python manage.py makemigrations
```
```
python manage.py migrate
```
5. Creer un super-utilisateur pour la page admin : saisir le user, email puis password
```
python manage.py createsuperuser
```
6. lancer l'app : 
```
python manage.py runserver
```
Utiliser ce lien pour acceder la page accueil http://127.0.0.1:8000/
Pour la page admin : http://127.0.0.1:8000/admin