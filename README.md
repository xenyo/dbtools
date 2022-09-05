# uni_devops

Provides devops scripts for Xenyo Uni Framework.

## Installation

Add the library to your project:

```bash
composer require xenyo/uni_devops
```

#### Note for Windows users

You must run the scripts using Git Bash. You may need to add the mysql bin directory to your PATH.

## Usage

Make sure you `cd` to your project root before running any scripts.

#### export-db

```bash
vendor/bin/export-db
```

Exports the database to `database.sql`. Cache, history and watchdog tables are excluded. The database dump is stored in plain text instead of gzipped so that git can process it efficiently.

#### import-db

```bash
vendor/bin/import-db
```
Imports the database from `database.sql`. Will drop existing database before importing.
