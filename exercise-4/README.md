# Exercise 4

This exercise is very similar to exercise 3, but with an important change. In order to run this app, we need 2 databases setup on our machine! There needs to be `postgres:9.6` and `mongo:3.6.6-jessie` configured. So we will now configure multiple services using docker-compose and then try running the app. You should see the logs for successful connections for both of them:

Configuration requirements:
- Name the `mongo` container `mongo`, leave the default authentication and database name should be `db`
- Name the `postgres` container `postgres`, leave the default authentication and database name should be `db`
- Use the `depends_on` to ensure that the db containers are started first
- We will be using the default network, so no need to create a new one

If you open `app.js` file - you can see we are connecting to `mongo` and `postgres` respectively according to the name of the service.

