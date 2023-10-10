# Shell scripts

## Installation

Go to scripts/docker and run:

```
sudo cp run /usr/local/bin/run
sudo cp prod-compose /usr/local/bin/prod-compose
sudo cp prod /usr/local/bin/prod
```

## Usage

```
run help
```

`prod` command is similar to run command, but it uses docker-compose.prod.yml file instead of docker-compose.yml
`prod-compose` is alias for `docker-compose -f docker-compose.prod.yml`

## Examples

Go to examples folder

- `run rebuild` - rebuilds all services in docker-compose.yml and starts them. Open http://localhost:8000 in browser 
- `run rebuild nginx` - rebuilds nginx service in docker-compose.yml and starts it
- `run sh nginx` - runs sh command in nginx service
- `run logs` - shows logs of all services in docker-compose.yml
- `run logs nginx` - shows logs of nginx service
- `run stop` - stops all services
