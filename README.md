
# Install latest version Laravel 
cd laravel 
sh ./install-laravel;
# Run Docker

./run-docker.sh up

docker exec -it laravel sh -c "composer install"
docker exec -it laravel sh -c "php artisan key:generate"

# Initialize PHP-CI

./initialize.sh
