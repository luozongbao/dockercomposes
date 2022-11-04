# how to use this compose file
1. run compose up -d
2. make sure 'src' is clean by delete the 'public' folder in 'src' folder.
3. run create project command using 'docker compose run'
```
docker compose run --rm composer composer create-project laravel/laravel .
```
4. make sure 'src/storage' and 'src/bootstrap' has 777 permission
```
  chmod -R 777 src/storage src/bootstrap
```
5. Edit src/.env file
6. run npm install using 'docker compose run'
```
docker compose run --rm npm install
```
7. run artisan migrate
```
docker compose run --rm artisan migrate
```
