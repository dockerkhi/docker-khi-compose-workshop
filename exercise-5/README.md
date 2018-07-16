# Exercise 5

There will be times when you will have multiple apps in the same repo, a frontend app and a backend app for example. It could be any other kind of setup is as well, may be a seperate backend server for async tasks or a mail server or a load balancer etc. Objective is to build multiple containers and run them.

In this particular example we are doing a MERN setup, one of the important tricks when running seperate servers is that the ports are different - so you need to proxy your requests to the nodeserver during development in order to avoid any CORS issues.

In this final example we will also use `docker-compose run` command to run the tests `npm run tests` on the frontend container. You can find the name of the container by doing `docker ps`.

