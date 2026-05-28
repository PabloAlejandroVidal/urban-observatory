# Project Setup

This document describes the initial setup of the Urban Observatory repository.

## Repository Structure

The project is organized as a monorepo:

```txt
urban-observatory/
├── apps/
│   ├── api/
│   └── web/
├── docs/
├── infra/
└── data/
```

## Main Directories

* `apps/api`: backend application built with NestJS.
* `apps/web`: frontend application planned with Angular.
* `docs`: technical documentation.
* `infra`: deployment and infrastructure-related files.
* `data`: sample datasets, dataset references or data documentation.

## Requirements

* Node.js 22 LTS
* npm 10+
* Git
* NestJS CLI

The Node.js version is documented in the root `.nvmrc` file.

## Backend API

The backend application was initialized inside:

```txt
apps/api
```

The API was created with NestJS using:

```bash
nest new api --strict --skip-git --package-manager npm
```

### Command Notes

* `--strict`: creates the NestJS app with stricter TypeScript settings.
* `--skip-git`: prevents NestJS from creating a nested Git repository inside `apps/api`.
* `--package-manager npm`: uses npm as the package manager and generates `package-lock.json`.

## Running the API

From `apps/api`:

```bash
npm install
npm run start:dev
```

By default, the API runs at:

```txt
http://localhost:3000
```

The initial NestJS application returns:

```txt
Hello World!
```

## Git Notes

The repository uses a single Git history from the root of the monorepo.

A nested `.git` directory should not be created inside `apps/api` or `apps/web`.

## Line Endings

The repository includes a `.gitattributes` file to normalize line endings to LF:

```gitattributes
* text=auto eol=lf

*.bat text eol=crlf
*.cmd text eol=crlf
```

This helps avoid line-ending issues across Windows, Linux, Docker, CI/CD and VPS environments.

## Environment Variables

Environment variables should be documented in `.env.example`.

Real `.env` files must not be committed.
