# Steps to reproduce

1. Install dependencies via `composer i`.
1. Setup your `.env` properly according to `.env.example`:
    - `DB_CONNECTION=pgsql` required
    - Your `DB_HOST`
    - Your `DB_PORT`
    - Your `DB_DATABASE`
    - Your `DB_USERNAME`
    - Your `DB_PASSWORD`
1. Inside project run the following commands in this order:
    - `php artisan migrate` - All must be ok
    - `php artisan migrate:fresh` - Command fails on `common.users` table
