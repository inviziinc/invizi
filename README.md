# README

## Local Development Setup

### Requirements

- Ruby >3 (see `Gemfile`)
- PostgreSQL >9.3 (ideally, latest stable version)

After cloning the repo, the basic setup commands are:

```sh
cd invizi
cp .env.example .env
bin/setup
bin/dev

# TODO: Optionally, load demo data
rake demo_data:reset
```
