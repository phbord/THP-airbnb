# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version : _5.2.5_

* System dependencies :
  * gem `table_print`
  * gem `faker`

* Deployment instructions
  * `bundle i`
  * `rails db:migrate`
  * `rails db:seed`

* Configuration

* Models creation
  * `rails generate model Dogsitter name:string`
  * `rails generate model Dog name:string`
  * `rails generate model City city_name:string`
  * `rails generate model Stroll name:string duration:integer`

* Database initialization
  * `rails db:migrate`

* How to run the test suite

* Seeds
  * `rails db:seed`

* Tests

|ACTION|COMMANDE|
|:---|:---|
|Afficher la table des promenades|`tp Stroll.all`|
|Créer une ville|`City.create(city_name: "nom de la ville")`|
|Créer un nouveau dogsitter|`Dogsitter.create(first_name: "prénom", last_name: "nom de famille", city: City.find_by(city_name: nom de la ville))`|
|Créer un chien|`Dog.create(first_name: prénom du patient, city: City.find_by(city_name: nom de la ville))`|
|Créer une promenade|`Stroll.create(date: YYYY-mm-DD HH:MM:SS, dogsitter: dogsitter_existant, dog: chien_existant)`|

## Projet
Plateforme où des personnes pourraient promener les chiens des autres, en échange de cash-money.

### Models
- Dogsitter
- Dog
- City
- Stroll