pur pipeline consists of the following:

## orbs
these are the required packeges to run every aspect of our workflow
in this project we'll need node to install dependencies and build both frontend and backend 
we also need AWS cli as well as EB cli to deploy our application

## jobs
these are the operations to be made through out this pipeline and their sequence will be managed later by workflow section.
the jobs we have here are build and deploy.

## workflow
the pattern bywhich our jobs will be done, first of all we'll de the build job with all of it's aspects (explained later) then we hold and wait for user's approval to perfom the other job which is deploying our app.

so as a result of this pipleline structurem this will happen after pushing any new update into our repo:

### build:
by integrating the new changes into the existing repo it prepares the environment variables and prepare enviroment (node)
then install frontend and backend dependencies
then lint frontend code
then start building frontend
and finally start building backend

### hold:

just wait for human approval top start deploying our app

### deploy:

prepares the environment variables
prepare and install enviroment (node, AWS cli and EB cli )
configure user access data into AWS
start deploying frontend and backend

