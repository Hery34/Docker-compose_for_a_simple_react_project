# Docker-compose_for_a_basic_react_project
This repostory contains a basic Docker-compose for a react-project

# #Starting
Copy the Dockerfile in the root directory of the project.


# #About the dockerfile
This Dockerfile uses the latest version of Node.js as the base image, sets the working directory to  /app, copies the  package.json and  package-lock.json files to the working directory, installs the dependencies, copies the rest of the project files to the working directory, exposes port  3000, and starts the application with the  `npm  start` command.

# #About the Docker-compose 

Copy the  docker-compose.yml file in the root directory of the project.

This  docker-compose.yml file defines a service called  app that builds the Docker image using the Dockerfile in the current directory (.), maps port  3000 on the host to port  3000 in the container, and mounts the current directory as a volume in the container.  
  
To start the application in a local environment, you can run the following command in the root directory of your project:
 

`docker-compose up`

This will build the Docker image and start the container. You should be able to access the application at  http://localhost:3000.

