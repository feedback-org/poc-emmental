# poc-emmental

Why emmental ? Take a quick look in the code, there are some `*TBW*` holes all allong the scripts... This is where critical code needs `To Be Written` to make the application working.


## Task 1 : poc-docker

All this task is relative to build a docker postgres flask environment to setup all the development application.

In the end, one Api is ready to be used and some managed scripts can be written to also interact (through flask_script cli) with the running container. One should be able to go to your `poc-docker` branch of your repository and do successfully these commands:

  1. `./poc start` making run the docker containers and the Flask Api is available at localhost:80,

  2. on anther shell, `curl localhost:80/health` returning a json object specifying if the database is ok but with no user data in it for now,

  3. `./poc sandbox` making the app write one user in the database

  4. again, `curl localhost:80/health` should now return database is okay with some users,

  5. `./poc psql` helps to go inside a postgres psql process and `SELECT * from "user"` returns one object,

  6. `./poc python` helps to go inside an api python process and `from models.user import User;User.query.all()` returns the same user object through a sqlalchemy instance.

![Alt Text](https://github.com/feedback-news/poc-emmental/blob/poc-docker/images/poc-docker.gif)
