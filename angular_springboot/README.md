# angularspringbootmicrosservico
This application was generated using JHipster 4.5.1, you can find documentation and help at [https://jhipster.github.io/documentation-archive/v4.5.1](https://jhipster.github.io/documentation-archive/v4.5.1).

This is a "microservice" application intended to be part of a microservice architecture, please refer to the [Doing microservices with JHipster][] page of the documentation for more information.

This application is configured for Service Discovery and Configuration with . On launch, it will refuse to start if it is not able to connect to .

## Development

To start your application in the dev profile, simply run:

    ./gradlew


For further instructions on how to develop with JHipster, have a look at [Using JHipster in development][].

### Using angular-cli

You can also use [Angular CLI][] to generate some custom client code.

For example, the following command:

    ng generate component my-component

will generate few files:

    create src/main/webapp/app/my-component/my-component.component.html
    create src/main/webapp/app/my-component/my-component.component.ts
    update src/main/webapp/app/app.module.ts

## Building for production

To optimize the angularspringbootmicrosservico application for production, run:

    ./gradlew -Pprod clean bootRepackage

To ensure everything worked, run:

    java -jar build/libs/*.war


Refer to [Using JHipster in production][] for more details.

## Testing

To launch your application's tests, run:

    ./gradlew test

For more information, refer to the [Running tests page][].

## Using Docker to simplify development (optional)

You can use Docker to improve your JHipster development experience. A number of docker-compose configuration are available in the [src/main/docker](src/main/docker) folder to launch required third party services.
For example, to start a no database in a docker container, run:

    docker-compose -f src/main/docker/no.yml up -d

To stop it and remove the container, run:

    docker-compose -f src/main/docker/no.yml down

You can also fully dockerize your application and all the services that it depends on.
To achieve this, first build a docker image of your app by running:

    ./gradlew bootRepackage -Pprod buildDocker

Then run:

    docker-compose -f src/main/docker/app.yml up -d

For more information refer to [Using Docker and Docker-Compose][], this page also contains information on the docker-compose sub-generator (`jhipster docker-compose`), which is able to generate docker configurations for one or several JHipster applications.

## Continuous Integration (optional)

To configure CI for your project, run the ci-cd sub-generator (`jhipster ci-cd`), this will let you generate configuration files for a number of Continuous Integration systems. Consult the [Setting up Continuous Integration][] page for more information.

[JHipster Homepage and latest documentation]: https://jhipster.github.io
[JHipster 4.5.1 archive]: https://jhipster.github.io/documentation-archive/v4.5.1
[Doing microservices with JHipster]: https://jhipster.github.io/documentation-archive/v4.5.1/microservices-architecture/
[Using JHipster in development]: https://jhipster.github.io/documentation-archive/v4.5.1/development/
[Using Docker and Docker-Compose]: https://jhipster.github.io/documentation-archive/v4.5.1/docker-compose
[Using JHipster in production]: https://jhipster.github.io/documentation-archive/v4.5.1/production/
[Running tests page]: https://jhipster.github.io/documentation-archive/v4.5.1/running-tests/
[Setting up Continuous Integration]: https://jhipster.github.io/documentation-archive/v4.5.1/setting-up-ci/


