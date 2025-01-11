# Rails Playground

This project is a playground for experimenting and exploring Rails. The database is PostgreSQL.

## Getting Started

1. Run `bundle install`.
2. Run `bin/rails db:setup`.
3. Run `bin/rails server`.

## Database

The database is PostgreSQL. The database is created in the `db/seeds.rb` file.

- Run `bin/rails db:migrate` to perform migrations.
- Run `bin/rails db:rollback` to undo the last migration.
- Run `bin/rails db:seed` to perform seeding.

Whenever someone makes changes to the database schema, you need to run `bin/rails db:migrate` to update the database locally. If the seeds were updated, you need to run `bin/rails db:seed` to update the database with the new seeds.

## Console

Rails has a console that you can use to interact with the database. Run `bin/rails console` to start the console.

If the console is running while you make updates to the code, run `reload!` to load the new code.

If you want changes in the console to not affect the database run `bin/rails console --sandbox`. This will rollback any changes you make whenever you exit the console.

## TODO

- [ ] Add a simple API
- [ ] Add a simple admin interface
- [ ] Add Sentry
- [ ] Add Codecov
- [ ] Add simple background job with Sidekiq
- [ ] Experiment with [Fabrication](https://fabricationgem.org/)

Things you may want to cover:

- Ruby version

- System dependencies

- Configuration

- Database creation

- Database initialization

- How to run the test suite

- Services (job queues, cache servers, search engines, etc.)

- Deployment instructions

- ...
