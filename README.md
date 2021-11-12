# Phoenix Framework 1.2.5 With Elixir Developement environment in Docker. 

For course [The Complete Elixir and Phoenix Bootcamp](https://www.udemy.com/course/the-complete-elixir-and-phoenix-bootcamp-and-tutorial).

Built for comfortable finish of this slightly outdated tutorial. ))

Thanks author of this course for great job. Hope it helps for other, to finish this course in comfortable way.

## Prerequisites:

Install Docker Engine according [this official documentation](https://docs.docker.com/engine/install/).

Install Docker Compose according [this official documentation](https://docs.docker.com/compose/install/).



## Getting started:

Clone this repository. Than cd inside it.

In two separate terminal windows

Run:

`./1_start_docker.sh`

> This will create all required preparations and start Phoenix and Postgres in two connected services.
> Also start pgAdmin at http://localhost:15432
>
> you can Log In with these credentials:
> admin@pgadmin.com
> password
>
> then add our Server to see tables:
>
> 1) Go to "Servers" in the left top corner
>
> 2) In the middle of appeared page press "Add New Server"
>
> 3) In first tab in "Name" field: type name of server for example "docker_db" or "db"
>
> 4) Then press "Connection" tab 
>
> 5) In "Host name/address" field: type "db" (this default hostname of our db in container)
>
> 6) In "Username" field: type "postgres" (this default username for our db in container)
>
> 7) In "Password" field: type "postgres" (this default username for our db in container)
>
> 8) Press "Save" button below in form.
>
> 9) Thats all. Now you can see our database and its tables by path: Servers->db->Databases->discuss_dev->Schemas->public->Tables-> your_preffered_table (in our course its "topics" for example)
>
> 10) For more information you may use [pgAdmin Documentation](https://www.pgadmin.org/docs/pgadmin4/latest/index.html)
>
>     

Then:

`./2_start_dev_shell.sh`

> This run interactive shell into Phoenix container and give you ability to run mix commands as you do in normal way.

As soon as you see command prompt 

`something_yours:/app#`

you should run at the first time

`mix ecto.create`

to create required tables in database

then you feel free to run any commands and of cause run 

`mix phoenix.server`

If everything runs correct you then able to see brand new website by opening [http://localhost:4000](http://localhost:4000) in your favorite browser.
Then of course you can open project from subdirectory ./src with you preferred IDE (VsCode or IntelliJ Idea product or any IDE or editor you suit).

Have nice coding. 

 



