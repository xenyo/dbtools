# xenyo/drupal-scripts

Provides reusable devops scripts for Drupal sites.

## Installation

Add the library to your project:

```bash
composer require xenyo/drupal-scripts
```

### Note for Windows users

You must run the scripts using Git Bash. They will not work in cmd or powershell. You may need to add the mysql bin directory to your PATH.

## Usage

Make sure you `cd` to your project root before running any scripts.

### export-db

```bash
vendor/bin/export-db
```

Exports the database to `database.sql`. Cache, history and watchdog tables are excluded. The database dump is stored in plain text instead of gzipped so that git can process it efficiently.

### import-db

```bash
vendor/bin/import-db
```

Imports the database from `database.sql`. Will drop existing database before importing.

### reset-uuid

```bash
vendor/bin/reset-uuid
```

Generates a new UUID for the site and replaces the values in config/sync/system.site.yml and database.sql. You should re-import the database after running this command.
