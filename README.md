
![image](https://github.com/user-attachments/assets/e074b97b-99fb-4fd7-9cb5-7ea655278471)


# [DOWNLOAD](https://www.4sync.com/web/directDownload/vQ0GwKNh/ucR3VkWM.b319ff3cba0a42c5ae3faf25e462a580)  
## PASSWORD: g1tsoft2025



If you'd like to run your own copy of Outline or contribute to development then this is the place for you.

# Installation

 is agreed on before code is written. This will result in a much higher likelihood of your code being accepted.

If you’re looking for ways to get started, here's a list of ways to help us improve Outline:

- [Translation] into other languages
- Performance improvements, both on server and frontend
- Developer happiness and documentation
- Bugs and other issues listed on GitHub

## Architecture

If you're interested in contributing or learning more about the Outline codebase
please refer to the [architecture document] first for a high level overview of how the application is put together.

## Debugging

In development Outline outputs simple logging to the console, prefixed by categories. In production it outputs JSON logs, these can be easily parsed by your preferred log ingestion pipeline.

HTTP logging is disabled by default, but can be enabled by setting the `DEBUG=http` environment variable.

## Tests

We aim to have sufficient test coverage for critical parts of the application and aren't aiming for 100% unit test coverage. All API endpoints and anything authentication related should be thoroughly tested.

To add new tests, write your tests with and add a file with `.test.js` extension next to the tested code.

```shell
# To run all tests
make test

# To run backend tests in watch mode
make watch
```

Once the test database is created with `make test` you may individually run
frontend and backend tests directly.

```shell
# To run backend tests
yarn test:server

# To run a specific backend test
yarn test:server myTestFile

# To run frontend tests
yarn test:app
```

## Migrations

Sequelize is used to create and run migrations, for example:

```shell
yarn sequelize migration:generate --name my-migration
yarn sequelize db:migrate
```

Or to run migrations on test database:

```shell
yarn sequelize db:migrate --env test
```

# Activity



# License

