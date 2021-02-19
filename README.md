# Instructions for:
## Updating source code and rebuilding
1. Make desired changes to code
2. Go to azerothcore root directory
3. Run `./bin/acore-docker` to trigger compilation
4. Run `docker-compose down` then `docker-compose up` to destroy then recreate your docker containers

## Editing server variables
1. File worldserver.conf.dist is in /docker/worldserver/etc/
2. After changes are made, restart the worldserver either manually through docker's GUI or by running `docker-compose down` then `docker-compose up` 

## Connecting to Worldserver
1. Go to azerothcore root directory
2. Run `winpty docker attach azerothcore-wotlk_ac-worldserver_1`

