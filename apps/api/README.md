# API

Backend de Urban Observatory.

Esta aplicación expone la API principal de la plataforma, encargada de gestionar autenticación, usuarios, roles, datasets, capas geográficas y futuras operaciones relacionadas con datos urbanos y geoespaciales.

## Stack

* NestJS
* TypeScript
* PostgreSQL
* PostGIS
* JWT Authentication
* Roles y permisos

## Requirements

* Node.js 22 LTS
* npm 10+
* Git
* NestJS CLI

## Project setup

```bash
npm install
```

## Run the application

```bash
# development
npm run start

# watch mode
npm run start:dev

# production mode
npm run start:prod
```

## Run tests

```bash
# unit tests
npm run test

# e2e tests
npm run test:e2e

# test coverage
npm run test:cov
```

## Project context

This API is part of the Urban Observatory monorepo.

Repository structure:

```txt
urban-observatory/
├── apps/
│   ├── api/
│   └── web/
├── docs/
├── infra/
└── data/
```

## Notes

This backend starts as a modular NestJS API and will evolve progressively with authentication, roles, database integration, geospatial data support and deployment configuration.
