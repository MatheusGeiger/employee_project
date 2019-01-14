# Parent repository to join employee project repositories

## API

https://bitbucket.org/matheusgeiger/node-employee-api/src/master/

## CLIENT API

https://bitbucket.org/matheusgeiger/angular-cli/src/master/

### USAGE

## SUBMODULES

This project use git submodules. Read more https://git-scm.com/book/en/v2/Git-Tools-Submodules

After clone, inicialize the submodules:
- `git submodule init`

![Submodule Init](/docs/images/submodule_init.png "Submodule Init")

Git will not download the contents of the submodules when cloning this project. To make the clone of all the commands you must execute:
- `git submodule update`

![Submodule Update](/docs/images/submodule_update.png "Submodule Update")

before running project use `git submodule foreach git pull origin master` to get the last version of code provided in master branch.

## RUNNING PROJECT

Using docker you can up the project with command `docker-compose up --build`

This command will up and create three containers:
- API: the employees and users api
- ANGULAR_CLI: the client view with graphs and table from employees
- MONGO: the database to persist values from employees and user

## URLS

After run up the project  command we can access then using urls above:
- API: http://localhost:3001/api/employess
- ANGULAR_CLI: http://localhost:4200