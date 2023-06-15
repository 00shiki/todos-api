# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

ruby 3.2.2

* System dependencies

```sh
$ bundle install
```

* Database creation

```sh
$ rails db:create
```

* Database initialization

```sh
$ rails db:migrate
```

* How to run the test suite

```sh
$ bundle exec rspec
```
# API Docs

- Endpoint : POST /signup

Request Body

```json
{
    "name" : "foobar",
    "email" : "foo@bar.com",
    "password" : "foobar",
    "password_confirmation" : "foobar"
}
```

Response body

```json
{
    "message" : "Account created successfully",
    "auth_token" : "foo"
}
```

- Endpoint : POST /auth/login

Request Body

```json
{
    "email" : "foo@bar.com",
    "password" : "foobar"
}
```

Response body

```json
{
    "auth_token" : "foo"
}
```

- Endpoint : GET /todos

- Endpoint : GET /todos/:id

- Endpoint : PUT /todos/:id

- Endpoint : DELETE /todos/:id

- Endpoint : GET /todos/:id/items

- Endpoint : PUT /todos/:id/items

- Endpoint : DELETE /todos/:id/items
