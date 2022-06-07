

To create a local container with the project execute:
git clone https://github.com/kollexarbeit/ctta.git --recurse-submodules ctta
cd ctta
cd app
git checkout master
composer install
cd ..
docker-compose up


To create a DB and pull the beers list into local repo:
- run the CLI on ctta_myapp_1 container, execute inside:
php bin/console doctrine:database:create
php bin/console doctrine:migrations:migrate


To display the beers page:
http://localhost:8000/beers

