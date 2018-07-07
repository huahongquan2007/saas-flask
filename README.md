## Build
- Build images and run container
```
docker-compose up --build
```
- Run container
```
docker-compose up
```
- Stop container. Ctrl-C or
```
docker-compose stop
```

## Command line interface
- View list commands
```
docker-compose exec website snakeeyes
```
- View command help for `test`
```
docker-compose exec website snakeeyes test --help
```

## Tests

### Run tests
- Run tests using CLI
```
docker-compose exec website snakeeyes test
```
- Run tests manually
```
docker-compose exec website py.test snakeeyes/tests
```

### Run test coverage
- Run test coverage using CLI
```
docker-compose exec website snakeeyes cov
```
- Run test coverage manually
```
docker-compose exec website py.test --cov-report term-missing --cov snakeeyes/
```

### Run code quality
- Check code quality using CLI
```
docker-compose exec website snakeeyes flake8
```
- Check code quality manually
```
docker-compose exec website flake8 .
```
