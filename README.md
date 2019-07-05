
Description
===========

Given an undefined project, composed of

- a backend application, developed in Python/Django, or PHP/Symfony 2.x
- a frontend application, developed in Python/Flask, or PHP/Sylex, or Angular
- a relational database, such as PostgreSQL
- a NoSQL database, such as Redis, or Mongo, working as cache
- a queue server, such as RabbitMQ
- a container manager, such as Docker Composse
- a continous integration manager, such as Jenkins, or Grunt

The frontend will have no business logic, these will be entirely in the backend application.

Every time the frontend needs some information, it will check the cache server (Couchbase, MongoDB),
if the information is not there it will then query the backend application for that information in
the relacional database (PostgreSQL) and update the cache server with the information it receives from it.

Every time the frontend needs to update data, it will store the new data in the cache server and
add a request in the queue server (RabbitMQ), which will be consumed by the backend application
whenever possible, updating the relational database (PostgreSQL).

Goals
=====

To improve myself in some of the following technologies:

- Python
- Django
- Flask
- Symfony 2.x
- Sylex
- Angular
- PostgreSQL
- Couchbase
- MongoDB
- RabbitMQ
- Kubernetes
- Docker
- Ansible
- Vagrant
- Jenkins
- Grunt

Secondary Goals
===============

Have the user's client store information using the HTML5 Storage, accessing it before 
making any ajax requests to the frontend application.
