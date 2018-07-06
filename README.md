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

## Tests
- Run tests
```
docker-compose exec website py.test snakeeyes/tests
```
- Run test coverage
```
docker-compose exec website py.test --cov-report term-missing --cov snakeeyes/
```
- Check code quality
```
docker-compose exec website flake8 .
```
