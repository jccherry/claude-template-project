# Database

## Overview

<!-- Describe the database: type (Postgres, MySQL, MongoDB, etc.), hosting, ORM/query builder. -->

## Schema

<!-- High-level description of the data model. Include an ER diagram if helpful. -->

```
┌──────────┐       ┌──────────┐
│  users   │───┐   │  orders  │
└──────────┘   │   └──────────┘
               │        │
               └────────┘
```

## Tables / Collections

<!-- Document key tables with their columns and relationships. -->

### `users`

| Column | Type | Constraints | Description |
|--------|------|-------------|-------------|
| <!-- id --> | <!-- uuid --> | <!-- PK --> | <!-- Primary key --> |

## Migrations

<!-- Describe the migration tool and workflow. -->

```bash
# Run migrations
# npm run migrate

# Create a new migration
# npm run migrate:create <name>

# Rollback last migration
# npm run migrate:rollback
```

## Seeding

```bash
# Seed the database with test data
# npm run seed
```

## Indexes

<!-- Document any important indexes beyond primary keys and their rationale. -->

## Backups

<!-- Describe the backup strategy: frequency, retention, restore process. -->

## Connection Configuration

| Variable | Description | Required |
|----------|-------------|----------|
| <!-- DATABASE_URL --> | <!-- Connection string --> | <!-- Yes --> |

## Notes

<!-- Performance considerations, known data constraints, archival strategy. -->
