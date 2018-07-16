# Exercise 3

Time to up the ante, in this project you will convert your Docker image to run on Docker Compose. The Dockerfile is already provided, for practice you can first try running this using just the `docker run` command. This will launch a NodeJS api on port `3000`. When linking the volumes remember not to override the node_modules folder. Once you have got it running, make some changes in views/index.hbs and refresh the page to see the changes.

If you are looking for node to auto-restart when making the change, then I would recommend using nodemon as the startup service. You can override that using the command prop in the compose file.