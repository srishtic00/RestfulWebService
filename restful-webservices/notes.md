#RESTful Web Services

Retrieve all Users	-GET /users
Create a User		-POST /users
Retrieve one User	-GET /users/{id}
Delete a User		-DELETE /users/{id}

Retrieve all posts of a User	GET /users/{id}/posts
Create a post for a User		POST /users/{id}/posts
Retrieve details of a post		GET /users/{id}/post/{post_id}

#H2 database embedded
Hibernate: drop table if exists user CASCADE 
Hibernate: drop sequence if exists hibernate_sequence
Hibernate: create sequence hibernate_sequence start with 1 increment by 1
Hibernate: create table user (id integer not null, birth_date date, name varchar(255), primary key (id))
