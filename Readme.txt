python -m venv venv --Cria ambiente virtual
venv/Scripts/activate --usa virtual env source
pip install django --instala o django dentro da env 
pip install djangorestframework -- instala o restframework
pip install markdown --instala markdown
pip install django-filter --instala django filter
django-admin startproject api --cria projeto django com o nome de api
cd api --entra na pasta
python manage.py startapp core --cria uma aplicação
abrir o settings.py da pasta api e escrever "'core'," no ultimo item de INSTALLED_APPS = [
python manage.py migrate --cria banco de dados
python manage.py createsuperuser --cria superusuario
cadastre o usuario e crei a senha
python manage.py runserver --roda o projeto
registrar 'rest_framework', no settings igual ao core
incluir from django.urls import path, include + path('api-auth/', include('rest_framework.urls')) no urls.py do api
python manage.py makemigrations --prepara atualizacao banco de dados
python manage.py migrate --efetiva a atualizacao

