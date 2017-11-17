# README

Rails Gems:

gem 'bcrypt', '~> 3.1.7'
gem 'jwt'
gem 'simple_command'

Rails Commands

    1) bundle
    2) rails db:create
    3) rails db:migrate
    4) rails db:seed
    5) rails s

Create account:
Rails c

User.create!(email: 'admin@gmail.com' , password: 'adminadmin' , password_confirmation: 'adminadmin')


Commands for  API:

    $ curl -H "Content-Type: application/json" -X POST -d '{"email":"admin@gmail.com","password":"adminadmin"}' http://localhost:3000/login

    $ curl -H "Authorization: <tokken>" http://localhost:3000/items

	Example:
    curl -H "Authorization: eyJhbGciOiJIUzI1NiJ9.eyJ1c2VyX2lkIjoyLCJleHAiOjE1MTA4NTQ1NjZ9.En-1ZmziPeorKklNESHQTbzRrFrAH-fDIn8hwWgdK2k" http://localhost:3000/items