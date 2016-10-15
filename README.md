#### Alex & Sally's changes:

* Add migration file for user (only has `username`, `email`, `password_hash`)
* Comment out validations for `first_name` and `last_name` in `User` model
* Add `/session-viewer` and `/session-clearer` to `index.rb` controller
* Add timestamps (with null option set to false) to users table migration

Updated 2016/10/12 by parkyngj

#### Ali's changes:
* Require BCrypt in environment file
* Add user instance #authenticate? method
* Add/Require Faker
* User faker to make stock user seed data for out-of-box/local testing

updated 2016/12/10 by thealicat13

----

### Purpose
The Sinatra Skeleton:

1. Provides a foundation for building challenges or creating a new Sinatra application.
2. Demonstrates a reasonable set of practices around building Sinatra applications.
3. Eases the transition to Rails

### Quickstart

1.  `bundle install`
2.  `shotgun config.ru`

As needed, create models & migrations with the `rake` tasks:

```
rake generate:migration  # Create an empty migration in db/migrate, e.g., rake generate:migration NAME=create_tasks
rake generate:model      # Create an empty model in app/models, e.g., rake generate:model NAME=User
```

### Contributing

We would love for you to help make the skeleton more awesome, There are three ways to contribute:

1. Ask for a bug fix or enhancement!
2. Submit a pull request for a bug fix or enhancement!
3. Code review an open pull request!