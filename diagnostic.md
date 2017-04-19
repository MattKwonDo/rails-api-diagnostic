# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```md
to manage data (store created and updated data, send and receive data)
```

Which layer in the MVC pattern is used by the controller to fetch data?

```md
model
```

Which layer in the MVC pattern communicates with the model?

```md
controller
```

Why don't we use views in our interpretation of the MVC pattern?

```md
they are outdated, we don't need no views.
```

What does C.R.U.D stand for?

```md
create read update delete
```

In which part of the MVC pattern can we find C.R.U.D actions?

```md
model
```

List at least 5 standard rails actions that C.R.U.D requests correspond to?

```md
index show create update destroy new edit
```

A user action fires a `GET` request for `/people/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```md
- router receives request and sends it to the indicated controller
- if the controller exists, then the controller will send the request to
the indicated model (if it exists).
- the model will take the request and process it.
- if the right number of arguments are provided and all required
arguments are valid, the model will be able to successfully send data
back to the controller, which will then send data to the browser who Will
view the data.
```

What is the command to generate a new rails-api app?

```bash
rails-api new my_api
```

What is the command to start an instance of a rails server?

```bash
bin/rails server
```

What are the commands to drop, create, migrate and seed a database from the command
line? (5 bullet points)

```bash
- bin/rake db:drop
- bin/rake db:create
- bin/rake db:migrate
- bin/rake db:seed
- bin/rake db:examples
```

What is the command to scaffold a pet with a name and age attributes (hint:
Also think of the data types for each attribute)?

```bash
rails generate scaffold pet name:string name:string age:integer
```
