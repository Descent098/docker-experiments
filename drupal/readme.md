# Drupal

A simple compsoe for getting drupal up and running



## Usage

First setup a network to use:

```bash
docker network create drupal
```

Then run the container using 

```bash
docker compose up
```

From there head to [http://localhost:7885](http://localhost:7885) and finish setup. 



If you **do not want postgres** then on the *Setup database* step, select SQLite and enter your info, if you do, then scroll down (I didn't bother doing MySQL/MariaDB support).



## Using Postgres

To setup postgres uncomment the commented out lines in docker-compose.yml (keep track of the`network_mode`,  `container_name` and `environment` details).



Setup drupal as normal, but on the *Set up a database* tab you need to change the following settings:



    Database type: PostgreSQL

    Database name: drupal (environment.POSTGRES_DB)

    Database username: drupal (environment.POSTGRES_USER)

    Database password: pass (environment.POSTGRES_PASSWORD)



Then under the *Advanced Options* dropdown you want to change:



    Host: postgres (container_name and this only works if `network_mode` is same on drupal and postgres)






