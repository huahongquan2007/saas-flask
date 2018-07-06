

## Tests
- Run tests
```
docker-compose exec website py.test snakeeyes/tests
```
- Run test coverage
```
docker-compose exec website py.test --cov-report term-missing --cov snakeeyes/
```
