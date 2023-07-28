# AVANSER PHP Coding Test

## Objective

This compact coding exercise forms part of the selection process for AVANSER job vacancies.
It comprises three primary tasks meant to gauge your comprehension of PHP frameworks and database operations.

## Goal

The three tasks that need to be completed are:

1. Create a migration script that will create a new column in the database
named **duration** as an INT(11) field and fill in the new field for the existing
rows by calculating the duration in seconds, subtracting the call_start time from
the call_end time.
1. Create an HTML view showing a summary for each client_id, with a count of the calls
and total duration of the calls.
1. On the summary page, add a filter for client ids, dates and numbers so that the summary page
shows data for the appropriate clients, date ranges or number selections.
1. Provide a link from the summary page to a details page that will show a list 
of the calls from the database, along with the same total call count and duration.


## Guidelines

Use a PHP framework of you choosing, such as Laravel. Your code must adhere to the PSR-12 coding standard.

## Bonus Points are awarded for

- The use of a UI framework, such as Svelte, Vue.js, Next.js & React
- Asynchronous communication between client and server
- Use of Test Driven Development methodology
- Providing a Readme on code design and employed framework

## Instructions for using the sample database and docker files

The Docker files provided will build an environment with PHP, Apache, MySQL and
PHPMyAdmin. `docker compose build` and `docker compose up` will be helpful
commands once Docker Desktop is installed. Docker Compose documentation can be 
found at [https://docs.docker.com/compose/gettingstarted/](https://docs.docker.com/compose/gettingstarted/)

MySQL will have a database initialised and accessible through the credentials
provided in the docker-compose.yaml file.

The `src` folder should be used to store the PHP code required.

The Docker configuration can be updated to include Composer locally if this
makes builds easier.

PHPMyAdmin can be utilised via [http://localhost:8008](http://localhost:8008).
The PHP app can be seen at [http://localhost:8000](http://localhost:8000). If
these ports are used by your environment already they can be updated in the
Docker config.
