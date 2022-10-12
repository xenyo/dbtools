# xenyo/uni-tools

Developer tools for Xenyo Uni Framework sites.

## Installation

Add the library to your project:

```bash
composer require xenyo/uni-scripts
```

### Notes for Windows users

- You must run the scripts using Git Bash. They will not work in cmd or powershell.
- You must add the MySQL bin directory to your PATH.

## Scripts

Make sure you `cd` to your project root before running any scripts.

### export-db

```bash
vendor/bin/export-db
```

Exports the database to `database.sql`. Cache, history and watchdog and sessions tables are excluded. The database dump is stored in plain text instead of gzipped so that git can track changes efficiently.

### import-db

```bash
vendor/bin/import-db
```

Imports the database from `database.sql`. Will drop existing database before importing.
