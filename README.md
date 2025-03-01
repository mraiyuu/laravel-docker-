<!--Heading-->
![npm](https://img.shields.io/npm/v/npm
) ![php](https://img.shields.io/badge/php-v8.2.0-v8
) ![laravel](https://img.shields.io/badge/laravel-v11.0-v8
)

---

# _Installation_

```diff
+PHP version 8.2 is required
```



# _Configuration_
```diff
Connect to your database
DB_CONNECTION=mysql
DB_HOST=database
DB_PORT=3306
DB_DATABASE=laravel
DB_USERNAME=root
DB_PASSWORD=
```

# _Docker configuration and running_
```
Have docker installed in you OS, chech how to do that 
from official docs. 

>>cd in the root directory of your project 

>>copy .env from .env.example

>>make entrypoint.sh executable
>> chmod +x docker/entrypoint.sh

>>docker-compose up -d --build(pull, build and run the containers)

>>docker ps(check active running containers)

>>docker exec -it larave_app php artisan migrate(run migrations inside your container)
laravel_app is the name of your container, if you change that, make sure to replace here


-docker compose down(stops the containers, you dont want them running forever right?)
