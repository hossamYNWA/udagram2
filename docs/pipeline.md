*after pushing anu new change into our repo, circleCi does the folllowing:
### build:
1.     by integrating the new changes into the existing repo
2.     prepares the environment variables
3.     prepare enviroment (node)
4.     install frontend and backend dependencies
5.     lint frontend code
6.     start building frontend
7.     start building backend

### hold:

-     waiting for human approval top start deploying our app

### deploy:

-     prepares the environment variables
-     prepare and install enviroment (node, AWS cli and EB cli )
-     configure user access data into AWS
-     start deploying frontend and backend

