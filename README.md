# xenyo/uni-tools

Developer tools for Xenyo Uni Framework sites.

## Installation

Add the library to your project:

```bash
composer require xenyo/uni-tools
```

## Scripts

`cd` to your project root before running any scripts.

### database-export

```bash
composer exec database-export
```

```bash
composer exec dbe
```

Exports the database to `database.sql`. Cache, history and watchdog and sessions tables are excluded. The database dump is stored in plain text instead of gzipped so that git can track changes efficiently.

### database-import

```bash
composer exec database-import
```

```bash
composer exec dbi
```

Imports the database from `database.sql`. Drops existing database before importing.
