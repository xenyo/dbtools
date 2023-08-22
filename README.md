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
composer exec dbe [file]
```

Exports the database to the given file. Defaults to `database.sql`.

### Import database

```
composer exec dbi [file]
```

Drops existing database and imports the database from the given file. Defaults to `database.sql`.

### Export database (gzipped)

```
composer exec dbez [file]
```

Exports the database to the given file. Defaults to `database.sql.gz`.

### Import database (gzipped)

```
composer exec dbiz [file]
```

Drops existing database and imports the database from the given file. Defaults to `database.sql.gz`.
