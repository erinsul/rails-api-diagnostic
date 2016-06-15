# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What is the purpose of a backend?

```bash
// It stores data over time so that it can be accessed again and also by other users.
```

Which layer in the MVC pattern is used by the controller to fetch data?

```bash
// The model.
```

Which layer in the MVC pattern communicates with the model?

```bash
// The controller.
```

Why don't we use views in our interpretation of the MVC pattern?

```bash
// Views push entire pages of newly created HTML up to the front end, and cause the page to //refresh and be rebuilt. We are building single page apps where that is not supposed to //happen.
```

What does C.R.U.D stand for?

```bash
// Create, Read, Update, Destroy
```

In which part of the MVC pattern can we find C.R.U.D actions?

```bash
// The controller.
```
List at least 5 standard actions that C.R.U.D corresponds to?

```bash
// creating a single instance, updating a single instance, deleting/destroying a single instance, returning a list of all resource instances, returning a single instance
```

A user action fires a `GET` request for `person/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```bash
// The user fires the GET request. It goes to the router, which sends it to the correct //controller (the one handling show). The controller runs a method that will call on the
// correct associated model to fetch the data from the database. The data is passed back to //the controller, and the controller will send it back up front.
```

What is the command to generate a new rails-api app?

```bash
// rails-api new app_name
```

What is the command to start an instance of a rails server?

```bash
// rails server
```

What are the commands to drop, create and migrate a database? (3 bullet points)

```bash
// rake db:drop
// rake db:create
// rake db:migrate
```

What is the command to scaffold a pet with a name and an age?

```bash
// rails-api g scaffold pet name:string age:fixnum
```

List two advantages of using serializers? (2 bullet points)

```bash
// It hides content from those who should not be authorized to view it.
// It transforms objects into JSON for use on the front end.
```
