# its a basic web server which displays hello world on port 3000

# inside the dockerfile installed npm, exposed the server to port 3000

# inside .github/workflows there are 2 files
# CI-image-push.yaml ---> inside CI file there are 3 steps, login to dockerhub, build the docker image and push
# CD-ec2-deploy.yaml ---> inside CD file there are 3 steps, login to dockerhub, pull the image, run the container

# In  order to run the CD there is a workflow added which waits for CI to complete then starts the CD, to deploy the container on ec2 we need to install runner on ec2 by following the steps which are mentioned while you create the runner. once the runner is up and running we can deploy the container

# also, there are environment variable defines inside the yaml files, username and password which are used to authorize to dockerhub, these are stored in secret and variables inside the repository

