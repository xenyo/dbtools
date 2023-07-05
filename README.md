# xenyo/dbtools

Command line tools for importing and exporting databases on Drupal sites.

## Features

- DB dumps exclude cache, history and watchdog and sessions tables.
- Option to import and export with compression (gzip).

## Installation

Run this command in your project root to install the package:

```bash
composer require xenyo/dbtools
```

## Commands

All commands must be run from the project root.

### Export database

```
composer exec dbe
```

Exports the database to `database.sql`.

### Import database

```
composer exec dbi
```

Drops existing database and imports the database from `database.sql`.

### Export database (gzipped)

```
composer exec dbez
```

Exports the database to `database.sql.gz`.

### Import database (gzipped)

```
composer exec dbiz
```

Drops existing database and imports the database from `database.sql.gz`.
