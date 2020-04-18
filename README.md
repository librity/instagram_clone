# Instagram clone

Forked from https://github.com/vinnydeveloper/fake_instagram

## Resources

- https://app.diagrams.net/ aka draw.io
- https://www.slant.co/options/166/alternatives/~draw-io-alternatives
- https://dev.mysql.com/downloads/workbench/
- https://www.apachefriends.org/pt_br/index.html
- https://hub.docker.com/_/mysql/
- https://dbeaver.io/
- https://sqldbm.com/Home/

## Sequelize

- https://sequelize.org/v5/
- https://sequelize.org/master/manual/migrations.html
- https://sequelize.org/master/manual/raw-queries.html
- https://sequelize.org/master/manual/model-basics.html
- https://sequelize.org/master/manual/querying.html
- https://sequelize.org/master/manual/raw-queries.html

## Setup

1. copy dotenv:

```bash
$ cp .env.example .env
```

2. create a persistent mysql5 docker container:

```bash
$ docker run --name mysql_5_7_29 -e MYSQL_ROOT_PASSWORD=root -p 3306:3306 -d mysql:5
```

3. install our dependencies

```bash
$ yarn
```

4. Create, migrate and seed our database:

```bash
$ yarn sequelize db:create
$ yarn sequelize db:migrate
$ yarn sequelize db:seed:all
```

5. start our dev server:

```bash
$ yarn start
```
