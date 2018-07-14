# Exercise 2

This exercise uses the image `httpd:2.4-alpine` to serve an html page through the container using Apache. Dont forget to configure your ports, 
httpd serves on port `80` of the container, you can configure it to run on port `8080` of the system. And Apache serves the `/var/www/` folder
by default, so we want to attach our volume on that.