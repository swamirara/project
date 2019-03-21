
A docker compose example project with a MySQL and a Tomcat container linked together.

To run: 

	$ docker-compose up --build

Containers:
- MySQL: on startup, the container executes a simple database initialisation script `./db/mysql-init.sql`, which
  creates a database containing a few tables populated with a few records.
- Tomcat: a simple web application .war file, located within `./tomcat/webapps`, is deployed. The application contains some JSPs to test the database link between the Tomcat and the MySQL containers.
