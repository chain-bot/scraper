# coinprice price scraper
<a href='https://github.com/jpoles1/gopherbadger' target='_blank'>![gopherbadger-tag-do-not-edit](https://img.shields.io/badge/Go%20Coverage-75%25-brightgreen.svg?longCache=true&style=flat)</a>

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/X8X71S1S7)

Web-Scraper for crypto prices built in Go

## Database Migrations and Models
- App [models](./main/models/generated) are generated using the database schema
- [sqlboiler](https://github.com/volatiletech/sqlboiler) introspects the database schema and creates the model files
- Before generating the models, the database needs to be running, and the migrations need to be executed
```bash
docker-compose up -d 
./scripts/run-database-migrations.sh
./scripts/generate-database-models.sh
```

## Tests
- TODO: Integrate uber fx in tests
- Run tests and update code coverage badge via script
```bash
./scripts/run-test-with-coverage.sh
```
