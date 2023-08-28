# Rails API

## Run project with docker
**Create a docker image**
```console
$ docker build -t rails-api .  
```

**Create a container**
```console
$ docker run --name rails-api --net=host -p 3000:3000 rails-api
```

## Project Setup

**Install all gems**:

```console
$ bundle install
```

**Update the database with new data model**:

```console
$ rails db:migrate
```

**Feed the database with default seeds**:

```console
$ rails db:seed
```

**Start the web server on `http://localhost:3000` by default**:

```console
$ rails server
```

| TYPE   | Path
|--------| ------ 
| POST   | /register |
| POST   | /login   |
| GET    | /posts |
| GET    | /posts/:post_id | 
| POST   | /posts |
| PUT    | /posts/:post_id |
| DELETE | /posts/:post_id |
| GET    | /posts/:post_id/comments |
| GET    | /posts/:post_id/comments/:comment_id |
| POST   | /posts/:post_id/comments |
| PUT    | /posts/:post_id/comments/:comment_id |
| DELETE | /posts/:post_id/comments/:comment_id |