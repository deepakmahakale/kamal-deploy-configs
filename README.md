# kamal-deploy-configs

A collection of `config/deploy.yml` files for [kamal](https://kamal-deploy.org/)

**Usage:**

Copy the following files to your kamal project directory:

And replace with the following placeholders:

- `DOCKER_USERNAME` - Your docker username
- `SERVER_IP_ADDRESS` - Your server ip address from Hetzner or Digital Ocean
- `DOMAIN_NAME` - Domain name (example.com)
- `DOMAIN_NAME_WITH_WWW` - Domain name (www.example.com)
- `YOUR_EMAIL_ADDRESS` - email address to generate SSL certificate for letsencrypt

## SQLite

Ensure the `Gemfile` has following entry:

```ruby
# Use sqlite3 as the database for Active Record
gem "sqlite3"
```

This `sqlite` directory includes the following files:

```sh
- config/deploy.yml
- config/deploy2.yml # Use this for second rails app
- config/database.yml
.env
Dockerfile
```

## PostgreSQL

Ensure the `Gemfile` has following entry:

```ruby
# Use sqlite3 as the database for Active Record
gem "pg"
```

This `postgresql` directory includes the following files:

```sh
- config/deploy.yml
- config/database.yml
.env
Dockerfile
```
