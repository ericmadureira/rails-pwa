# Rails PWA (Progressive Web App)

## Technologies used
* Ruby: **2.5.5**
* Rails: **5.2.3**
* database: **postgres**

## Setup
1. Open terminal
2. Run `git clone https://github.com/ericmadureira/rails-pwa`
3. Run `cd rails-pwa`
4. In config/database.yml change the definitions to match your database

From here on things get different if you want to use Docker or not:

* Install using Docker
5. Run `docker-compose up`
6. Open another terminal and run `docker-compose run web bundle exec rake db:create db:migrate` (needs to be done only once)
7. Your rails PWA is ready at localhost:3000.

* Install without Docker
5. Run `bundle install`
6. Run `bundle exec rake db:create db:migrate`
7. Run `rails server`
8. Your rails PWA is ready at localhost:3000.

## References
* https://docs.docker.com/compose/rails/
* https://onebitcode.com/pwa-rails/ (pt-BR) - Thanks to Leonardo Scorza and his amazing job teaching at OneBitCode
* 