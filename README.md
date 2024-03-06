# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

3.3.0

* System dependencies

* Configuration

* Database creation
Run the following commands in `psql` shell.

On linux you can login as superuser `postgres` and launch `psql` shell
with: 

```
sudo -u postgres psql
```

After launching `psql` as `postgres` run the following commands:

```
  create user sa_invizi_dev with password 'super_secret_password';
  create user sa_invizi_test with password 'super_secret_password';
  create database invizi_development owner sa_invizi_dev;
  create database invizi_test owner sa_invizi_test;
  alter user sa_invizi_test CREATEDB;
  alter user sa_invizi_dev CREATEDB;
```

Move the files `.env.*.*.template` to `.env.*.*` and substitute the
environmental variables with the ones from above.

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...
