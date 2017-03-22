## Docker for Akeneo Pim
@see https://hub.docker.com/r/jeanberu/akeneo-pim/
### Requirements

1. Make sure you have docker and docker-compose on your system
2. Clone the Akeneo repository `git clone https://github.com/akeneo/pim-community-standard.git` in some path (`/home/julien/workspace` on my system)
3. Clone this repository in `some/other/path`

### Installation
0. Check the file `docker-compose.yml` and change `/home/julien/workspace` by your path.
1. `cd some/other/path` and start the projects using `docker-compose up -d`
2. Install Akeneo Pim with :
```
docker-compose run --rm app composer install
docker-compose run --rm app app/console pim:install
```

### After Installation
1. Go to `localhost:8080` and use `admin/admin` as login/password