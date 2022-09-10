# Customer Relationship Management System

Role-based Django web application with Postgres DBMS

## First steps

### Environment variables

    cp .env.example .env

### Start dev containers

    docker-compose up --build -d

### Run migrations

    docker-compose exec app python crm1/manage.py migrate

### Create super user

Create superuser credentials using the command below so you can login to the web app Django administration panel

    docker-compose exec app python crm1/manage.py createsuperuser

## Getting started

 - Request to [localhost:8080](localhost:8080) and login in to the **web app**
 - Request to [localhost:8080/admin](localhost:8080/admin) for accessing to the web app admin panel using superuser credentials previously created
 - For administreate database in **Pgadmin** request to [localhost:82](localhost:82)
 - You can see emails on **Mailhog** requesting to [localhost:8025](localhost:8025)