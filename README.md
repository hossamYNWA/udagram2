this project is a full stack application hosted on amazon web service (AWS) .
- you can visit the deployed frontend (on AWS S3) from here http://udagram-frontend-3.s3-website-us-east-1.amazonaws.com
- also you can check the deployed backend (on AWS EB) from [here](http://udagram-api-env.eba-7jpsvdkd.us-east-1.elasticbeanstalk.com/ "here")

##### if you want to install the project locally follow the following: 
1. in *udagram/udagram-frontend* folder install the dependencies through `npm install` then run this `npm run start`
2. while the frontend is waiting for server to run navigate into *udagram/udagram-api* and run `npm install` to set all the required dependencies then run `npm run dev` to run our server.


##### if you wanted to deploy the project manually do the following:
1. set your AWS account configurations
2. navigate into *udagram/udagram-frontend* and run this command in terminal `npm run deploy` to deploy the frontend files into S3
3. install EB CLI and configure *.elasticbeanstalk/config.yml* file
4. navigate into *udagram/udagram-api* and run this command in terminal `npm run deploy` to deploy the backend files into elastic beanstalk

to know morw about the infrastructure and how we make CI/CD for ths project, check the .md files and screenshots in the documentations folder [here](./docs "here")

######## this project made by **udacity** and deployed by **Hossam Mousa**
